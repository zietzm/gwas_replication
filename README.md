# Replication of GWAS

## Title

Replicability across populations of genome-wide significant SNPs and enriched biological processes in type 2 diabetes

## Abstract

Type 2 diabetes mellitus (T2D) is a chronic metabolic disorder affecting over 30 million individuals in the United States. The pathogenesis of T2D depends on a number of factors and is known to have a genetic component. While a number of studies have been conducted and have found SNPs with genome-wide significance for T2D, such studies are often limited by their inclusion of limited population diversity. Recent meta-analyses of GWA studies in the Japanese (2019) and Sub-Saharan African (2019) populations, and a more distant (2012) large-scale GWAS meta-analysis in European populations afford an opportunity to compare the replicability of genome-wide significant SNPs and enriched biological processes between populations. We hypothesized that enriched biological processes are more replicable across populations than genome-wide significant SNPs. In this study we evaluate the replicability of significant SNPs across the Japanese, European, and African populations included in these studies, and we perform gene set enrichment analyses on the SNPs from each study (GSEA-SNP) to evaluate the replicability of enriched biological processes. **Summary of results will go here**

## Data sources

### SNP resources

* Japanese T2DM meta-analysis (Suzuki, et al.)
    * GWAS Catalog:  https://www.ebi.ac.uk/gwas/studies/GCST007847
    * Paper: https://www.nature.com/articles/s41588-018-0332-4
* European T2DM meta-analysis  (Morris, et al.)
    * GWAS Catalog: https://www.ebi.ac.uk/gwas/studies/GCST005047
    * Paper: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3442244/
* African TDDM study (Chen, et al.)
    * GWAS Catalog: https://www.ebi.ac.uk/gwas/studies/GCST008114
    * Paper: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6560001/

### Gene set resources

To investigate enriched gene sets and their replicability between these two studies, we used GSEA gene sets for biological processes (BP: “GO biological process”, 7350 gene sets). These are available in MSigDB, a resource provided by the Broad Institute (link: MSigDB).

## Methods

### Data collection

Data from both studies was acquired through the EBI GWAS Catalog (https://www.ebi.ac.uk/gwas/). The studies used in this analysis were GCST007847, GCST005047 and GCST008114. Included for each study were SNPs, mapped genes, and p-values for each SNP.

### GSEA-SNP

For this study we used The Molecular Signatures Database (MSigDB), a collection of 22596 annotated gene sets that are separated into eight major collections e.g., “H: hallmark gene sets” and “C5: GO gene sets”. The GSEA gene sets used in this analysis were classified under biological processes (BP: “GO biological process”, 7350 gene sets). We conducted our GSEA-SNP analysis using GSEA v4.0.2 for Linux, provided by the Broad Institute (http://software.broadinstitute.org/gsea/). GSEA-SNP is an extension of GSEA where the analysis is done at the SNP level instead of the gene level and uses a more powerful, genotype-based test: the MAX-test. (https://academic.oup.com/bioinformatics/article/24/23/2784/180339)

### Replicability

To compare the replicability of genome-wide significant SNPs and enriched biological processes, we created two separate contingency tables. The first table represents the SNPs that are associated with T2D at genome-wide significance. The second table represents biological process gene sets significantly enriched among T2D-associated genes (mapped from associated SNPs). Both of these will correspond to a three-way comparison between GWA studies.
