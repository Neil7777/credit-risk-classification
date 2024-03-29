# Credit-Risk-Classification
This repository contains a machine learning project for credit risk classification using a logistic regression model. The goal of this project is to predict whether a loan is "healthy" (0) or "high-risk" (1) based on various financial attributes of borrowers.

## Dataset

The dataset used for this analysis is lending_data.csv, which includes the following columns:

- loan_size: Size of the loan
- interest_rate: Interest rate of the loan
- borrower_income: Income of the borrower
- debt_to_income: Debt-to-income ratio of the borrower
- num_of_accounts: Number of accounts the borrower has
- derogatory_marks: Number of derogatory marks on the borrower's credit report
- total_debt: Total debt of the borrower
- loan_status: Target variable indicating loan status (0 for healthy, 1 for high-risk)

### Process
1. Data Preprocessing:

    - Reading and exploring the dataset
    - Splitting the data into training and testing sets
2. Model Building:

    - Utilizing logistic regression as the primary model
    - Training the logistic regression model on the training data
    - Evaluating the model's performance on the testing data   

### Model Evaluation
The model's performance was evaluated using the following metrics:

- Accuracy: Overall proportion of correctly classified instances
- Precision: Ability of the model not to label as positive a sample that is negative
- Recall: Ability of the model to find all the positive samples
- F1-score: Weighted average of precision and recall
### Results
The logistic regression model achieved the following results:

- Accuracy: 99%
- Precision (0 - Healthy Loan): 1.00
- Recall (0 - Healthy Loan): 0.99
- F1-score (0 - Healthy Loan): 1.00
- Precision (1 - High-Risk Loan): 0.85
- Recall (1 - High-Risk Loan): 0.91
- F1-score (1 - High-Risk Loan): 0.88
### Recommendations
Based on the results, the logistic regression model is recommended for credit risk classification due to its high accuracy and balanced performance in classifying both healthy and high-risk loans.

### Files Included
- lending_data.csv: The dataset used for analysis
- Credit_Risk_Classification.ipynb: Jupyter Notebook containing the Python code for data preprocessing, model building, and evaluation
- README.md: Detailed information about the project, including dataset description, analysis overview, results, and recommendations
- Credit Risk Analysis Report.md : Detailed analysis overview, results, and recommendations.

### Dependencies
The following Python libraries were used for this analysis:

- 'pandas': Data manipulation and analysis
- 'numpy': Mathematical functions
- 'scikit-learn': Machine learning library for logistic regression, metrics, and data preprocessing
- 'matplotlib', 'seaborn': Visualization libraries
### How to Use
1. Clone this repository to your local machine using git clone.
2. Install the required dependencies using pip install -r requirements.txt.
3. Open and run the Credit_Risk_Classification.ipynb notebook in Jupyter or any compatible environment.
4. Follow the notebook's instructions to explore the dataset, preprocess the data, build the logistic regression model, and evaluate its performance.
5. Review the results, metrics, and recommendations provided in the notebook.
### Note
- Ensure you have Python installed on your machine.
- It is recommended to use an environment like Anaconda or virtualenv for managing dependencies.