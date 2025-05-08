# credit-risk-classification.

## Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Overview of the Analysis

The purpose of this analysis was to evaluate the risk level of loans using a machine learning classification model. Specifically, the goal was to predict whether a loan would be “healthy” or “high risk” based on several financial features provided in the dataset.

Financial Information & Prediction Target:
The dataset contained financial data related to loan applicants, such as income, debt-to-income ratio, and number of accounts. The target variable (loan_status) was a binary classification: 0 for high-risk loans and 1 for healthy loans.

Value Counts of Target Variable:
The loan_status field was split between two classes. A value_counts() would typically show the distribution of 1s and 0s, which is important for understanding any class imbalance (though this wasn't printed in the notebook).

Stages of the Machine Learning Process:

Data Preparation: The target (y) and feature variables (X) were separated.

Train-Test Split: The data was split into training and testing sets using train_test_split with a random_state of 1.

Model Selection: Logistic Regression was chosen as the classification model.

Model Training: The model was trained on the training set.

Model Evaluation: Predictions were made on the test set, and a confusion matrix and classification report were generated to evaluate performance.

Algorithm Used:
The algorithm used in this challenge was Logistic Regression, a common method for binary classification tasks.

Results
Machine Learning Model 1: Logistic Regression

Accuracy: 0.95

Precision:

Class 0 (high risk): 0.85

Class 1 (healthy): 0.96

Recall:

Class 0 (high risk): 0.68

Class 1 (healthy): 0.99

## Summary
Best Performing Model:
Since only one model was used (Logistic Regression), it is the default choice for recommendation. It shows high accuracy and strong performance in predicting healthy loans (class 1) with a recall of 0.99, which means it rarely misses a healthy loan.

Performance Consideration:
The model performs better at predicting healthy loans than high-risk loans, as evidenced by the lower recall (0.68) for class 0. This suggests that the model may not be as effective at flagging risky loans, which could be a concern if the goal is to minimize financial loss by catching high-risk cases.

## Recommendation:
Logistic Regression can be used if the goal is to maximize the identification of healthy loans. However, if identifying high-risk loans is more critical, it may be necessary to try other models or improve class balance techniques (e.g., SMOTE or reweighting).
