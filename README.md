# 💸 Financial Risk Profile Prediction

## 🧠 Objective
Train a machine learning model to predict the **financial risk profile** of individuals and provide **explainability** to understand the key features affecting their financial health.

---

## 🔁 Process Overview

### ✅ 1. Data Understanding
- The dataset is **synthetic**, containing demographic, economic, and behavioral variables.
- The **target variable** represents **three classes** of financial risk: `Low`, `Medium`, and `High`.

---

### ⚙️ 2. Model Training and Evaluation
- Trained multiple classification models:
  - **Random Forest Classifier** (with GridSearchCV tuning)
  - **XGBoost Classifier**
- Evaluation Metrics:
  - **Accuracy ≈ 33%**
  - **Precision, Recall, F1-Score ≈ 0.33** for all classes
  - **Confusion matrix** showed uniform misclassification—suggesting random predictions.

---

### 📊 3. Observations
- Due to the **synthetic nature of the dataset**, we observed:
  - **High overlap** of feature values across all classes.
  - **Weak correlation** between input features and the target variable.
  - No clear class separation after PCA and visualization.

---

## ⭐ Key Insights: Top Influential Features

Despite the low accuracy, the following features consistently appeared as **important drivers of financial health**:

```
Top Features Identified:
-------------------------
1. Mortgage Information  
2. Savings Rate  
3. Inflation Rate  
4. Emergency Fund Status  
5. Debt-to-Income Ratio  
6. Local Unemployment Rate  
7. Investment Accounts  
8. Credit Card Usage  
9. Interest Rates  
10. Average Monthly Expenses  
11. Credit Score  
12. Age  
13. Bank Account Activity  
14. Years in Current Job  
15. Number of Credit Inquiries
```

---

## 📌 Conclusion
- The dataset's **overlapping structure** limited the model's predictive power.
- However, **feature importance analysis** helped highlight the core elements that likely influence an individual's financial risk status.
- These insights can be valuable when applied to **real-world financial data** for better decision-making.

---
