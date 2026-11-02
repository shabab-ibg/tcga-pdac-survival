# TCGA-PDAC Survival Analysis

Survival analysis of pancreatic ductal adenocarcinoma (PDAC) using TCGA clinical and gene expression data.

## Question
Does gene expression add prognostic value beyond clinical stage for PDAC survival?

## Data
- TCGA-PAAD cohort (160 patients after quality filtering)
- 89 death events
- Source: https://portal.gdc.cancer.gov/

## Methods
- Cox proportional hazards baseline (stage, age, sex)
- Penalized Cox regression on gene expression
- Cross-validated C-index comparison

## Structure
- `notebooks/01_cohort_lock.ipynb` - Cohort construction and QC
- `notebooks/02_gene_filtering.ipynb` - Gene filtering (in progress)
- `notebooks/03_baseline_cox.ipynb` - Clinical baseline model (in progress)
- `notebooks/04_penalized_cox_cv.ipynb` - Expression model with CV (in progress)

## Setup
```bash
pip install -r requirements.txt
```

## Status
Work in progress - second-year BTech CSE (AI/ML) side project.
