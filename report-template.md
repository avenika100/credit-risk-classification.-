# Module 12 Analysis Report 

## Overview of the Analysis
The purpose of this analysis was to build and evaluate machine learning models that can predict the loan status of applicants — whether they are a high-risk or low-risk borrower. This type of prediction is critical for financial institutions to minimize losses and maximize profitable lending decisions.

The dataset included financial features such as loan amount, interest rate, borrower income, debt-to-income ratio, and more.
The main objective was to predict the loan_status label, where:

0 = Low risk

1 = High risk

Basic information about the target variable (loan_status):
-     loan_status.value_counts()

Sample distribution:

   * Low Risk (0): Majority

   * High Risk (1): Minority

This suggests an imbalanced classification problem, which can impact model performance.

The machine learning process included:

Loading and inspecting the dataset.

Splitting the data into features (X) and target labels (y).

Dividing the data into training and testing sets.

Training two models:

Logistic Regression

Random Forest Classifier

Evaluating the models using confusion matrices and classification reports.



## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
