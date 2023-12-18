# Credit Card Fraud Detection

## Overview

This Jupyter Notebook focuses on predicting credit card fraud using an anonymized dataset. The goal is to develop models that can effectively identify fraudulent transactions while minimizing false negatives. The analysis includes data exploration, scaling, and the training and evaluation of multiple models, such as logistic regression, naive Bayes, and XGBoost. The final model is a stacking classifier, combining the strengths of multiple models.

## Data Source

The dataset used in this analysis is sourced from Kaggle: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). Please note that the data file included in this repository is only a subset.

## Notebook Content
1. **Loading and Checking Data:** Load the dataset and perform a meticulous check for missing values.
2. **Displaying Dataset Information:** Showcase the structure and descriptive statistics of the dataset for comprehensive understanding.
3. **Data Exploration - Violin Plot:** Utilize a violin plot to visually inspect the distribution of variables, excluding "Class," "Time," and "Amount."
4. **Data Scaling:** Employ StandardScaler to scale feature variables and subsequently split the data into training and testing sets.
5. **Logistic Regression Model:** Train a logistic regression model on the scaled training data and evaluate its performance.
6. **Bernoulli Naive Bayes Model:** Train a Bernoulli Naive Bayes model on the scaled training data and evaluate its performance.
7. **XGBoost Model with Hyperparameter Tuning:** Train an XGBoost classifier with hyperparameter tuning using RandomizedSearchCV.
8. **Stacking Classifier:** Construct a Stacking Classifier using logistic regression, naive Bayes, and XGBoost as base estimators, with XGBoost as the final estimator.
9. **Conclusion:** Evaluate the performance of the final stacked model.

## Model Performance
The final stacked model exhibits the following metrics:

- True Positive (TP): 308
- True Negative (TN): 213200
- False Positive (FP): 74
- False Negative (FN): 24
- Accuracy: 99.95%
- Precision: 80.63%
- Recall: 92.77%
- F1 Score: 86.27%
