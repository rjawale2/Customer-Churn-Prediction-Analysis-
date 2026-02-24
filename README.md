# Customer Churn Prediction Analysis

## Project Overview

Customer churn is a critical business problem that directly impacts revenue and customer lifetime value. This project builds and evaluates machine learning models to predict whether a customer is likely to churn based on historical behavioral and demographic data.
The objective is to identify high-risk customers early and support proactive retention strategies.

---

## Business Problem

Customer acquisition is significantly more expensive than customer retention. Accurately predicting churn allows businesses to:

- Reduce revenue loss
- Improve retention campaigns
- Optimize marketing spend
- Increase customer lifetime value

---

## Dataset Description

The dataset contains customer-level information including:

- Demographics
- Account information
- Service usage
- Billing details
- Contract type
- Tenure
- Target variable: `Churn` (Yes/No)

---

## Project Workflow

### 1. Data Preprocessing
- Handled missing values
- Encoded categorical variables
- Scaled numerical features
- Converted target variable to binary

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis
- Correlation analysis
- Churn rate visualization
- Feature importance exploration

### 3. Model Development

The following models were implemented and compared:

- Logistic Regression
- Random Forest
- XGBoost (if used)
- Additional baseline models (if applicable)

### 4. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC Score

---

## Results Summary

The final Random Forest model was selected due to its strong churn detection capability under class imbalance. Using a tuned probability threshold (0.35), the model achieved approximately 72% accuracy while maintaining high churn recall (~0.87), meaning it successfully captures most true churners for proactive retention. Precision is lower, reflecting a deliberate tradeoff to prioritize identifying at-risk customers over minimizing false positives. ROC-AUC (~0.86) indicates strong ranking ability, and PR-based evaluation further supports robustness for imbalanced churn prediction.

Business insight: 

Target retention outreach by risk score (top deciles): Focus offers/calls on the top ~20–35% highest predicted churn probabilities to capture most churners while controlling operational cost.

Contract strategy: If month-to-month contract is a top driver, prioritize incentives to move customers to longer-term contracts.

Price/charge sensitivity: If monthly charges/total charges contribute strongly, test tiered discounts or bundled plans for high-charge segments.

Tenure-based interventions: If churn is highest at low tenure, deploy early-life onboarding programs (first 30–90 days) and proactive support to reduce early churn.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

