# 📊 Multiple Linear Regression — Theory, Mathematics & Practical Understanding

## 📌 Introduction
Multiple Linear Regression (MLR) is a supervised learning technique used to model the relationship between a **continuous dependent variable** and **multiple independent variables**. It extends simple linear regression from one predictor to many, enabling more realistic modeling of business and real‑world systems.

This project implements MLR on **Marketing Spend vs Sales**, while this document provides the **complete theoretical foundation and interpretation guide** aligned with enterprise analytics practices.

---

## 1️⃣ What is Multiple Linear Regression?
Multiple Linear Regression estimates:

\[
y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + … + \beta_D x_D + \epsilon
\]

Where:
- y → Target variable (Sales)
- x₁…x_D → Predictor variables (TV, Radio, Newspaper etc.)
- β₀ → Intercept
- βᵢ → Coefficient of each predictor
- ε → Random error

---

## 2️⃣ Why Multiple Linear Regression?
Simple regression only evaluates one factor at a time.  
Real world outcomes depend on **multiple drivers simultaneously**.

Multiple Regression helps:
✔ Measure combined influence  
✔ Separate individual effects  
✔ Control inter‑dependencies  
✔ Create reliable prediction systems  

Example:
Sales = TV + Radio + Newspaper  
Revenue = Customer Count + Price + Region  
House Price = Size + Location + Rooms  

---

## 3️⃣ Matrix Representation (Professional Form)
Multiple Regression in matrix notation:

\[
\mathbf{y} = \mathbf{X\beta} + \epsilon
\]

Where:
- y → n×1 output vector
- X → n×(D+1) feature matrix
- β → coefficient vector
- ε → noise

This enables analytical solving.

---

## 4️⃣ How Does MLR Estimate Coefficients?
MLR uses **Ordinary Least Squares (OLS)**.
Goal → Minimize Residual Sum of Squares (RSS)

\[
RSS = \sum (y_i − \hat{y_i})^2
\]

Analytical solution:

\[
\hat{\beta} = (X^T X)^{-1} X^T y
\]

Libraries like scikit‑learn and statsmodels compute this internally.

---

## 5️⃣ Interpreting Model Parameters

### 🔹 Intercept (β₀)
Predicted value when all predictors are zero.

### 🔹 Coefficients (βᵢ)
Change in dependent variable **when that predictor changes by 1 unit**, keeping others constant.

Example:
If β₂ = 0.05 for Radio:
> Increasing Radio spend by 1 unit → Sales increase by 0.05 units  
Holding TV & Newspaper fixed.

---

## 6️⃣ Key Assumptions of Multiple Linear Regression

| Assumption | Meaning | Validated Using |
|----------|--------|----------------|
| Linearity | Relationship is linear | Scatter & fit plots |
| Independence | Observations independent | Data design |
| Homoscedasticity | Equal residual variance | Residual vs Predicted |
| Normal Residuals | Errors normally distributed | Histogram / QQ Plot |
| No Multicollinearity | Predictors not highly correlated | Correlation / VIF |

📌 Violations reduce trustworthiness of results.

---

## 7️⃣ Model Evaluation Metrics

### Error-Based Metrics
- MAE — Mean Absolute Error  
- MSE — Mean Squared Error  
- RMSE — Root Mean Squared Error

Lower → Better

### Goodness of Fit — R²
\[
R^2 = 1 − \frac{RSS}{TSS}
\]

Meaning:
- 0 → Model explains nothing
- 1 → Perfect explanation
- 0.7–0.95 → Strong models in business context

### Adjusted R²
Prevents misleading improvement when adding useless variables.

---

## 8️⃣ Statistical Significance (Statsmodels Perspective)
Each predictor provides:
- Coefficient
- Standard Error
- t‑Statistic
- p‑Value

📌 p‑Value < 0.05 → Statistically significant predictor  
📌 p‑Value > 0.05 → Weak or irrelevant predictor

Example:
Newspaper often becomes insignificant once TV & Radio are present → indicates redundancy.

---

## 9️⃣ Residual Diagnostics
Residuals evaluate model reliability.

### ✔ Residual Distribution
Should be normal.

### ✔ Residual vs Predicted Plot
Should show random spread, not pattern.

### ✔ QQ Plot
Residuals should align with 45° reference line.

If not → model may be incorrect / missing features / nonlinear relationship.

---

## 🔟 Multicollinearity
When predictors are highly correlated:
- Coefficients become unstable
- Interpretation becomes misleading
- Performance deteriorates

### Variance Inflation Factor (VIF)
| VIF Value | Interpretation |
|---------|----------------|
| < 5 | Acceptable |
| 5 – 10 | Concerning |
| > 10 | Serious issue |

---

## 💼 Business Value
Multiple Linear Regression enables:
✔ Marketing ROI evaluation  
✔ Budget optimization  
✔ Sales forecasting  
✔ Driver importance analysis  
✔ Evidence‑based decision making  

Leadership gains:
- Clear insight into what matters
- Quantified financial impacts
- Reliable predictive capability

---

## 🚫 When NOT to Use MLR
Avoid when:
❌ Relationships are nonlinear  
❌ Strong multicollinearity exists  
❌ Too many predictors for dataset size  
❌ Heavy outliers distort model  
❌ Target isn’t continuous  

Better alternatives:
- Polynomial Regression
- Ridge / Lasso Regression
- Tree‑based Models
- Nonlinear ML Models

---

## ✅ Final Summary
Multiple Linear Regression is:
- Statistically robust  
- Highly interpretable  
- Business‑friendly  
- Foundation for advanced ML models  

It supports:
📌 Understanding  
📌 Prediction  
📌 Explainability  
📌 Decision Intelligence  

---

## 👤 Author
**Vinay Sangam**  
Data & AI Engineer
