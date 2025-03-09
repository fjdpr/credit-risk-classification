# Module 12 Report Template

## Overview of the Analysis

**Purpose of the Analysis:**  
The purpose of this analysis is to develop a machine learning model to predict credit risk. Specifically, we aim to identify high-risk loans that may have a significant probability of default.

**Financial Information:**  
The financial data focuses on credit information from customers. The target variable we need to predict is `loan_status`, where a value of 0 indicates a healthy loan and a value of 1 indicates a high-risk loan.

**Basic Information about Variables:**
- `loan_size`: Loan amount
- `interest_rate`: Interest rate
- `borrower_income`: Borrower income
- `debt_to_income`: Debt-to-income ratio
- `num_of_accounts`: Number of accounts
- `derogatory_marks`: Number of derogatory public records
- `total_debt`: Total debt
- `loan_status`: Loan status (0: healthy loan, 1: high-risk loan)

**Machine Learning Process:**
1. **Data Reading:** The data was read from the CSV file `lending_data.csv` into a Pandas DataFrame.
2. **Data Preparation:** The data was separated into labels (`y`) and features (`x`). The data was split into training and testing sets.
3. **Feature Scaling:** The features were standardized using `StandardScaler`.
4. **Models Used:** 
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier
5. **Model Evaluation:** Predictions were made, and the model performance was evaluated using confusion matrices and classification reports.

**Methods Used:**
- `LogisticRegression` from `sklearn`
- `DecisionTreeClassifier` from `sklearn`
- `RandomForestClassifier` from `sklearn`
- `StandardScaler` from `sklearn`
- `train_test_split` from `sklearn`

## Results

**Machine Learning Model 1: Logistic Regression**
- **Accuracy:** 0.99
- **Precision:**
  - Healthy loan (0): 1.00
  - High-risk loan (1): 0.84
- **Recall:**
  - Healthy loan (0): 0.99
  - High-risk loan (1): 0.99
- **F1-Score:**
  - Healthy loan (0): 1.00
  - High-risk loan (1): 0.91
- **Support:**
  - Healthy loan (0): 18765
  - High-risk loan (1): 619

**Machine Learning Model 2: Decision Tree Classifier**
- **Accuracy:** 0.99
- **Precision:**
  - Healthy loan (0): 1.00
  - High-risk loan (1): 0.84
- **Recall:**
  - Healthy loan (0): 0.99
  - High-risk loan (1): 0.85
- **F1-Score:**
  - Healthy loan (0): 0.99
  - High-risk loan (1): 0.85
- **Support:**
  - Healthy loan (0): 18765
  - High-risk loan (1): 619

**Machine Learning Model 3: Random Forest Classifier**
- **Accuracy:** 0.99
- **Precision:**
  - Healthy loan (0): 1.00
  - High-risk loan (1): 0.85
- **Recall:**
  - Healthy loan (0): 0.99
  - High-risk loan (1): 0.89
- **F1-Score:**
  - Healthy loan (0): 1.00
  - High-risk loan (1): 0.87
- **Support:**
  - Healthy loan (0): 18765
  - High-risk loan (1): 619

## Summary

**Which Model Performs Best:**  
The logistic regression model showed excellent performance, with high precision and accuracy in predicting both healthy loans and high-risk loans. The random forest model also performed very well, with slightly higher precision and recall for high-risk loans. The decision tree model had lower precision and recall for high-risk loans compared to the logistic regression and random forest models.

**Recommended Model:**  
We recommend using the random forest model to predict credit risk due to its higher performance and accuracy in identifying high-risk loans.

**Considerations:**  
- It is crucial for the company to accurately predict `1` to manage and mitigate financial risk effectively.
- Continuously improving the model through parameter adjustments and exploring other algorithms can be beneficial.
