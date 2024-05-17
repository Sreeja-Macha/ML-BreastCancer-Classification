# ML-BreastCancer-Classification

# Logistic Regression and Feature Selection Analysis for Breast Cancer Classification

## Overview

This project explores and analyzes the Breast Cancer Dataset, aiming to classify breast cancer tumors as malignant or benign using logistic regression. The analysis includes data preprocessing, model development, evaluation, and feature selection, providing a comprehensive insight into predictive modeling and interaction analysis in the context of medical data.

## Dataset Description

The Breast Cancer Dataset comprises features computed from a digitized image of a fine needle aspirate of a breast mass. These features describe the characteristics of the cell nuclei present in the image. The primary objective is to predict the diagnosis of breast cancer, classifying tumors as either malignant or benign.

## Project Workflow

### 1. Data Exploration and Visualization

Initial exploration and visualization were conducted to understand the distribution and relationships of different features in the dataset. Key steps included:
- **Statistical Summaries**: Generating summary statistics to grasp the central tendencies and dispersions of the features.
- **Visualizations**: Creating histograms and box plots to visualize the data distribution and identify any patterns or anomalies.

### 2. Logistic Regression Model Development

A logistic regression model was developed to predict the malignancy of the tumors. Key preprocessing steps included:
- **Data Cleaning**: Removing any extraneous columns and handling missing values.
- **Encoding Categorical Variables**: Converting categorical data into numerical format for the model.
- **Addressing Multicollinearity**: Identified highly correlated predictors (with VIF >10)
- **FDR**: Performed FDR control to get significant predictors.

### 3. Model Evaluation

The performance of the logistic regression model was evaluated using various metrics:
- **Accuracy**: Proportion of correctly classified instances.
- **R^2** and **RMSE**

The dataset was split into training and testing sets to validate the model's performance out-of-sample.

### 4. Testing Interactions Between Features

To understand the interactions between different features, a linear regression model was utilized, focusing on:
- **Interaction Terms**: Creating and analyzing interaction terms between categorical (e.g., diagnosis) and continuous variables (e.g., radius_mean, texture_mean).
- **Model Interpretation**: Discussing the implications of these interactions and how they influence the model's predictions.
- **Discusses the issues with using linear model to predict binary outcomes**

### 5. Feature Selection and Cross-Validation

Feature selection was performed to enhance the model's efficiency and interpretability:
- **Reduced Model**: Selecting a subset of significant predictors using methods like FDR.
- **Cross-Validation**: Comparing the performance of the full model (all predictors) with the reduced model using 10-fold cross-validation.
- **Performance Metrics**: Evaluating the out-of-sample performance and determining the optimal model.

## Conclusion

The analysis provides a thorough examination of the Breast Cancer Dataset, from initial data exploration to advanced predictive modeling and feature selection. The logistic regression model, enhanced by careful preprocessing and feature selection, demonstrates robust performance in classifying breast cancer tumors. Additionally, exploring interactions between features offers deeper insights into the underlying data relationships, contributing to more informed medical predictions.

