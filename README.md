# BRCA-Therapeutic-Targets-Survival
Prognostic evaluation and overall survival analysis of top 10 hub genes in Breast Invasive Carcinoma (BRCA) using the GEPIA2 platform.
# Survival Analysis of Top 10 Hub Genes in Breast Invasive Carcinoma (BRCA)

## Overview
This repository contains the overall survival (OS) analysis for the top 10 hub genes identified as potential key therapeutic targets in Breast Invasive Carcinoma (BRCA). Following a rigorous network analysis of gene interactions (using degree centrality), these top genes were evaluated for their prognostic value to determine if their expression levels significantly impact patient survival outcomes. 

## Methodology
The survival analysis was conducted using the **[GEPIA2 web tool](http://gepia2.cancer-pku.cn/#index)** (Gene Expression Profiling Interactive Analysis). 
* **Dataset:** Breast Invasive Carcinoma (BRCA) from TCGA.
* **Method:** Kaplan-Meier survival curves.
* **Grouping:** Patients were divided into "High" and "Low" expression groups based on median gene expression cutoffs.
* **Metrics:** Log-rank test p-values and Hazard Ratios (HR) were calculated to assess statistical significance.

## Results Summary
The analysis of the top 10 identified genes yielded the following prognostic data:

| Gene Symbol | Hazard Ratio (HR) | Log-rank p-value | Significance (p < 0.05) |
| :--- | :--- | :--- | :--- |
| **RRM2** | 1.3 | 0.21 | No |
| **KIF4A** | 1.6 | 0.024 | **Yes** |
| **NEK2** | 1.3 | 0.24 | No |
| **MELK** | 1.2 | 0.38 | No |
| **ASPM** | 0.99 | 0.95 | No |
| **TPX2** | 1.2 | 0.53 | No |
| **ESR1** | 1.2 | 0.46 | No |
| **FN1** | 1.5 | 0.064 | Borderline |
| **NCAPG** | 1.4 | 0.16 | No |
| **TOP2A** | 1.0 | 0.96 | No |

### Key Findings
* **KIF4A** is the most clinically significant gene among the top 10 analyzed. High expression of KIF4A correlates with a poorer overall survival rate in BRCA patients (HR = 1.6, p = 0.024), making it a strong candidate for further targeted therapeutic research.
* **FN1** showed borderline significance (p = 0.064), suggesting a potential trend that may warrant investigation in larger or more specific cohorts.

## Repository Contents
* `GEPIA2_SurvivalAnalysis_Top10_BRCA.pdf`: The complete exported document containing the 10 Kaplan-Meier survival plots generated from GEPIA2.
## Author
**Nagendra** GitHub: [@DrNagendra619](https://github.com/DrNagendra619)
