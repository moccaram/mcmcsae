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

# Prediction Script for MCMC Spatial Model (BYM2)
This script is used for generating predictions based on the MCMC results from the BYM2 spatial model. 

## Key Features:

- **Prediction Calculation**: Combines fixed and random effects from MCMC results to generate predictions.
- **Summary Statistics**: Computes the mean, standard deviation, and confidence intervals for the predictions.
- **Log-Transformation**: Reverses any log-transformation applied to predictions during model fitting.
- **Result Storage**: Stores predictions, standard deviations, and confidence intervals in the dataset.

# Bangladesh DHS Data Analysis for U5MR Estimation

This repository contains the R code to process demographic and geographic data for Bangladesh and calculate the Under-5 Mortality Rate (U5MR) for different time periods. The analysis is based on data from the Bangladesh Demographic and Health Surveys (BDHS), along with spatial shapefiles for different administrative regions of Bangladesh.

## Prerequisites

To run this analysis, you will need to have the following libraries installed:

- `sf` – For handling spatial data and shapefiles
- `stringi` – For string manipulation
- `dplyr` – For data manipulation

You can install these packages using the following commands in R:

```r
install.packages("sf")
install.packages("stringi")
install.packages("dplyr")
