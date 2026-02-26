Here’s an enhanced description you can put in your `description.md` for the GitHub repository, incorporating details from the dataset and competition context:

---

# Poverty Prediction Challenge – DrivenData

This repository contains a solution for the **Poverty Prediction Challenge** hosted by DrivenData. The goal is to predict household-level daily consumption per capita in USD (2017 PPP) using survey data from multiple years.

## Dataset Overview

The provided training dataset consists of three panels of household surveys conducted in different years. Each household responds to a wide variety of questions, and their responses are recorded along with the household’s daily consumption per capita. Household weights are included to reflect the household's representativeness of the population. From these weights and consumption values, the consumption distribution is computed, and the poverty rate is calculated—the proportion of the population with consumption below a specific threshold.

### Files Provided

* **`train_hh_features.csv`** – Household-level survey features, including:

  * Identifiers & sampling information
  * Welfare & expenditure information
  * Demographics & household composition
  * Education & employment
  * Housing & utilities
  * Geography
  * Food-consumption indicators (last 7 days)

* **`train_hh_gt.csv`** – Ground truth labels: daily per capita consumption (USD).

* **`feature_descriptions.csv`** – Full data dictionary describing each feature.

* **`feature_value_descriptions.csv`** – Descriptions of coded indicator values.

### Objective

The task is to **predict household-level consumption** for each survey response in the test set. Predictions should reflect the daily per capita consumption in **2017 USD PPP**.

### Notes

* Population-expanded weights are included to allow accurate population-level estimates.
* Categorical and numeric survey features provide insights into household demographics, expenditures, and living conditions.
* The challenge emphasizes robust modeling for socio-economic prediction from structured survey data.

### Approach (Optional)

* Feature engineering to handle categorical codes and missing values.
* Regression modeling to predict continuous consumption values.
* Evaluation using weighted metrics considering household survey weights.


