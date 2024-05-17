# Credit Risk Classification
## Machine Learning: Logical Regression Model, Confusion Matrix, and Classification Report

<img width="575" alt="image" src="https://github.com/Colex317/credit_risk_classification/assets/148498483/5f1382a1-a67f-40e5-8ab4-760e22f77756">

_______________________________________________________________________________________________________________________________________________

The Credit Risk Classification assignment focused on using the Logical Regression Model, Confusion Matrix, and Classification Report in supervised machine learning. Python and supervised learning were used to train and evaluate a model based on loan risk. A dataset of historical lending activity from a peer-to-peer lending services company was used to build a model that identified the creditworthiness of borrowers.

# Files Included
- [Credit_Risk](https://github.com/Colex317/credit_risk_classification/tree/main/Credit_Risk): Contains the [credit_risk_classification.ipynb](https://github.com/Colex317/credit_risk_classification/blob/main/Credit_Risk/credit_risk_classification.ipynb) (Python file) and the [lending_data_csv](https://github.com/Colex317/credit_risk_classification/blob/main/Credit_Risk/lending_data.csv).
  
- [Report_template](https://github.com/Colex317/credit_risk_classification/blob/main/report-template.md): Contains the description of the analysis.

# Steps
1. Split the Data into Training and Testing Sets
    - Read the `lending_data.csv` data from the `Resources` folder into a Pandas DataFrame.
      
    - Create the labels set (`y`)  from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.
      
    - Split the data into training and testing datasets by using `train_test_split`.


    -------------------------------------------------------------------------------------------------------------------------------------
2. Create a Logistic Regression Model with the Original Data
   - Fit a logistic regression model by using the training data (`X_train` and `y_train`).
      
    - Save the predictions on the testing data labels by using the testing feature data (`X_test`) and the fitted model.
      
    - Evaluate the model’s performance by doing the following: 

**Generate a confusion matrix**
<img width="550" alt="image" src="https://github.com/Colex317/credit_risk_classification/assets/148498483/6019de52-b8fc-4175-85b1-0693db290193">

**Print the classification report**
<img width="550" alt="image" src="https://github.com/Colex317/credit_risk_classification/assets/148498483/a0720bec-a1cd-4154-8a57-bdc1b63cb3b9">


# Credit Risk Analysis Report
An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.
