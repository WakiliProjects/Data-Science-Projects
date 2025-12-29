📌 Project Overview

This project explores fraud detection using transactional data, with the aim of identifying behavioural patterns associated with fraudulent activity. The analysis focuses on understanding class imbalance, engineering meaningful features, and applying statistical modelling techniques to distinguish fraudulent from legitimate transactions.

The workflow follows a structured data science process:

- Data preprocessing and feature engineering (Python)

- Exploratory data analysis and class imbalance assessment

- Classification modelling (Logistic Regression & Decision Trees)

- Interpretation of results

- fraud-detection-analysis/
│
├── data/
│   └── cleaned_data.csv
│
├── notebooks/
│   └── fraud_detection_analysis.ipynb
│
├── README.md

🧠 Dataset Description

The dataset consists of transaction-level financial records, including:

Transaction type

Transaction amount

Sender and recipient account balances (before and after transactions)

Fraud labels indicating fraudulent activity

The data simulates real-world mobile money transactions and presents a highly imbalanced classification problem, where fraudulent transactions represent a small minority of observations.

🔧 Data Preprocessing & Feature Engineering

Data preprocessing was performed in Python to ensure data quality and analytical relevance. The following steps were applied:

✔ Data Cleaning

Removed non-informative identifier variables (step, nameOrig, nameDest, isFlaggedFraud)

Verified data types and missing values

✔ Feature Engineering

New variables were created to capture transactional behaviour:

deltaOrig – change in the sender’s account balance

deltaDest – change in the recipient’s account balance

log_amount – logarithmic transformation of transaction amount to reduce skewness

✔ Feature Selection

Only variables relevant to fraud classification were retained:

type

log_amount

deltaOrig

deltaDest

isFraud

The cleaned dataset was then exported for modelling.

📊 Exploratory Data Analysis

Exploratory analysis revealed a strong class imbalance, with fraudulent transactions representing a small fraction of the dataset. Cross-tabulation of transaction type and fraud status showed that fraudulent activity occurs almost exclusively within TRANSFER and CASH_OUT transaction types.

This insight guided model selection and feature focus during the modelling stage.

🤖 Modelling Approach

Two classification approaches were used:

1. Logistic Regression

Provides interpretable coefficients

Suitable for understanding the impact of explanatory variables

2. Decision Tree Classifier

Captures non-linear relationships

Handles interactions between features effectively

These models were evaluated to compare predictive performance and interpretability.

📈 Key Insights

Fraud is highly concentrated in specific transaction types

Balance change features are strong indicators of fraudulent behaviour

Log-transforming transaction amounts improves model stability

Class imbalance must be considered when evaluating performance

🧰 Tools & Technologies

- Python (Pandas, NumPy)

- R (for modelling and statistical evaluation)

- Jupyter Notebook

- R Markdown

- GitHub

📌 Future Improvements

Address class imbalance using resampling techniques (e.g., SMOTE)

Compare additional machine learning models (Random Forest, XGBoost)

Perform model evaluation using ROC-AUC and precision-recall metrics

Deploy model as a simple prediction API
