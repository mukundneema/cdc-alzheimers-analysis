CDC Alzheimer's Disease Analysis

This repository contains the data, code, and analysis for my research project with Professor Zheming Gao. The project uses CDC Alzheimer's and Healthy Aging data to investigate relationships between Alzheimer's-related health measures and other health and demographic variables.

Dataset

The primary dataset is the CDC Alzheimer's and Healthy Aging Data.

- File: `cdc_alzheimers_data.csv`
- Years: 2015–2022
- Locations: 59
- Rows: 284,142
- Columns: 33
- Data source: CDC
- Dataset ID: `hfr9-rurv`

The dataset is stored using **Git LFS** because of its large file size.

Code

The `CDC` script contains code for:

- Loading the CDC dataset
- Examining dataset structure and data types
- Checking missing values
- Examining unique values and distributions
- Generating descriptive statistics
- Filtering data by topic, age group, and other variables
- Analyzing Subjective Cognitive Decline (SCD)
- Analyzing lifetime diagnosis of depression
- Comparing health measures between age groups
- Examining relationships between depression and SCD
- Performing statistical tests and regression analyses

Current Analysis

Current analysis has focused on:

Subjective Cognitive Decline

Comparison of reported SCD prevalence between:

- Adults aged 50–64
- Adults aged 65 years or older

Analyses include descriptive statistics, Welch's t-test, IQR-based outlier analysis, and sensitivity analysis after removing statistical outliers.

Lifetime Diagnosis of Depression

Comparison of reported lifetime depression prevalence between:

- Adults aged 50–64
- Adults aged 65 years or older

Analyses include descriptive statistics, Welch's t-test, IQR-based outlier analysis, and sensitivity analysis.

Depression and SCD

The relationship between reported lifetime depression prevalence and reported SCD prevalence is being investigated separately for the two age groups.

Analyses include:

- Pearson correlation
- Spearman correlation
- Fisher's z-test for comparing correlations
- Linear regression
- Interaction analysis
- Residual diagnostics
- Q-Q plots
- Sensitivity analysis involving statistical outliers

Data Processing

The CDC dataset is saved locally in the repository so that analysis can be reproduced without downloading the dataset from the CDC website each time the code is run.

The raw dataset is not modified during analysis unless explicitly stated in the corresponding analysis code.

Notes

The CDC dataset consists of aggregated survey estimates rather than individual-level observations. Therefore, statistical results should be interpreted as associations among reported population-level estimates rather than individual-level causal relationships.

Statistical outliers are not automatically treated as erroneous observations. Outlier analyses are used as sensitivity analyses to evaluate how unusual observations affect the results.

Research Status

This repository is an ongoing research project. Analyses, code, and conclusions may be updated as additional questions are investigated and feedback is incorporated.
