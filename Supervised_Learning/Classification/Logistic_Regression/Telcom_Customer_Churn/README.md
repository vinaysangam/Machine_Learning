# Telco Customer Churn Prediction – Logistic Regression

## 📌 Business Problem
Customer churn results in major revenue loss for telecom companies. Identifying **which customers are likely to churn** enables proactive retention strategies such as personalized offers, improved support engagement, and loyalty programs.

This project builds a **Logistic Regression model** to predict churn probability and extract meaningful business insights.

---

## 🧠 Dataset Overview
Key Features include:
- Customer demographics (SeniorCitizen, Partner, Dependents)
- Subscription behavior (Contract type, Internet service)
- Service engagement (Tech Support, Streaming Services)
- Financial attributes (MonthlyCharges, TotalCharges)
- 📍 **Target Variable: Churn (Yes/No)**

---

## 🎯 Machine Learning Objective
Predict:

```
Churn = 1  (Customer Will Leave)
Churn = 0  (Customer Will Stay)
```

Logistic Regression is chosen because it provides:
✔ Probability-based prediction  
✔ Strong interpretability  
✔ Business-aligned outputs  

---

## 🧪 Methodology
1️⃣ Data Cleaning & Transformation  
2️⃣ Encoding categorical features  
3️⃣ Train-Test Split  
4️⃣ Feature Scaling  
5️⃣ Logistic Regression Training  
6️⃣ Model Evaluation  
7️⃣ Business Interpretation  

---

## 📊 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC Curve & AUC

Special Focus:
- Recall → Important to capture customers likely to churn
- AUC → Overall discrimination strength

---

## 💼 Business Impact
Insights help answer:
- Which customers are at highest churn risk?
- What behavioral attributes drive churn?
- How should retention strategy prioritize customers?

Churn probability enables risk buckets:
- > 0.7 → High Risk (Immediate intervention)
- 0.4 – 0.7 → Medium Risk
- < 0.4 → Low Risk

---

## ⚠️ Practical Considerations
- False Negatives = Lost Revenue  
- False Positives = Retention Cost  
Decision threshold tuning is critical for enterprise deployment.

---

## 👤 Author
**Vinay Sangam**  
Data & AI Engineer
