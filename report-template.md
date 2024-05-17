# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

**Purpose of the Analysis**
The primary objective of this analysis is to develop and evaluate a machine learning model that can accurately predict borrowers' creditworthiness. This model aims to classify borrowers into risk categories, thereby aiding the peer-to-peer lending services company in making informed lending decisions and minimizing the risk of loan defaults.

**Financial Information and Prediction Objective**
The dataset used in this analysis consists of historical lending data from a peer-to-peer lending platform. The financial information in the dataset includes the following variables:

   - Loan Size: The amount of money requested by the borrower.
   - Interest Rate: The interest rate assigned to the loan.
   - Borrower Income: The annual income of the borrower.
   - Debt-to-Income Ratio: A ratio comparing the borrower’s total monthly debt payments to their gross monthly income.
   - Number of Accounts: The number of credit accounts held by the borrower.
   - Derogatory Marks: The number of derogatory marks on the borrower’s credit report.
   - Total Debt: The total amount of debt the borrower owes.

The target variable (label) we need to predict is Loan Status, which indicates whether the loan is healthy or has a high risk of default.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
