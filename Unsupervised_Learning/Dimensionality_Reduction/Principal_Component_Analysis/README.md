
# 📉 Principal Component Analysis (PCA)

## 🔷 Brief Primer & History
Principal Component Analysis (PCA) is a **statistical dimensionality reduction technique** that transforms a dataset with possibly correlated features into a new feature space consisting of **linearly uncorrelated variables** called **Principal Components (PCs)**.

- First component captures **maximum variance**
- Each subsequent component captures maximum remaining variance
- Components are **orthogonal**
- Sensitive to **feature scaling**

Invented by **Karl Pearson (1901)** and later formalized by **Harold Hotelling (1930s)**.

---

## 🧮 Mathematical Foundation

Assume a dataset matrix:

- \( \mathbf{X} \) : \( n \times p \) matrix  
- \( n \) = samples  
- \( p \) = features  
- Data is mean-centered

### ✅ Objective
Find a projection that maximizes variance:

\(\max \ \mathrm{Var}(\mathbf{Xw}) \)

subject to

\(\|\mathbf{w}\| = 1\)

---

## ✔ Step 1 — Covariance Matrix
Compute covariance matrix:

$$
\mathbf{C} = \frac{1}{n-1}\mathbf{X}^T \mathbf{X}
$$

---

## ✔ Step 2 — Eigen Decomposition
Solve for eigenvalues \( \lambda \) and eigenvectors \( \mathbf{w} \):

$$
\mathbf{Cw} = \lambda \mathbf{w}
$$

Where:

- **Eigenvectors** → Principal directions (Principal Components)
- **Eigenvalues** → Variance captured by each PC

---

## ✔ Step 3 — Order Components
Eigenvalues ranked:

$$
\lambda_1 \ge \lambda_2 \ge \lambda_3 \dots \ge \lambda_p
$$

Largest eigenvalue → Highest variance direction.

---

## ✔ Step 4 — Project Data
Projection of sample \( i \) on component \( k \):

$$
t_k^{(i)} = \mathbf{x}^{(i)} \cdot \mathbf{w}_k
$$

Matrix projection form:

$$
\mathbf{T} = \mathbf{XW}
$$

- \( \mathbf{T} \) → Transformed PCA space
- \( \mathbf{W} \) → Matrix of eigenvectors

---

## 📊 Variance Explained
Explained Variance Ratio:

$$
\text{EVR}_k = \frac{\lambda_k}{\sum_{i=1}^{p}\lambda_i}
$$

Cumulative:

$$
\text{Cumulative EVR} = \sum_{k=1}^{m} \text{EVR}_k
$$

Used to decide how many PCs to retain.

---

## 🧠 Intuition
PCA rotates the coordinate system so that:

- Axis‑1 aligns with maximum variance direction
- Axis‑2 aligns with next maximum orthogonal variance
- Noise + redundancy reduce

Think of PCA as:

> “Finding better coordinate axes for your data”

---

## 🏢 Business Value
PCA is widely used in:
- Customer segmentation
- Financial risk analysis
- Image compression
- Noise reduction
- Feature engineering
- Visualization of high‑dimensional data

---

## ⚠️ When PCA May Not Work Well
- Non‑linear structure (use t‑SNE or UMAP)
- Highly imbalanced variance
- Not scaled data
- When interpretability of raw features is critical

---

## 🛠 Tech Stack Aligned
- NumPy
- Pandas
- Scikit‑learn
- Matplotlib / Seaborn

---

## 👤 Author
**Vinay Sangam**  
_Data & AI Engineer_
