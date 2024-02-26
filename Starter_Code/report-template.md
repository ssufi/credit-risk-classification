# Module 12 Report Template

## Overview of the Analysis

Throughout this analysis, the objective was to develop machine learning models aimed at classifying credit risk by leveraging past lending activity data. The aim was to forecast the creditworthiness of borrowers by considering a range of financial characteristics.

## Data Overview
The dataset included information on peer-to-peer lending, with a focus on predicting loan status (0 for healthy loans and 1 for high-risk loans). Key variables: loan_status, feature1, feature2, ... (additional features). The target variable (loan_status) had imbalanced classes, with a majority of loans being healthy.




## Machine Learning Process:

Data Splitting: The dataset was divided into training and testing subsets. Model 1 - Logistic Regression (Original Dataset):

A Logistic Regression model was trained using the original dataset. Evaluation metrics such as Accuracy, Precision, and Recall were computed. Model 2 - Logistic Regression (Oversampled Dataset):

To address class imbalance, the original dataset underwent oversampling using RandomOverSampler. A Logistic Regression model was then trained using the oversampled dataset. Evaluation metrics including Balanced Accuracy, Precision, and Recall were analyzed.


## Results
* Model 1 - Logistic Regression (Original Data):

  * Accuracy: 0.99
  * Precision (Label 0): 1.00
  * Recall (Label 0): 0.99
  *  (Label 1): 0.85
  * Recall (Label 1): 0.91

* Model 2 - Logistic Regression (Oversampled Data):

  * Balanced Accuracy: 0.994
  * Precision (Label 0): 1.00
  * Recall (Label 0): 0.99
  * Precision (Label 1): 0.84
  * Recall (Label 1): 0.99


## Summary

The logistic regression model trained on the oversampled dataset (Model 2) demonstrates superior performance compared to the original model across multiple metrics, especially in addressing high-risk loans (label 1). Through oversampling, enhancements are observed in balanced accuracy, precision, and recall for both labels.

## Recommendation:

It is advisable for the company to adopt Model 2, which involves Logistic Regression with oversampled data. The advancements observed in various metrics, particularly in managing high-risk loans, signify improved predictive prowess. The effectiveness of a model depends on the specific problem at hand, and in this scenario, accurately identifying high-risk loans (1) is paramount. Model 2 demonstrates excellence in this regard, making it the preferred choice.
