# 🧮 Principal Component Analysis (PCA) — Professional Learning & Reference Guide

## 📌 Overview
Principal Component Analysis (PCA) is a **linear dimensionality reduction** technique used to transform high‑dimensional datasets into a smaller set of meaningful features (Principal Components), while retaining as much variance (information) as possible.

It helps in:
- Reducing dimensionality
- Removing multicollinearity
- Noise reduction
- Visualization of complex data
- Improving downstream ML performance

---

## 🧾 Brief Primer & History
PCA was introduced in **1901 by Karl Pearson** as an analogue of the principal axes theorem in mechanics and later formalized and extended by **Harold Hotelling in the 1930s**.

It uses an **orthogonal transformation** to convert correlated variables into **uncorrelated principal components**.  
These components are ordered such that:
- 1st component captures the highest variance
- 2nd captures the next highest variance under orthogonality constraint
- and so on…

PCA is **sensitive to feature scaling**, so normalization / standardization is critical.

---

## 🧠 Mathematical Foundation

Consider a dataset matrix:

\mathbf{X} ∈ ℝ^{n×p}

Where:
- n = number of observations
- p = number of features
- X is assumed to be centered (mean of each column is zero)

### Step 1 — Compute Covariance Matrix
\mathbf{C} = \frac{1}{n-1} \mathbf{X}^T \mathbf{X}

### Step 2 — Eigen Decomposition
Find eigenvalues (λ) and eigenvectors (w):

\mathbf{Cw} = \lambda \mathbf{w}

- Eigenvectors → Principal directions (principal components)
- Eigenvalues → Variance explained by each component

### Step 3 — Ordering Components
Components are ranked:

λ₁ ≥ λ₂ ≥ λ₃ … ≥ λₚ

### Step 4 — Projection
Principal Component Scores:

tₖ(i) = \mathbf{x}_{(i)} \cdot \mathbf{w}_{(k)}

Matrix form:

\mathbf{T} = \mathbf{XW}

Where:
- W = matrix of eigenvectors
- T = transformed dataset in PCA space

### Maximization Objective
PCA maximizes projected variance:

\mathbf{w}_{(1)} = arg max_{||w||=1} (||Xw||²)

Subject to:
- orthogonality constraints
- unit length eigenvectors

### Successive Component Extraction
After extracting k−1 components:

X̂ₖ = X − Σ (X wₛ wₛᵀ)

Next component:

\mathbf{w}_{(k)} = arg max \frac{\mathbf{w}^T \mathbf{\hat{X}}^T \mathbf{\hat{X}} \mathbf{w}}{\mathbf{w}^T \mathbf{w}}

In modern practice:
📌 PCA is computed using **Singular Value Decomposition (SVD)** for numerical stability.

---

## 📉 Variance Explained
Explained Variance Ratio:

EVRₖ = λₖ / Σ λ

Cumulative Variance tells how many components we need:

Σ EVRₖ ≥ Threshold (e.g., 90–95%)

---

## 🔍 Where PCA is Useful
- Customer Segmentation
- Finance Risk Modeling
- Gene Expression Analysis
- Image Compression
- Noise Filtering
- Recommendation Systems
- Preprocessing for ML Models

---

## ⚠️ Limitations
- Assumes linear relationships
- Sensitive to feature scaling
- Components may be hard to interpret
- Poor performance on highly non‑linear datasets → t‑SNE / UMAP preferred

---

## 🛠️ Tech Used in Notebook
- Python
- NumPy
- Pandas
- Scikit‑learn
- Matplotlib / Seaborn

---

## 👤 Author
**Vinay Sangam**  
_Data & AI Engineer_

---
⭐ Explore more Machine Learning work across the repository!
