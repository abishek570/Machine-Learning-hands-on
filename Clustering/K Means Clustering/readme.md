# 🛍️ Customer Segmentation using K-Means Clustering

This project demonstrates a **K-Means Clustering model** to segment customers based on their **annual income** and **spending score**. The project focuses on unsupervised learning and customer segmentation analysis.

---

## 📊 Dataset Description

The dataset used is **Mall_Customers.csv** and contains customer demographic and spending information.

* **Independent Variables (Features):** 2 (used for clustering)
* **Dependent Variable (Target):** None (Unsupervised Learning)

Each row represents a customer in the mall.

---

## 🧾 Data Dictionary

### 🔹 Features Used for Clustering

| Feature               | Description                                      |
|-----------------------|--------------------------------------------------|
| Annual Income (k$)    | Annual income of the customer (in thousand $)   |
| Spending Score (1-100)| Score assigned based on spending behavior       |

> K-Means is an **unsupervised algorithm**, meaning there is no target variable.

---

## 🛠️ Project Steps (Copy_of_k_means_clustering.ipynb)

1. Import required libraries 📦  
2. Load the dataset 📂  
3. Select relevant features ⚙️  
4. Apply Elbow Method 📉  
5. Train K-Means clustering model 🧪  
6. Visualize clusters 📈  

---

## 📊 Elbow Method

![Elbow Method Plot](assets/image%20copy.png)

The **Elbow Method** helps determine the optimal number of clusters (K).

It works by plotting:

- **Number of clusters (K)**
- **Within-Cluster Sum of Squares (WCSS)**

### 🔍 What is WCSS?

WCSS (Within-Cluster Sum of Squares) measures how compact the clusters are.  
Lower WCSS indicates tighter clusters.

### 📌 How to Select the Optimal Number of Clusters?

- As K increases, WCSS decreases.
- Initially, the decrease is sharp.
- After a certain point, the decrease slows down.
- The point where the graph forms a noticeable “bend” or **elbow** is considered the optimal K.

In this project, the elbow appears at **K = 5**, so 5 clusters were selected.

---

## 📊 Visualize Customer Segments

![Customer Segmentation](assets/image.png)

The scatter plot shows:

- Different colored clusters representing customer groups  
- Cluster centroids marked clearly  
- Segmentation based on income and spending patterns  

This segmentation helps businesses identify:

- High-income, high-spending customers  
- Low-income, low-spending customers  
- Target customer groups for marketing  

---

## ✅ Conclusion

The K-Means Clustering model successfully segments customers into meaningful groups based on spending behavior and income levels.

This project strengthens understanding of:

- Unsupervised learning  
- Cluster analysis  
- Elbow Method for selecting optimal K  
- Customer segmentation in business analytics  

K-Means is widely used in marketing analytics, recommendation systems, and customer profiling.
