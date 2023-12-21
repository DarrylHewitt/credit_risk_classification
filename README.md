# Credit Risk Classification

## Overview

This project focuses on building a machine learning model to assess the creditworthiness of borrowers using historical lending activity data from a peer-to-peer lending services company. The goal is to create a logistic regression model capable of predicting whether a loan is healthy (0) or has a high risk of defaulting (1).

## Project Structure

The project repository is organized as follows:

- **credit-risk-classification**
  - **Credit_Risk**
    - `credit_risk_classification.ipynb` (Jupyter Notebook containing code)
    - `lending_data.csv` (Dataset used for analysis)
  - `README.md` (This file)

## Split the Data into Training and Testing Sets

- Read the `lending_data.csv` data into a Pandas DataFrame.
- Create labels set (y) from the “loan_status” column.
- Create features set (X) DataFrame from the remaining columns.
- Split the data into training and testing datasets using `train_test_split`.

## Create a Logistic Regression Model with both the Original and Resampled Data

- Fit a logistic regression model using the training data (X_train and y_train).
- Save predictions for the testing data labels using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance:
  - Generate a confusion matrix.
  - Print the classification report.

## Credit Risk Analysis Report

### An Overview of the Analysis

The objective of this analysis is to employ different methods to develop and assess a model for predicting loan risk. The task involves utilizing a dataset containing past lending transactions from a peer-to-peer lending services company. The goal is to create a model capable of determining the healthiness of a loan based on historical lending activity.

The financial data includes: 

* loan_size: The amount of the loan requested by the borrower.
* interest_rate: The interest rate associated with the loan.
* borrower_income: The income of the borrower.
* debt_to_income: The ratio of the borrower's debt to their income.
* num_of_accounts: The number of accounts the borrower has.
* derogatory_marks: The number of derogatory marks on the borrower's credit history.
* total_debt: The total debt of the borrower.
* loan_status: Indicates the status of the loan (i.e. Whether it is healthy or not).

The dataset was separated into labels and features and the data dplit into training and testing sets. A logistic regression model was instantiated and fit to the training data before predictions were made on the testing data. 

A balanced accuracy score was created and a confusion matrix produced to evaluate the model performance. Finally, a classification report was generated which included precision, accuracy and an F1-score. 

All of the above was then repeated on another logistic regression model after random oversampling was applied to balance the class distribution in the training data.

### Results

Results are broken down into accuracy, precision and recall as produced in the classification report mentioned above. 

**Accurary** is understood as the proportion of correctly predicted instances (both true positives and true negatives) out of the total instances.
**Precision** is the ratio of correctly predicted positive observations to the total predicted positives.
**Recall** (Sensitivity or True Positive Rate) is the ratio of correctly predicted positive observations to the all observations in the actual class.

* Machine Learning Model 1 (original data):

- **Accuracy Score:**

The overall accuracy of the model is 99%, which is the proportion of correctly predicted instances (both true positives and true negatives) out of the total instances.

- **Precision Score:**

For class 0: Precision is 1.00, indicating that all predicted positive instances for class 0 were correct.
For class 1: Precision is 0.87, meaning that 87% of the predicted positive instances for class 1 were correct.

- **Recall Score:**

For class 0: Recall is 1.00, indicating that the model correctly identified all actual instances of class 0.
For class 1: Recall is 0.89, meaning that the model captured 89% of the actual instances of class 1.


* Machine Learning Model 2 (resampled data):

- **Accuracy Score:**

The overall accuracy of the model is 100%, suggesting that all instances were correctly classified.

- **Precision Score:**

For class 0: Precision is 1.00, indicating that all predicted positive instances for class 0 were correct.
For class 1: Precision is 0.87, meaning that 87% of the predicted positive instances for class 1 were correct.

- **Recall Score:**

For class 0: Recall is 1.00, indicating that the model correctly identified all actual instances of class 0.
For class 1: Recall is also 1.00, suggesting that the model captured all actual instances of class 1.

### Summary

Both models have a very high accuracy. The first model has an accuracy of 99%, while the second model has an accuracy of 100%. Based on overall accuracy alone, the second model appears to perform slightly better.

The F1-score provides a balance between precision and recall. While both models have high F1-scores, the second model has a higher F1-score for class 1 (0.93) compared to the first model (0.88). This indicates better performance in capturing true positives for class 1 in the second model.

The second model has perfect precision and recall for class 0, indicating that it correctly identifies all instances of class 0 without any false positives or false negatives. The first model, while also performing well, has a slightly lower recall for class 0 (0.99).

Considering these factors, the second model appears to perform slightly better overall, especially in terms of F1-score and precision-recall balance. 

It's also worth noting that it's more important to predict the 1's, further justifying the use of Model 2 over Model 1.


