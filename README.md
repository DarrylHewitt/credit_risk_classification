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

## Create a Logistic Regression Model with the Original Data

- Fit a logistic regression model using the training data (X_train and y_train).
- Save predictions for the testing data labels using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance:
  - Generate a confusion matrix.
  - Print the classification report.

### Model Performance

- Accuracy Score: [Provide the accuracy score]
- Precision Score: [Provide the precision score]
- Recall Score: [Provide the recall score]

**Question:** How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

[Answer the question here]

## Credit Risk Analysis Report

### An Overview of the Analysis

Explain the purpose of this analysis, emphasizing the goal of predicting creditworthiness using machine learning.

### Results

- **Accuracy Score:** [Provide insights into the accuracy]
- **Precision Score:** [Provide insights into the precision]
- **Recall Score:** [Provide insights into the recall]

### Summary

Summarize the results obtained from the machine learning model. Provide justification for recommending or not recommending the model for use by the company.

If you don’t recommend the model, justify your reasoning.

## Conclusion

Include any concluding remarks, future considerations, or potential improvements for the model.

