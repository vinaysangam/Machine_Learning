# Simple Linear Regression – TV Marketing vs Sales

## Overview
This project applies **Simple Linear Regression** to evaluate the relationship between **TV Marketing Spend** and **Sales Performance**.  
The objective is to quantify whether increased advertising investment leads to measurable improvement in sales outcomes and to develop a predictive capability to support business decision-making.

---

## Business Problem
Organizations frequently invest heavily in television advertising. Leadership expects clarity on return and effectiveness, including:

- Does TV marketing significantly influence sales performance?
- What level of sales improvement can be expected for a given increase in spend?
- Can sales be estimated in advance based on budget allocation?

This analysis addresses these questions using a structured statistical and machine learning approach.

---

## Dataset
| Feature | Description |
|--------|-------------|
| TV | TV marketing expenditure |
| Sales | Product sales outcome |

- Feature Type: Continuous
- Target Type: Continuous
- Learning Type: Supervised → Regression
- Model Type: Simple Linear Regression

---

## Methodology
1. Data exploration and understanding  
2. Visual analysis of feature vs target relationship  
3. Model training using Simple Linear Regression  
4. Coefficient and intercept interpretation  
5. Model evaluation using statistical metrics  
6. Business interpretation and insight generation  

---

## Model Representation

Sales = b0 + b1 × TV

Where:
- **b0 (Intercept):** Expected baseline sales when TV spend is zero  
- **b1 (Slope):** Estimated change in sales for every unit increase in TV marketing spend  

---

## Evaluation Metrics
Model performance is assessed using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

Lower error metrics and higher R² indicate a more reliable and better fitting model.

---

## Insights and Learnings
- Enables quantification of marketing effectiveness  
- Provides interpretability through coefficients  
- Supports strategic resource allocation  
- Forms foundation for advanced regression models such as multiple regression and regularized regression

---

## Technology Stack
- Python
- Pandas
- NumPy
- Seaborn / Matplotlib
- Scikit-learn

---

## Author
**Vinay Sangam**  
Data & AI Engineer
