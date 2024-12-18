# Campaign Performance Prediction

This repository contains the code and analysis for predicting the performance of advertising campaigns using machine learning models. The goal is to build a model that can predict campaign performance based on various features such as impressions, clicks, media cost, and engagement metrics. The project involves extensive data preprocessing, feature engineering, model selection, and evaluation.

## Table of Contents

- [Overview](#overview)
- [Data Preparation](#data-preparation)
- [Feature Engineering](#feature-engineering)
- [Model Selection and Evaluation](#model-selection-and-evaluation)
- [Results](#results)

## Overview

The dataset used for this project contains various attributes related to online advertising campaigns. The objective is to predict the success of these campaigns, measured by metrics such as leads, clicks, cost per lead, and others. The project aims to build a model that balances interpretability and performance, using a combination of logistic regression, Random Forest, and XGBoost models.

## Data Preparation

1. **Data Cleaning**: 
   - Missing values were handled by dropping columns with significant missing data (e.g., **Registrations** and **CPR**).
   - Unnecessary or redundant columns were removed to focus on key features.

2. **Feature Engineering**:
   - New features and calculated metrics, such as CTR (Click-Through Rate), CPC (Cost Per Click), CPR (Cost Per Registration), and CPQV (Cost Per Qualified Visit), were created to better represent the campaign performance.
   - These features helped improve model accuracy and provide better insights into what factors influenced campaign success.

## Feature Engineering

Key engineered features:
- **CTR (Click-Through Rate)**: Measures the ratio of clicks to impressions, indicating the effectiveness of the ad in generating interest.
- **CPC (Cost Per Click)**: Indicates how much was spent per click, helping evaluate the cost efficiency of the campaign.
- **CPR (Cost Per Registration)**: Measures how much was spent for each registration, providing insight into the conversion efficiency of the campaign.
- **CPQV (Cost Per Qualified Visit)**: Represents the cost of each qualified visit to the landing page, helping assess the quality of the leads generated.

## Model Selection and Evaluation

To predict campaign performance, several models were evaluated:
- **Logistic Regression**: Used as a baseline model due to its interpretability.
- **Random Forest**: An ensemble method that provides high performance and is capable of handling complex relationships.
- **XGBoost**: A powerful gradient boosting model that was tuned for optimal performance.

### Model Performance:
- **Logistic Regression**: Provided clear insights into feature importance, offering a better understanding of what drives campaign success.
- **Random Forest and XGBoost**: Achieved better performance metrics (accuracy: 85%, precision: 82%, recall: 80%), demonstrating the power of ensemble models.

### AUC-ROC Score: 0.90, indicating strong model performance.

## Results

The final model, which combines logistic regression for interpretability and ensemble models for predictive power, demonstrated:
- **Accuracy**: 85%
- **Precision**: 82%
- **Recall**: 80%
- **AUC-ROC Score**: 0.90

This model successfully identified the key features that influence campaign performance and provided high predictive accuracy.
