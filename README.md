## Bayesian Hierarchical Analysis of Serious Crime Rates in Los Angeles

### Overview
This project analyzes the variation in serious crime rates across 21 LAPD districts
using a Bayesian hierarchical modeling framework. Since districts differ in population
size and total crime counts, raw proportions can be misleading. A hierarchical model
allows partial pooling across districts to produce more stable and interpretable estimates.

### Data
The raw LAPD crime dataset used in this project is not included in this repository due to GitHub file size limitations.
However, the data are publicly available from:
https://catalog.data.gov/dataset/crime-data-from-2020-to-present

- Dataset name: Crime Data from 2020 to Present
- Source: Los Angeles Open Crime Data (Data.gov)
- Units: 21 LAPD districts
- Response: Proportion of serious crimes among total reported crimes

### Methods
- Binomial likelihood for district-level serious crime counts
- Hierarchical prior on district crime probabilities
- Posterior inference via MCMC
- Posterior predictive checks and prior sensitivity analysis

### Results
The hierarchical model shrinks extreme district-level estimates toward the overall mean,
reducing variance while preserving meaningful between-district differences. Districts
with limited observations benefit most from partial pooling.

### Files
- `report.pdf`: Full analysis and results
-  `data`: Raw dataset from Kaggle
-  `code`: R scripts for data cleaning, modeling, and visualization

### Authors
Yiming Gao, Yuran Wang, Molin Yang, Rongsheng Zhang
