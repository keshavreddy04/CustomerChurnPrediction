# Customer Churn Prediction

![Python](https://img.shields.io/badge/Python-3.12-blue) ![XGBoost](https://img.shields.io/badge/XGBoost-GradientBoosting-orange) ![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Supervised-green)

---

## 📌 Project Overview
Predict whether a customer will churn (leave) a telecom provider using **XGBoost**. The model leverages customer demographics, account info, and service usage to identify churn patterns.

---

## 📂 Dataset
- **Source:** Kaggle - [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Target:** `Churn` (Yes/No)
- **Features:** `gender`, `SeniorCitizen`, `Partner`, `Dependents`, `tenure`, `MonthlyCharges`, `Contract`, `PaymentMethod`, `InternetService`, etc.

---

## 🔍 Exploratory Data Analysis
- Distribution analysis of numeric features: `tenure`, `MonthlyCharges`.
- Churn analysis by categorical features: `Contract`, `PaymentMethod`, `InternetService`.
- Visualized correlation heatmap to identify feature relationships.
- Detected class imbalance (`Yes` < `No`) in churn.

---

## 🛠 Preprocessing
- Handled missing values.
- Encoded categorical features (one-hot encoding).
- Label-encoded target variable (`Churn_Encoded`).
- Balanced classes using **SMOTE** for better model performance.

---

## 🧠 Model & Performance
- **Algorithm:** XGBoost Classifier
- **Metrics after tuning & SMOTE:**
  - **Accuracy:** 0.83
  - **F1-score (Churned):** 0.71
  - Improved recall for minority class.

---

## 💾 Saved Model
- `xgb_churn_model.pkl` → Trained XGBoost model  
- `feature_columns.pkl` → Columns used for training  

## 👨‍💻 Author

* V Om Keshava Reddy
* 📌 B.Tech CSE (AI & ML), SRM University
* 🔗 [LinkedIn](https://www.linkedin.com/in/v-om-keshava-reddy-792478349/)| [GitHub](https://github.com/keshavreddy04)| [LeetCode](https://leetcode.com/u/keshav_30/)
