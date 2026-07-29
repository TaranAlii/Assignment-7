# 🛍️ AI-ML Assignment 7: Customer Segmentation using K-Means

This repository contains the implementation of **AI-ML Assignment – 7**, which focuses on segmenting mall customers into meaningful groups using **K-Means Clustering**.

The segmentation is based on customer demographics and purchasing behavior, particularly **Age, Gender, Annual Income, and Spending Score**. **Principal Component Analysis (PCA)** is then used to reduce the feature space to two dimensions for visualization.

---

## 👤 Student Information

- **Name:** Taran Ali Ahmed
- **Registration Number:** 23BCE10952
- **Application Number:** IN26009846
- **Batch:** 2B

---

# 📌 Objective

The objective of this project is to divide mall customers into distinct groups based on their demographic characteristics and spending behavior.

Customer segmentation can help mall management:

- Identify different customer profiles.
- Develop targeted marketing campaigns.
- Improve customer engagement.
- Design personalized offers and promotions.
- Understand high-value and low-value customer groups.

The project uses **K-Means Clustering** as the primary unsupervised learning algorithm and **PCA** for two-dimensional visualization.

---

# 📊 Dataset

The project uses the **Mall Customer Segmentation Dataset**.

### Dataset Source

- **Kaggle:** https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python

### Dataset Features

| Feature | Description |
|---------|-------------|
| **CustomerID** | Unique identifier assigned to each customer |
| **Gender** | Customer gender |
| **Age** | Customer age |
| **Annual Income (k$)** | Annual income in thousands of dollars |
| **Spending Score (1–100)** | Score assigned based on customer spending behavior |

> **Note:** `CustomerID` is removed during preprocessing because it is an identifier and does not provide useful information for customer segmentation.

---

# 🛠️ Libraries Used

The following Python libraries were used:

- **Pandas** – Data loading, cleaning, and analysis
- **NumPy** – Numerical computations
- **Scikit-Learn**
  - `StandardScaler` – Feature standardization
  - `LabelEncoder` – Encoding categorical values
  - `KMeans` – Customer clustering
  - `PCA` – Dimensionality reduction
- **Matplotlib** – Visualization
- **Seaborn** – Statistical visualization and cluster plots

---

# ⚙️ Methodology

The project follows a structured machine learning pipeline.

## 1. Data Understanding

The dataset was loaded and explored using Pandas.

The following steps were performed:

- Displayed the first few records.
- Examined dataset dimensions.
- Inspected data types.
- Calculated summary statistics.
- Identified numerical and categorical features.
- Checked for missing values.

The main features used for clustering are:

- Age
- Gender
- Annual Income
- Spending Score

---

## 2. Data Preprocessing

The following preprocessing operations were performed:

### Remove Unnecessary Features

The `CustomerID` column was removed because it is only an identifier and has no meaningful relationship with customer behavior.

### Encode Categorical Data

The `Gender` column was converted into numerical values using `LabelEncoder`.

For example:

```text
Female → 0
Male   → 1
