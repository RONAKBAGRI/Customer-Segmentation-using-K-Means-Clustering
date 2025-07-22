# 👥 Customer Segmentation using K-Means Clustering

This project applies **K-Means Clustering** to segment mall customers based on their **Annual Income** and **Spending Score**. The segmentation helps businesses understand customer groups and target marketing strategies effectively.

---

## 📄 Dataset

- **Source:** Mall Customer Segmentation Data (e.g., Kaggle, UCI, or internal CSV)
- **Description:** Contains basic information about mall customers, including:
  - CustomerID
  - Gender
  - Age
  - Annual Income (k$)
  - Spending Score (1–100)

---

## ⚙️ Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib & Seaborn  
- Scikit-learn (KMeans)

---

## 🚀 Project Workflow

### 1️⃣ Data Loading & Exploration
- Load the dataset using `pandas.read_csv`.
- Preview the data using `.head()`, `.shape`, and `.info()` methods.
- Check for missing values using `.isnull().sum()`.

### 2️⃣ Feature Selection
- Select **Annual Income** and **Spending Score** columns for clustering.
- Extract these into a NumPy array `X`.

### 3️⃣ Optimal Clusters Selection (Elbow Method)
- Compute WCSS (Within-Cluster Sum of Squares) for `k = 1 to 10`.
- Plot the elbow graph to determine the optimal number of clusters.

### 4️⃣ Model Training
- Fit the **KMeans** model using the optimal number of clusters (`k=5`).
- Predict cluster labels using `.fit_predict()`.

### 5️⃣ Visualization
- Visualize all clusters in a 2D scatter plot.
- Different colors are used for each customer group.
- Plot cluster centroids for reference.

---

## ✅ Results

- **5 distinct customer segments** were identified based on annual income and spending score.
- Each cluster represents a unique group with different purchasing behaviors, useful for targeted marketing and customer retention strategies.

---

## 💡 What We Learned

- How to apply **unsupervised learning** using K-Means.
- Use of **WCSS and Elbow Method** to determine optimal clusters.
- Visualizing and interpreting customer segments using scatter plots.
- Importance of feature selection for clustering.

---

## 📥 How to Run

1️⃣ **Clone this repository:**

```bash
git https://github.com/RONAKBAGRI/-Customer-Segmentation-using-K-Means-Clustering.git
```

2️⃣ **Install dependencies:**
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

3️⃣ **Run the notebook:**
```bash
jupyter notebook  Customer_Segmentation_using_K_Means_Clustering.ipynb
```