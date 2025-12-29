# 🕵️ Fraud Detection Analysis

## 📌 Project Overview

This project explores fraud detection using transactional data, focusing on identifying behavioural patterns associated with fraudulent activity. The analysis follows a structured data science workflow, including data preprocessing, feature engineering, exploratory analysis, and classification modelling.

The objective is to demonstrate practical data analysis and modelling skills using real-world–inspired financial transaction data.

---

## 🧠 Dataset Overview

The dataset contains transaction-level records, including:
- Transaction type  
- Transaction amount  
- Sender and recipient account balances (before and after transactions)  
- Fraud labels indicating fraudulent activity  

The dataset exhibits a strong class imbalance, with fraudulent transactions representing only a small proportion of total observations.

---

## 🔧 Data Preprocessing & Feature Engineering

Data preprocessing was performed in **Python** to improve data quality and analytical reliability. The following steps were applied:

- Removal of non-informative identifier variables  
- Creation of balance change features:
  - `deltaOrig`: change in the sender’s account balance  
  - `deltaDest`: change in the recipient’s account balance  
- Logarithmic transformation of transaction amounts (`log_amount`) to reduce skewness  
- Selection of key variables relevant to fraud classification  

The cleaned dataset was then exported for further analysis.

---

## 📊 Exploratory Data Analysis

Exploratory analysis was conducted to understand transaction patterns and class distribution. Results showed a strong class imbalance, with fraudulent transactions occurring primarily within **TRANSFER** and **CASH_OUT** transaction types.

This insight informed the modelling approach and feature selection process.

---

## 🤖 Modelling Approach

Two classification models were applied:

- **Logistic Regression** – for interpretability and statistical inference  
- **Decision Tree Classifier** – to capture non-linear relationships and feature interactions  

Model performance was evaluated to assess predictive capability and interpretability.

---

## 🚀 Future Improvements

Several enhancements could further improve the robustness and performance of this analysis:

- Apply resampling techniques (e.g. SMOTE or undersampling) to address class imbalance  
- Evaluate additional machine learning models such as Random Forests or Gradient Boosting  
- Perform hyperparameter tuning to optimise model performance  
- Incorporate cross-validation for more reliable performance estimation  
- Explore feature importance and model explainability techniques (e.g. SHAP values)  
- Develop a simple deployment pipeline for real-time fraud prediction  

---

## 🧰 Tools & Technologies

- Python (Pandas, NumPy)
- R (statistical modelling and evaluation)
- Jupyter Notebook
- R Markdown
- GitHub

