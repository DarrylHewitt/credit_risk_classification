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

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

### Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * 
- **Accuracy Score:** [Provide insights into the accuracy]
- **Precision Score:** [Provide insights into the precision]
- **Recall Score:** [Provide insights into the recall]

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

- **Accuracy Score:** [Provide insights into the accuracy]
- **Precision Score:** [Provide insights into the precision]
- **Recall Score:** [Provide insights into the recall]

### Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you don’t recommend the model, justify your reasoning.

## Conclusion

Include any concluding remarks, future considerations, or potential improvements for the model.

