# Survey Analysis for Causes of Death
This script processes survey data to compute direct estimates of causes of death. The key functionalities include:

- **Survey Analysis**: Handles complex survey design features such as weights, strata, and clusters.
- **Smoothing and Prediction**: Applies smoothing techniques to adjust responses and sample sizes. Uses a Generalized Variance Function model to predict standard errors.
- **Data Imputation**: Replaces missing values with division-level means to ensure completeness of the data.

# Spatial Modeling Using MCMC for Direct Estimates
This script demonstrates how to perform spatial modeling with MCMC using the `mcmcsae`, `spdep`, and `sf` R packages. 
The analysis addresses spatial dependencies, heteroscedasticity, and temporal-spatial interactions in direct estimates data.

## Key Features:

- **Spatial Modeling (BYM2)**: Fits a BYM2 spatial model to account for spatial dependencies, random walks, and spatial-temporal interactions.
- **MCMC Simulation**: Runs MCMC simulations to estimate model parameters with multiple chains to ensure convergence.
- **Heteroscedasticity Handling**: Models varying variance (heteroscedasticity) across predictors such as year and standard error.
- **Model Validation**: Summarizes MCMC results and saves the outputs for further analysis.
