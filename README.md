# Life Expectancy Analysis Using R

## Overview

This repository contains the R code used for analyzing global life expectancy data. The analysis is part of a study aimed at understanding the determinants of life expectancy across countries and continents. Key factors such as economic indicators, health infrastructure, and societal aspects are explored using statistical and machine learning techniques.

## Dataset

- **Source**: The dataset was obtained from Kaggle and includes data from the World Health Organization (WHO) and United Nations.
- **Details**: The dataset includes:
  - 22 variables and 2,938 observations, later reduced to 1,649 observations after preprocessing.
  - **Dependent Variable**: Life expectancy (years).
  - **Predictors**: Factors such as GDP, adult mortality, schooling, health expenditure, and immunization coverage.

## Preprocessing

- Addressed missing data by either removing rows or imputing values.
- Grouped countries into continents to handle multicollinearity issues.

## Models

### 1. Multiple Linear Regression (MLR)
- Performed log transformation to address non-linearity and variance issues.
- Used stepwise variable selection for model simplification and improved interpretability.

### 2. Machine Learning Models
- **Gradient Boosting**
- **Random Forest**

### 3. Evaluation Metrics
- Mean Squared Prediction Error (MSPE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)

## Key Findings

- The MLR model explained 86.7% of the variability in life expectancy.
- Random Forest outperformed other models in prediction accuracy but at the cost of interpretability.

## R Scripts

1. **Data Preprocessing**: Handles missing values and organizes data into continents.
2. **Model Development**: Includes MLR with log transformation and variable selection.
3. **Model Evaluation**: Provides diagnostics and accuracy metrics.
4. **Prediction**: Generates life expectancy predictions using the trained models.

## Instructions

### Setup
1. Install the required R packages: `lmtest`, `car`, `MASS`, `ggplot2`, `caret`, `randomForest`, `gbm`.
2. Place the dataset (`Life_Expectancy_Data.csv`) in the working directory.

### Running the Code
1. Execute the R scripts sequentially:
   - Data Preprocessing
   - Model Development
   - Model Evaluation
   - Prediction
2. Outputs include model summaries, diagnostic plots, and prediction results for different models.

## Conclusion

This analysis highlights the critical factors influencing life expectancy globally. While machine learning models provide high prediction accuracy, MLR offers better interpretability for understanding the underlying relationships.
