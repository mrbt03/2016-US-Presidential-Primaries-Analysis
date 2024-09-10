# 2016 US Presidential Primaries Analysis

This project explores voting trends in the 2016 Democratic and Republican Primaries, visualizes key patterns, and builds predictive models to forecast how a given county will vote in each respective primary. The analysis is conducted using Python with libraries such as `pandas`, `seaborn`, `matplotlib`, `xgboost`, and `scikit-learn`.

## Overview

The analysis focuses on understanding the demographic and socio-economic factors that influenced voting patterns in the 2016 primaries. The project involves:

- **Data Preparation**: Loading and cleaning data related to county demographics and primary results.
- **Exploratory Data Analysis (EDA)**: Visualizing relationships between demographics and primary winners for both parties.
- **Predictive Modeling**: Building and evaluating multiple models (Logistic Regression, XGBoost) to predict primary outcomes based on county data.

## Data Sources

- **Primary Results**: `primary_results.csv` - Contains voting results for each candidate by county.
- **County Demographics**: `county_facts.csv` and `county_facts_dictionary.csv` - Provide demographic and economic data for each county.

## Analysis Workflow

1. **Data Loading and Exploration**:
   - Load primary results and county facts data.
   - Examine data structure, summary statistics, and missing values.

2. **Data Cleaning and Feature Engineering**:
   - Create separate DataFrames for Democratic and Republican primaries.
   - Merge county demographics with primary results to create enriched datasets.

3. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of key demographics across different candidates.
   - Analyze the correlation between demographic factors and voting outcomes.

4. **Model Building and Evaluation**:
   - Use Logistic Regression (with and without regularization) to predict primary winners.
   - Apply XGBoost with GridSearchCV to optimize hyperparameters and improve model performance.
   - Evaluate model performance using accuracy scores and classification reports.

## Key Findings

- **Republican Primaries**:
  - XGBoost outperformed logistic regression models, achieving an accuracy of 84% in predicting primary outcomes.
  - Key predictors include the percentage of black and Hispanic populations and age distribution within counties.

- **Democratic Primaries**:
  - Logistic regression without regularization achieved the highest accuracy of 80%.
  - Higher population densities and a higher percentage of black population are strong indicators for counties won by Hillary Clinton.

## Technologies Used

- **Programming Language**: Python
- **Libraries**: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`, `xgboost`

## How to Run the Analysis

1. **Clone the repository**:
   ```bash
   git clone https://github.com/mrbt03/2016-US-Presidential-Primaries-Analysis.git
   cd 2016-US-Presidential-Primaries-Analysis

