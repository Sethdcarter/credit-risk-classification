# credit-risk-classification

## Overview of the Analysis

This analysis aims to predict whether a loan applicant will default on their loan using machine learning techniques.

The dataset includes the following financial attributes:

Loan Size: The amount borrowed by the customer.
Interest Rate: The percentage of interest applied to the loan.
Borrower Income: The total annual income of the borrower.
Debt-to-Income Ratio: The proportion of the borrower's debt relative to their income.
Number of Accounts: The total number of financial accounts the borrower holds.
Derogatory Marks: Any negative credit events associated with the borrower.
Total Debt: The total amount of outstanding debt.

The objective of this analysis was to predict loan status, specifically whether a borrower is likely to default (1) or not default (0) on their loan.


Tried to predict the creditworthiness of borrowers by looking at default rates.

##Stages of the Machine Learning Process

*Data Loading & Exploration
    Imported the dataset from a CSV file.
    Reviewed the dataset’s structure and identified key financial variables.

*Data Preprocessing
    Separated the dataset into features (X) and target variable (y).
    Split the data into training (80%) and testing (20%) sets.

*Model Selection & Training
    Selected Logistic Regression as the classification model.
    Trained the model using the training data.

*Model Evaluation
    Generated predictions using the test dataset.
    Evaluated model performance using a confusion matrix and classification report.

*Interpretation of Results
    Analyzed precision, recall, and accuracy scores.
    Noted the dataset's imbalance and assessed the model’s effectiveness in predicting loan defaults.

*Final Recommendation
    Summarized model performance and provided a recommendation for its use in loan risk assessment.

##Methods Used
    Logistic Regression (LogisticRegression from sklearn): Chosen for its effectiveness in binary classification problems like predicting loan defaults.
    Train-Test Split (train_test_split from sklearn): Used to divide the dataset into training and testing sets to evaluate model performance.
    Confusion Matrix (confusion_matrix from sklearn): Applied to assess the true positives, true negatives, false positives, and false negatives.
    Classification Report (classification_report from sklearn): Provided detailed precision, recall, and F1-score metrics to evaluate model effectiveness.

## Results

* Logistic Regression Model
    * Accuracy Score: 99%
    * Precision Score:
        Class 0 (Not Defaulted): 1.00
        Class 1 (Defaulted): 0.86
    * Recall Score:
        Class 0: 1.00
        Class 1: 0.91
    * F1-Score:
        Class 0: 1.00
        Class 1: 0.88

## Summary

The Logistic Regression model performed well, achieving an accuracy of 99%. It is  strong in predicting non-defaulting loans (Class 0) with perfect precision and recall. However, for defaulting loans (Class 1), while recall is high (91%), precision is slightly lower (86%), meaning there are some false positives.

Given the high scores, this model is effective for predicting loan defaults. However, if false positives are a concern, further tuning or alternative models could be considered. For most business applications, this model is suitable for use in assessing loan risks.
