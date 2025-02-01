# Amex RiskGuard: Credit Default Prediction – Kaggle Competition

🚀 **Credit Default Risk Prediction using Machine Learning**

![American Express Default Prediction](https://www.kaggle.com/competitions/amex-default-prediction)

---

## 📜 Project Overview
This project was developed for the **Kaggle American Express Default Prediction Competition**, where the goal was to **predict customer credit defaults** based on **transaction behavior and financial indicators**.

We worked with a **massive dataset containing 5,530,681 transactions** and **191 anonymized features**, applying **feature engineering, class balancing, and machine learning models** to improve credit risk prediction.

### 🔹 Key Objectives:
✅ **Predict the probability of a customer defaulting on credit payments**  
✅ **Handle large-scale financial data with missing values and high dimensionality**  
✅ **Develop robust ML models with high recall and precision for risk assessment**  
✅ **Extract key insights to help financial institutions reduce credit risk**  

---

## 📂 Dataset Overview
- **Dataset Link:** [American Express Default Prediction Dataset](https://www.kaggle.com/competitions/amex-default-prediction/data)  
- **Total Records:** 5,530,681 transactions  
- **Total Features:** 191 anonymized customer financial indicators  
- **Class Distribution:**  
  - **Default (1): 25%**  
  - **Non-Default (0): 75%**  
- **Feature Categories:**  
  - **D_** → Delinquency variables  
  - **S_** → Spending variables  
  - **P_** → Payment variables  
  - **B_** → Balance variables  
  - **R_** → Risk indicators  

---

## 🔍 Exploratory Data Analysis (EDA) & Insights

📊 **Key Findings from EDA:**  
✔ **Defaulters had significantly more missing values** in delinquency & balance features.  
✔ **Transaction recency played a key role** in predicting defaults (higher risk within the first 50 days).  
✔ **Certain features (P_2, B_9, D_48) had high predictive power**, influencing risk assessment.  

---

## 🛠️ Feature Engineering & Preprocessing
✅ **Handled missing values using median imputation & feature-specific techniques**  
✅ **Created new engineered features (P2/D48 ratio, log-transformed B9 balance, customer transaction trends)**  
✅ **Applied StandardScaler & MinMaxScaler to normalize features**  
✅ **Implemented class balancing techniques (SMOTE, class weighting)**  

---

## 📈 Model Development & Results

| **Model**            | **ROC-AUC Score** | **Recall** | **False Negatives Reduction** |
|----------------------|------------------|------------|------------------------------|
| Logistic Regression | **86.4%**         | 65%        | - |
| Random Forest       | **91.2%**         | 72%        | 8% |
| XGBoost            | **94.1%**         | 78%        | 10% |
| **CatBoost**        | **94.6%**         | **83%**    | **14%** |

✅ **Final Model: CatBoost** → **94.6% AUC, recall increased from 69% → 83%**  
✅ **False negatives reduced by 14%, making the model highly reliable for risk prediction.**  

---

## 📌 Key Takeaways & Business Impact
✅ **High-importance features like P_2, B_9, and D_48 were strong indicators of customer default.**  
✅ **Defaulters had more erratic transaction patterns and higher delinquency risk within the first 50 days.**  
✅ **The final model (CatBoost) significantly improved credit risk prediction, reducing misclassification rates.**  
✅ **Insights from this model can help financial institutions make better lending decisions and improve risk management.**  

