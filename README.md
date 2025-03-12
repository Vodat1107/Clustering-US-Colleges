# 🔍 K-Means Clustering from Scratch

## 📌 Overview
This project aims to **implement the K-Means clustering algorithm from scratch** using **object-oriented programming (OOP) principles in Python**. The goal is to **gain deeper insights** into how the algorithm works internally and compare our implementation with **Sklearn's KMeans**.

## 🎯 Objective
- Implement the **K-Means algorithm from scratch** using **NumPy**.
- Apply it to a **US College dataset** for clustering analysis.
- Compare results with **Sklearn's KMeans implementation**.
- Analyze and visualize cluster separability.

## 📊 Dataset
### 📌 **Data Source**
📂 Dataset Link: [US Colleges Dataset](https://drive.google.com/file/d/1IqSv-q8bE3Fa5n93ZB7-Jza0DffC3TK4/view?usp=sharing)

### 📌 **Dataset Description**
The dataset consists of **777 US colleges**, with **16 numerical features** and **1 categorical feature (Private)**. The main features include:
- **Applications & Enrollment**: `Apps`, `Accept`, `Enroll`
- **Academic Performance**: `Top10perc`, `Top25perc`
- **Student Population**: `F.Undergrad`, `P.Undergrad`
- **Financial Information**: `Outstate`, `Room.Board`, `Books`, `Personal`
- **Faculty Information**: `PhD`, `Terminal`, `S.F.Ratio`
- **Alumni Donations**: `perc.alumni`

---

## 🏗️ Methodology
### **📌 Data Preprocessing**
- Handling **missing values**.
- **Scaling** numerical features.
- **Encoding** categorical variables (`Private` column).

### **📌 K-Means Implementation**
We implement a **custom `KMeans` class** with the following **parameters** and **methods**:

#### **📌 Class: `KMeans`**
##### **📌 Parameters**
- `K`: Number of clusters
- `tol`: Convergence tolerance
- `max_iter`: Maximum number of iterations

##### **📌 Attributes**
- `cluster_centers_`: Final cluster centroids
- `labels_`: Cluster assignments for each data point
- `n_iter_`: Number of iterations run
- `inertia_`: Sum of squared distances to the nearest cluster

##### **📌 Methods**
- `fit(X)`: Train K-Means on dataset `X`
- `transform(X)`: Convert data into cluster-distance space
- `predict(X)`: Predict clusters for new data points
- `fit_transform(X)`: Train and transform data (optimized)
- `fit_predict(X)`: Train and assign clusters (shortcut method)

### **📌 Testing & Validation**
- Test our **custom `KMeans`** on the dataset.
- Validate results by comparing with **Sklearn's KMeans**.
- Use **evaluation metrics**:
  - **Elbow Method**
  - **Silhouette Score**
- Compare clustering results with the **Private (Public vs. Private universities) attribute**.

### **📌 Data Visualization**
- **Scatter plots** to visualize clusters.
- **Heatmaps** for feature correlation.
- **Elbow & Silhouette plots** to evaluate clustering performance.

---
