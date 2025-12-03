# 📊 Customer Churn EDA Python Project

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on a telecom customer churn dataset.  
The goal is to explore customer behavior and identify patterns related to churn (customers leaving the service).  
It is kept simple — focusing on **data cleaning, visualization, and insights** without predictive modeling.

## 📂 Dataset
- **Source**: [Telco Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
- **Rows:** 7,043  
- **Columns:** 21  
- **Target Variable:** `Churn` (Yes/No)  
- **Features:** Customer demographics, services subscribed, billing/payment details, tenure, charges.

## 🛠️ Tools & Libraries
- **Python** (3.x)  
- **pandas** – data cleaning & manipulation  
- **numpy** – numerical operations  
- **matplotlib** – visualization  
- **seaborn** – advanced plots  

## 🔎 Steps Performed
1. **Data Cleaning**
   - Converted `TotalCharges` to numeric (handled blanks as `0`).
   - Checked for duplicates (`customerID` → none).
   - Verified no missing values.

2. **Univariate Analysis**
   - Distribution of churn (`Yes` vs `No`).
   - Count plots for categorical features (Contract, InternetService, PaymentMethod).
   - Histograms for numerical features (tenure, MonthlyCharges, TotalCharges).

3. **Bivariate Analysis**
   - Churn vs SeniorCitizen.
   - Churn vs Contract type.
   - Tenure distribution split by churn.
   - MonthlyCharges distribution split by churn.

## 📈 Key Insights
- **Overall Churn Rate**:  
  - Yes (Churned) → **26.54%** (1,869 customers)  
  - No (Retained) → **73.46%** (5,174 customers)  

- **Senior Citizens**:  
  - Churned → **41.7%**  
  - Retained → **58.3%**  
  - Non‑seniors churn only **23.6%**.

- **Contract Type**:  
  - Month‑to‑Month → Highest churn (~43%).  
  - One Year → Lower churn (~11%).  
  - Two Year → Lowest churn (~3%).  

- **Tenure**:  
  - Customers with **1–2 months tenure** churn heavily.  
  - Customers with **> 2 years tenure** mostly stay.  

- **Payment Method**:  
  - Electronic Check users churn the most (~34%).  
  - Automatic Bank Transfer / Credit Card users churn less (~15–17%).  

- **Charges**:  
  - Average MonthlyCharges for churned customers: **~74.4**  
  - Average MonthlyCharges for retained customers: **~61.3**
