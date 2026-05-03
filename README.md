# Customer-Credit-Risk-Project

# Customer Credit Risk Analysis & Data Preprocessing Pipeline

## Project Overview
This project focuses on building an end-to-end data preprocessing and feature engineering pipeline for a Customer Credit dataset.

The goal is to transform raw, multi-source financial data into a clean and machine-learning-ready dataset for predicting customer credit risk (`default_flag`).

---

## Objectives
- Integrate data from multiple sources (CSV, SQL, JSON, API)
- Clean and preprocess raw financial data
- Handle missing values and outliers
- Encode categorical variables
- Apply feature scaling and transformations
- Perform feature engineering
- Generate a final ML-ready dataset

---

## Dataset Description
The dataset contains customer financial and behavioral information such as:

- Income details
- Loan amount
- Credit score
- Transaction history
- Demographic data
- Loan purpose
- Target variable: `default_flag` (0 = No Default, 1 = Default)

---

## Data Preprocessing Steps

### 1. Data Integration
Data was merged from multiple sources:
- CSV files
- SQL database
- JSON files
- REST API

---

### 2. Missing Value Handling
- Numerical features: Mean/Median imputation  
- Categorical features: Mode imputation  

---

### 3. Outlier Handling
- Outliers detected using IQR method  
- RobustScaler used to reduce impact of extreme values  

---

### 4. Encoding
- One-Hot Encoding: gender, region, loan_purpose  
- Label Encoding where required  

---

### 5. Feature Scaling
Applied different scaling techniques:
- Standardization (Z-score scaling)
- Min-Max scaling
- Max-Abs scaling
- Robust scaling

---

### 6. Feature Transformation
- Log transformation
- Square root transformation
- Reciprocal transformation
- Power transformation (Box-Cox / Yeo-Johnson)

---

### 7. Feature Engineering
New features created:
- Debt-to-Income Ratio  
- Spending-to-Income Ratio  
- Average Monthly Transactions  
- Income groups using KMeans clustering  

---

## Final Output
The final dataset is:
- Cleaned and preprocessed
- Fully encoded and scaled
- Feature engineered
- Ready for machine learning models
