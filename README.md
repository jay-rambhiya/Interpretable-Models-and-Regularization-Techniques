# Interpretable Models and Regularization Techniques for Classification and Regression

This project involves building interpretable models and exploring regularization techniques for regression. Key methods include decision trees, LASSO, ridge regression, and gradient boosting. The project also covers handling missing data, feature selection, and model evaluation. This project is part of Homework 5 for the DSCI 552 course.

## Table of Contents
- [Project Overview](#project-overview)
- [Datasets](#datasets)
- [Decision Trees](#decision-trees)
- [LASSO and Boosting for Regression](#lasso-and-boosting-for-regression)
- [Requirements](#requirements)

## Project Overview
The main objectives of this project are:
1. Building interpretable models using decision trees and converting the decision rules into a readable format.
2. Applying regularization techniques (LASSO, Ridge) and feature selection for regression.
3. Utilizing boosting methods to enhance model performance.

## Datasets
1. **Acute Inflammations**:
   - [Dataset Link](https://archive.ics.uci.edu/ml/datasets/Acute+Inflammations)
   - Used for building and pruning decision trees, focusing on interpretability.

2. **Communities and Crime**:
   - [Dataset Link](https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime)
   - Used for regression with LASSO, Ridge, and boosting techniques. The data requires handling missing values and selecting significant features.

## Decision Trees
1. **Tree Construction**:
   - Built a decision tree on the Acute Inflammations dataset and visualized it.
2. **IF-THEN Rules**:
   - Converted decision paths into a set of IF-THEN rules for interpretability.
3. **Pruning**:
   - Applied cost-complexity pruning to simplify the tree, improving interpretability.

## LASSO and Boosting for Regression
1. **Data Preprocessing**:
   - Missing values in the Communities and Crime dataset were imputed.
   - Generated a correlation matrix to examine feature relationships.
   - Calculated the Coefficient of Variation (CV) for each feature, selecting the top features for analysis.
2. **Regression Models**:
   - **Linear Regression**: Trained a linear regression model on the training set and evaluated its performance on the test set.
   - **Ridge Regression**: Performed cross-validation to select the optimal regularization parameter λ.
   - **LASSO Regression**: Identified important features using LASSO with cross-validation and compared results using standardized features.
   - **Principal Component Regression (PCR)**: Selected the optimal number of components via cross-validation.
3. **Boosting**:
   - Implemented an L1-penalized gradient boosting model using XGBoost, with α selected via cross-validation.

## Requirements
The project requires:
- Python
- Libraries: `numpy`, `pandas`, `matplotlib`, `sklearn`, `xgboost`
