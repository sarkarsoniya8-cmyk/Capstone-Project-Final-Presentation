# Customer Churn Prediction — Data Science Capstone Project

## Project Overview
This capstone project analyzes customer subscription data to predict whether a customer will leave (churn) the service. By identifying high-risk customers early, businesses can take proactive retention steps.

## Project Workflow
1. **Data Cleaning & Preprocessing:** Verified zero missing values, removed non-predictive identifier columns (`CustomerID`), and used `LabelEncoder` to convert categorical columns (`Contract_Type`, `Tech_Support`, `Payment_Method`, `Churn`) into numeric values.
2. **Exploratory Data Analysis (EDA):** Visualized churn rates across contract types and customer tenure. Discovered that customers on Month-to-Month contracts and those in their first 12 months have the highest churn risk.
3. **Model Building & Evaluation:** Split the dataset into 80% training and 20% testing sets. Trained and evaluated three standard classification models: Logistic Regression, Decision Tree, and Random Forest.

## Model Performance Summary

| Model | Accuracy (%) | Precision (%) | Recall (%) | F1-Score (%) |
| :--- | :---: | :---: | :---: | :---: |
| Logistic Regression | 87.0 | 83.82 | 79.17 | 81.43 |
| Decision Tree | 90.5 | 87.32 | 86.11 | 86.71 |
| Random Forest | 89.0 | 87.88 | 80.56 | 84.06 |

## Key Business Recommendations
* **Incentivize Annual Contracts:** Offer a 10–15% discount for Month-to-Month customers to upgrade to a 1-Year contract.
* **First-Year Onboarding Support:** Provide complimentary Tech Support for new customers during their first 6–12 months to reduce early churn.

## Files Included in This Repository
* `customer_churn_capstone.ipynb` — Complete Jupyter/Colab Notebook with Python code
* `customer_churn_data.csv` — Dataset (1,000 customer records, 7 features)
* `model_performance_summary.csv` — Evaluation metrics table for all trained models
* `Capstone_Project_Report.pdf` — Detailed PDF project report
* `churn_by_contract.png` & `churn_by_tenure.png` — EDA visualizations
