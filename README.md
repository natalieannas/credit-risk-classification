# credit-risk-classification

Purpose:
This analysis was used to predict credit risk, whether a loan was high risk or healthy based on financial data from borrowers. 

Financial Data Used and Prediction Target:
The data set we used included the borrowers financial information, including income, debt-to-income, loan amount, number of accounts, and a few other common factors that are looked at when applying for a loan. We looked at all these factors in order to predict if the candidates loan was going to be a 0 (healthy) or 1(high risk) loan.

Variables:
The variables we used for the prediction of the risks of the loan included all the columns of the data set except for loan_status. However, we did run a value_counts analysis of loan_status to see the class distribution. 

Machine Learning Process:
The process that I followed included:
    1. Reading and cleaning the dataset
    2.Seperating the features and the labels
    3.Splitting the data into training and testing sets
    4.Aplying the Logistic Regression model
    5.Making predictions and evaluating the model

Model Used:
LogisticRegression from sklearn.linear_model applied with solver='lbfgs' and random_state=1

Results:
    *Accuracy: 99%
    *Precision(Class 0 - healthy): 1.00
    *Recall (Class 0): 0.99
    *Precision(Class 1 - high risk): 0.85
    *Recall(Class 1): 0.95

Summary:
For this module only Logistic Regression was used, but it did perform really well overall. The model showed great performance in predicting healthy loans and high risk loans. However we did see some healthy loans being misclassified as risky. Meaning the precision wasn't as high as it could have been. I do recommend overall that this is a good model to use for this. It did perform very high accuracy and was fairly balanced throughout it's predictions. 

