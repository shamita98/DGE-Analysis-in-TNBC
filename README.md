# DGE-Analysis-in-TNBC

**Project Title:**
Differential Gene Expression Analysis in Triple Negative Breast Cancer

In this project, I performed a differential gene expression analysis to compare the bulk transcriptome of Triple Negative Breast Cancer (TNBC) primary tumor samples of TCGA Breast Invasive Carcinoma cohort and normal breaast tissue samples of GTEX cohort.

**Methodology**
<br>**1. Identification of TNBC Samples**
TNBC primary tumor sample IDs that have RNA-sequencing gene expression data were obtained from [cBioPortal of Cancer Genomics database](http://cbioportal.org). The samples were part of TCGA Breast Invasive Carcinoma (Firehose Legacy) cohort. There were 114 TNBC samples with RNA-sequencing data, and their clinical profiles including sample IDs were downloaded. TNBC primary tumor samples were identified using the following criteria:
• Cancer Type : Breast Cancer
• Sample Type: Primary
• ER status by IHC: negative
• PR status by IHC: negative
• HER2 status by IHC: negative
