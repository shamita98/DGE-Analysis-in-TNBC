# DGE-Analysis-in-TNBC

**Project Title:**
Differential Gene Expression Analysis in Triple Negative Breast Cancer

In this project, I performed a differential gene expression analysis to compare the bulk transcriptome of Triple Negative Breast Cancer (TNBC) primary tumor samples of TCGA Breast Invasive Carcinoma cohort and normal breaast tissue samples of GTEX cohort.

**Methodology**
<br>**1. Identification of TNBC Samples**
TNBC primary tumor sample IDs that have RNA-sequencing gene expression data were obtained from [cBioPortal of Cancer Genomics database](http://cbioportal.org). The samples were part of TCGA Breast Invasive Carcinoma (Firehose Legacy) cohort. There were 114 TNBC samples with RNA-sequencing data, and their clinical profiles including sample IDs were downloaded. TNBC primary tumor samples were identified using the following criteria:
<br>• Cancer Type : Breast Cancer
<br>• Sample Type: Primary
<br>• ER status by IHC: negative
<br>• PR status by IHC: negative
<br>• HER2 status by IHC: negative

**2. Differential Gene Expression Analysis**
Genome-wide differential gene expression analysis was carried out to compare 114 TNBC primary tumor samples and 179 normal breast tissue samples of GTEx cohort using Bulk RNA-seq analysis pipeline provided by [UCSC-Xena platform] (https://xenabrowser.net/). Both the primary tumor and normal breast tissue samples are part of TCGA Target GTEx study, where TCGA, Target and GTEx samples are reanalyzed using the same bioinformatics pipeline to eliminate batch effects contributing to unwanted variance. TCGA Target GTEx study also has solid normal tissue samples which is normal breast tissue adjacent to the tumor, and they are often used as healthy controls to compare with tumor samples. However only 16 out of 114 TNBC patients have matched normal samples. In addition, gene expression profiling of solid normal tissue samples showed that they resemble tumor tissue more. Therefore, in this study, TNBC primary tumor samples were compared with GTEx normal tissue samples which belong to non-diseased individuals. Differential gene expression analysis results were downloaded, and downstream analyses were done in R (version 4.3.1) using RStudio software. Differentially expressed genes that are significant were filtered using the following criteria: | log2fold_change | > 1 and adjusted p-value < 0.05. Upregulated genes have log2fold_change > 1, whereas downregulated genes have log2fold_change < 1. The results of differential gene expression analysis were visualized through a volcano plot. The source code for visualization is available [here.](https://github.com/shamita98/DGE-Analysis-in-TNBC/blob/d562987ac142f1952f9a4b7d54907f468e71db75/Volcano%20Plot%20Visualization%20of%20Differentially%20Expressed%20Genes%20in%20Triple%20Negative%20Breast%20Cancer.pdf)
