# Fraud Detection in Loan Applications

## 📌 Project Overview
This project implements a **fraud detection model** to identify fraudulent loan applications using **anomaly detection techniques**. The dataset contains various loan-related features, including applicant income, credit history, loan amount, and approval status.

## 🚀 Technologies Used
- **Python**
- **Pandas, NumPy** (Data Processing)
- **Matplotlib, Seaborn** (Data Visualization)
- **Scikit-Learn** (Machine Learning Models)

## 📂 Dataset
The dataset consists of **614 loan applications** with the following key features:
- **Gender, Married, Dependents, Education, Self_Employed** (Applicant demographics)
- **ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term** (Financial data)
- **Credit_History, Property_Area, Loan_Status** (Loan decision and history)

## 🔍 Data Preprocessing
1. **Handling Missing Values:**
   - Imputed missing values using **mode** (categorical) and **median** (numerical).
2. **Encoding Categorical Variables:**
   - Used **Label Encoding** for categorical features.
3. **Feature Scaling:**
   - Standardized numerical features for better model performance.
4. **Train-Test Split:**
   - Split the dataset into **80% training and 20% testing**.

## 📊 Exploratory Data Analysis (EDA)
- **Boxplots & Histograms** to analyze distributions and detect outliers.
- **Correlation Heatmap** to identify relationships between features.
- **Credit History Influence:** Strongest factor affecting loan approvals.

## 🏆 Models Implemented
### 1️⃣ **Isolation Forest**
- Detects anomalies by assigning anomaly scores.
- **Accuracy:** 73%
- **Precision (Fraudulent Loans):** 100%
- **Recall (Fraudulent Loans):** 13% (Misses many fraud cases)

### 2️⃣ **Local Outlier Factor (LOF)**
- Detects outliers by comparing local density.
- **Accuracy:** 70%
- **Precision (Fraudulent Loans):** 57%
- **Recall (Fraudulent Loans):** 11% (Lower than Isolation Forest)

## 📉 Model Performance Summary
| Model              | Accuracy | Precision (Fraud) | Recall (Fraud) | F1-Score |
|-------------------|----------|------------------|--------------|----------|
| Isolation Forest | 73%      | 100%             | 13%          | 0.23     |
| LOF             | 70%      | 57%              | 11%          | 0.18     |

## 🔬 Challenges & Improvements
- **Low Recall:** Both models fail to detect most fraudulent applications.
- **Imbalanced Data:** Majority of loans are approved, making fraud cases rare.
- **Next Steps:**
  - Implement **Autoencoders (Deep Learning)** for better anomaly detection.
  - Use **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset.
  - Combine **supervised models (Random Forest, XGBoost)** for better performance.




