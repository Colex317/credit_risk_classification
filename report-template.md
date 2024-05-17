# Credit Risk Analysis Report

## Overview of the Analysis

Description of the analysis completed for the machine learning models used in this Challenge. 

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

**Basic Information About the Variables**
To understand the distribution of the target variable (Loan Status), we examined its value counts:
<img width="500" alt="image" src="https://github.com/Colex317/credit_risk_classification/assets/148498483/0babce1f-d9fd-4ce2-ae1b-495475836ce4">


The dataset provides 77 536 loan statuses. Ninety-six (75 036) percent of the loans were in the healthy (0) category, and the remainder of 2 500 have a high risk of default (1).

**Stages of the Machine Learning Process**
The analysis was conducted through several stages, which are essential in the development of an effective machine-learning model:
Since the dataset was already preprocessed (cleaned, categorical variables encoded, and numerical features standardized). The process started with data splitting.

1. Data Splitting
   - Separation of labels and features: The data was divided into labels (y) from the loan status column and features (X) from the remaining columns.
   - Training and Testing Sets: The dataset was split into training and testing sets to evaluate the model's performance.

2. Model Training
    - Logistic Regression: This algorithm is often chosen for its simplicity and effectiveness in binary classification problems.

3. Model Evaluation
      - Confusion Matrix: Used to evaluate the performance of the classification model in terms of true positives, true negatives, false positives, and false negatives.
      - Classification Report: Provided precision, recall, F1-score, and support for each class to understand the model's performance comprehensively.

**Methods Used**
*Logical Regression* 
Was the primary algorithm used due to its interpretability and efficiency in handling binary classification tasks. Logistic regression estimates the probability of an event occurring, such as healthy and unhealthy loans, based on a given data set of independent variables.

*Confusion Matrix* 
Aids in visualizing the performance of the classification model by showing the number of accurate and inaccurate instances based on the model’s predictions.
<img width="500" alt="image" src="https://github.com/Colex317/credit_risk_classification/assets/148498483/2a51f0c3-1b24-4d8e-b7f8-567d19c3f65e">


True Positive: 18679 - the number of correct predictions for the positive class.
True Negative: 558 - the actual negative class instances accurately predicted as negative.

*Classification Report*
This report provided detailed metrics, including precision, recall, and F1-score, offering insights into the model's performance for each class.


## Results

<img width="500" alt="image" src="https://github.com/Colex317/credit_risk_classification/assets/148498483/e7a189ae-2445-4cd7-9e57-e345a98fb060">

- **Accuracy** is the overall proportion of correct predictions (both true positives and true negatives) out of all predictions made. 
      - An accuracy of 0.99 means 99% of the total predictions made by the model are correct.
  
- **Precision** measures the percentage of correct positive predictions relative to total positive predictions.
      - For class 0, precision is 1.00, meaning every instance predicted as class 0 is actually class 0.
      - For class 1, precision is 0.87, meaning 87% of the instances predicted as class 1 are actually class 1.

- **Recall** measures the percentage of correct positive predictions relative to total actual positives.
      - For class 0, recall is 1.00, meaning all actual instances of class 0 were correctly identified.
      - For class 1, recall is 0.89, meaning 89% of the actual class 1 instances were correctly identified.


## Summary
The logistic regression model appears to perform very well overall, with an accuracy of 99%. The model achieves perfect precision, recall, and F1-score for the majority class (class 0), and performs reasonably well for the minority class (class 1) with precision at 0.87 and recall at 0.89.

The importance of model performance depends on the specific problem and business requirements. In the context of credit risk classification, the implications of misclassifying borrowers can be significant.The model’s recall for class 1 (0.89) indicates that it correctly identifies 89% of the actual high risk of defaults, which is relatively high and desirable. The precision for class 1 (0.87) shows that 87% of the predicted high-risk of defaults are actual defaults, indicating good precision.

Based on the results, I recommend using the current logistic regression model. The model achieves high overall accuracy and performs well in identifying both healthy loans and loans at high risk of default.
The high recall for class 1 ensures that most high-risk defaults are correctly identified, which is crucial for risk management.

In conclusion, the logistic regression model is recommended for its strong performance and balance between identifying healthy and high-risk default loans, which are essential for effective credit risk management.


# References
Geekforgeeks (n.d.). Confusion Matrix in Machine Learning. Retrieved from https://www.geeksforgeeks.org/confusion-matrix-machine-learning/

IBM (n.d.). What is logistic regression? Retrieved from https://www.ibm.com/topics/logistic-regression

Statology (2022). How to Interpret the Classification Report in sklearn. Retrieved from https://www.statology.org/sklearn-classification-report/
