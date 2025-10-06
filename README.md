# 🧩 Customer Segmentation Using Unsupervised Machine Learning

This project applies **unsupervised learning techniques** to segment customers based on demographic and spending behavior data. The dataset used is the **Mall Customers dataset**, downloaded from Kaggle. The main objective is to identify distinct customer groups that can help businesses tailor marketing strategies and improve decision-making.

---

## 📊 Project Overview

Customer segmentation is a key aspect of data-driven marketing and customer relationship management.  
This project explores and compares multiple clustering algorithms to group customers based on:

- **Age**
- **Annual Income**
- **Spending Score**
- **Gender**

The project leverages several clustering techniques:
- **K-Means Clustering**
- **Hierarchical (Agglomerative) Clustering**
- **DBSCAN**

---

## 🧠 Objectives

- Perform **data preprocessing** (encoding, scaling, cleaning).
- Use **visualizations** to explore data distributions and correlations.
- Apply **K-Means clustering** and determine the optimal number of clusters using the **Elbow Method**.
- Build and compare results from **Hierarchical** and **DBSCAN** clustering.
- Visualize customer clusters and interpret their behavioral patterns.

---

## ⚙️ Technologies & Libraries Used

- **Python** 🐍
- **Pandas** – Data manipulation
- **NumPy** – Numerical computation
- **Matplotlib** & **Seaborn** – Visualization
- **Scikit-learn (sklearn)** – Machine learning models and preprocessing
- **SciPy** – Hierarchical clustering and dendrograms
- **KaggleHub** – Dataset download utility

---

## 📂 Dataset

**Source:** [Mall Customers Dataset on Kaggle](https://www.kaggle.com/datasets/joebeachcapital/customer-segmentation)

**Description:**
- `CustomerID`: Unique customer identifier  
- `Gender`: Male or Female  
- `Age`: Customer’s age  
- `Annual Income (k$)`: Income in thousands of dollars  
- `Spending Score (1–100)`: Spending score assigned by the mall  

---

## 🧾 Data Preprocessing

1. **Import & Inspect Data**
   - Loaded dataset using Pandas and checked data types and missing values.
2. **Feature Transformation**
   - Encoded `Gender` column as binary (Male = 1, Female = 0).
   - Scaled numerical features using `StandardScaler`.
3. **Feature Selection**
   - Dropped `CustomerID` as it’s not relevant for clustering.

---

## 📈 Exploratory Data Analysis (EDA)

- Plotted **histograms** for Age, Income, and Spending Score distributions.
- Used **heatmap correlation matrix** to understand relationships among variables.
- Visualized **gender distribution**.

---

## 🧮 Clustering Analysis

### 1. **K-Means Clustering**
- Determined the optimal cluster number using the **Elbow Method**.
- Visualized clusters and centroids on scatter plots.
- Compared different cluster counts (`k=3` and `k=6`).

### 2. **Hierarchical Clustering**
- Generated **dendrogram** using Ward linkage.
- Applied **Agglomerative Clustering** and visualized cluster assignments.

### 3. **DBSCAN**
- Implemented **density-based clustering** to detect arbitrary-shaped clusters and noise points.

---

## 📊 Visualizations

- Distribution plots (Histograms)
- Correlation heatmap
- Elbow plot for K-Means optimization
- Dendrogram (Hierarchical clustering)
- Cluster scatter plots (for K-Means, Hierarchical, and DBSCAN)

---

## 🚀 Results & Insights

- **K-Means (k=5–6)** provided well-separated customer clusters.
- Clear distinctions were found between:
  - **High-income, low-spending customers**
  - **Young, high-spending customers**
  - **Middle-aged, moderate-spending customers**
- Hierarchical and DBSCAN confirmed similar customer group patterns.



1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/customer-segmentation.git
