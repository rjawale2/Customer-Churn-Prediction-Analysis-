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

- Best performing model: *(update with your best model)*
- ROC-AUC Score: *(add value)*
- Key churn drivers identified: *(add 2–3 features)*

Business insight: Customers with shorter tenure and month-to-month contracts show significantly higher churn probability.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost (if used)

---

## Repository Structure
