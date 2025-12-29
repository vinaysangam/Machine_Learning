# 🚢 Titanic Survival Prediction – Logistic Regression with t-SNE Visualization

This project explores the famous **Kaggle Titanic dataset** using Logistic Regression to predict passenger survival.  
The workflow includes data preprocessing, exploratory analysis, model training, evaluation, and visualization — including a powerful **t-SNE based visual insight**.

---

## 📌 Problem Statement
Build a predictive model to determine whether a passenger survived the Titanic disaster based on their socio-economic status, demographics, and travel attributes.

---

## 📂 Project Structure

| File | Description |
|------|------------|
| `Titanic Data Analysis (Logit).ipynb` | Full EDA + Logistic Regression model |
| `Titanic Data Analysis (Logit)_tSNE.ipynb` | Includes t-SNE dimensionality reduction & visualization |
| `requirements.txt` | Python dependencies |

---

## 🧠 Key ML Concepts Demonstrated
- Logistic Regression (Binary Classification)
- Data Cleaning & Preprocessing
- Handling Missing Values
- Feature Engineering
- Train/Test Split
- Statistical Interpretation of Model
- Model Evaluation
- t-SNE Visual Exploration

---

## 🗂 Dataset
Dataset: **Kaggle Titanic – Machine Learning from Disaster**

Typical features used:
- Passenger Class
- Gender
- Age
- Siblings/Spouse Count
- Parents/Children Count
- Ticket Fare
- Embarkation Port

**Target**
```
Survived
1 → Survived
0 → Did not survive
```

---

## 📈 Performance Metrics

### Logistic Regression Model
From `Titanic Data Analysis (Logit).ipynb`:
- **Precision:** ~0.77  
- **Recall:** ~0.78  
- **F1-Score:** ~0.77  

### Logistic Regression + t-SNE Exploration
From `Titanic Data Analysis (Logit)_tSNE.ipynb`:
- **Precision:** ~0.76  
- **Recall:** ~0.76  
- **F1-Score:** ~0.75  

> These results indicate the model generalizes well while remaining interpretable.

---

## 🛠️ Tech Stack
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## ▶️ How to Run

1️⃣ Clone repository  
```
git clone https://github.com/<your-username>/Logistic_Regression
```

2️⃣ Navigate
```
cd Logistic_Regression
```

3️⃣ Install dependencies
```
pip install -r requirements.txt
```

4️⃣ Launch Notebook
```
jupyter notebook
```

---

## 🎨 Visual Insights
✔ Survival distribution across demographics  
✔ Feature influence patterns  
✔ t-SNE survival clusters

---

## 🚀 Future Enhancements
- Cross-validation
- Hyperparameter tuning
- Try advanced models (Random Forest / XGBoost)
- Deploy as API / Web App

---

## 👤 Author
**Vinay Sangam**

Data & AI Engineer