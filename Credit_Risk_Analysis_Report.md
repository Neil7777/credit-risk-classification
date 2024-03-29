# Credit Risk Analysis Report

## Overview of the Analysis
### Purpose of the Analysis
The purpose of this analysis was to develop machine learning models to predict credit risk for loans based on financial information of borrowers. The goal was to create models that could accurately classify loans into "healthy" (0) and "high-risk" (1) categories, providing valuable insights for loan approval processes.
### Financial Information and Prediction
The dataset contained financial data such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. The target variable we aimed to predict was the "loan_status" column, which had two classes: 0 for healthy loans and 1 for high-risk loans.
### Basic Information about Variables
To understand the distribution of the target variable:

- loan_status value_counts:
	- 0 (Healthy Loan): 18,765
	- 1 (High-Risk Loan): 619
### Stages of Machine Learning Process
1. Data Preprocessing:

    - Reading and exploring the dataset.
    - Splitting the data into training and testing sets.
2. Model Building:

	- Utilizing logistic regression as the primary model due to its interpretability and suitability for binary classification tasks.
	- Training the logistic regression model on the training data.
	- Evaluating the model's performance on the testing data.
### Methods Used
Logistic Regression: Used for its simplicity, interpretability, and effectiveness in binary classification tasks.


## Results


* Machine Learning Model 1:
    
    Classification Report:
    - Accuracy: 0.99
	- Precision (0 - Healthy Loan): 1.00
	- Recall (0 - Healthy Loan): 0.99
	- F1-score (0 - Healthy Loan): 1.00
	- Precision (1 - High-Risk Loan): 0.85
	- Recall (1 - High-Risk Loan): 0.91
	- F1-score (1 - High-Risk Loan): 0.88


## Summary
### Model Performance
- The logistic regression model achieved excellent results with an overall accuracy of 99%.
- For healthy loans (label 0), the model showed perfect precision (1.00) and high recall (0.99).
- High-risk loans (label 1) were also predicted well with a precision of 0.85 and recall of 0.91.
### Recommendation
Based on the results, the logistic regression model seems to perform best for this credit risk classification task. It effectively distinguishes between healthy and high-risk loans with high accuracy and balanced precision-recall scores for both classes.
### Performance Considerations
- Performance depends on the problem we are trying to solve:
	- Predicting healthy loans (label 0) is crucial for minimizing the risk of approving high-risk loans as healthy.
	- Predicting high-risk loans (label 1) is also important to identify loans that need closer scrutiny.
### Conclusion
The logistic regression model is recommended for predicting credit risk due to its high accuracy and balanced performance in classifying both healthy and high-risk loans. It provides a reliable tool for financial institutions to assess loan applications and make informed decisions.