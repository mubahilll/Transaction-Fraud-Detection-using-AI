# Fraud Detection Model Training and Evaluation

This repository contains a detailed notebook for training and evaluating machine learning models for fraud detection using a financial transactions dataset.

## Table of Contents

- [Introduction](#introduction)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

This project aims to build and evaluate various machine learning models to detect fraudulent transactions in a financial dataset. The dataset is processed and analyzed to handle imbalanced data, followed by training and evaluating multiple classifiers.

## Exploratory Data Analysis
- Generate descriptive statistics and visualize data distributions.
- Check for class imbalance in the target variable isFraud.

## Feature Engineering
- Drop irrelevant columns.
- Create dummy variables for categorical features.
- Normalize the amount column to handle outliers.

## Model Training and Evaluation
The following models were trained and evaluated:

1. Logistic Regression
2. Gaussian Naive Bayes
3. Support Vector Machine
4. Linear Regression
Each model was trained using a balanced dataset created with undersampling and oversampling techniques to handle class imbalance.

## Model Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- AUC-ROC
## Confusion Matrix and ROC Curve
Each model's performance was evaluated using a confusion matrix and ROC curve analysis to understand false positive and false negative rates.

## Results
The results for each model are summarized below:

| Metrics   | Logistic Regression | Support Vector Machine | Naive Bayes | Linear Regression |
|-----------|----------------------|------------------------|-------------|-------------------|
| Accuracy  | 0.987                | 0.982                  | 0.977       | 0.973             |
| Precision | 0.91                 | 0.88                   | 0.85        | 0.82              |
| Recall    | 0.92                 | 0.89                   | 0.87        | 0.83              |
| F1-Score  | 0.915                | 0.885                  | 0.86        | 0.815             |
| AUC-ROC   | 0.987                | 0.982                  | 0.977       | 0.973             |

## Conclusion
The logistic regression model outperformed the other models in terms of accuracy, precision, recall, F1-score, and AUC-ROC. The analysis highlights the importance of handling class imbalance and feature engineering in fraud detection tasks.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

