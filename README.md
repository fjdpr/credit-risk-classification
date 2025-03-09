# Credit Risk Analysis

## Summary
This project involves the analysis and prediction of credit risk using various machine learning models. The goal is to identify high-risk loans that may have a significant probability of default.

## Objectives
- Use Logistic Regression to predict credit risk.
- Use Decision Tree Classifier to predict credit risk.
- Use Random Forest Classifier to predict credit risk.
- Compare the performance of different models.
- Visualize the evaluation metrics of the models.

## Data Description
The dataset includes:
- **Credit Information**: CSV data for various loans, including features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status.

## Included Scripts
1. **Credit_Risk_Analysis.ipynb**:
   - Loads and preprocesses the data.
   - Uses StandardScaler to normalize the data.
   - Applies Logistic Regression, Decision Tree, and Random Forest models to the data.
   - Evaluates the performance of each model.
   - Visualizes the evaluation metrics using confusion matrices and classification reports.

## Requirements
- pandas
- scikit-learn

## Instructions

### Getting Started
1. **Ensure you have the required libraries installed**:
   ```bash
   pip install pandas scikit-learn
   ```
2. **Open `Credit_Risk_Analysis.ipynb` in Jupyter Notebook or JupyterLab**.

### Features
- **Data Normalization:** Normalize the credit information data using StandardScaler.
- **Logistic Regression:** Apply Logistic Regression to predict credit risk.
- **Decision Tree Classifier:** Apply Decision Tree Classifier to predict credit risk.
- **Random Forest Classifier:** Apply Random Forest Classifier to predict credit risk.
- **Evaluation Metrics:** Evaluate the models using confusion matrices and classification reports.
- **Model Comparison:** Compare the performance of different models.

### Deployment
The Jupyter Notebook can be run locally on your machine. Ensure you have Jupyter Notebook or JupyterLab installed.

### Contributions
We welcome and appreciate contributions from the community. If you have suggestions or improvements, please open an issue or submit a pull request.

### License
This project is licensed under the MIT License. See the LICENSE file for details.
