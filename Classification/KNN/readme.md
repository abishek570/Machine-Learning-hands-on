# 🤝 Purchase Prediction using K-Nearest Neighbors (K-NN)

This project demonstrates a **K-Nearest Neighbors (K-NN) classification model** to predict whether a user will **purchase a product** based on their **age** and **estimated salary**. The project is designed to be **simple and beginner-friendly**, focusing on distance-based classification.

---

## 📊 Dataset Description

The dataset used is **Social_Network_Ads.csv** and contains user demographic information and purchase decisions.

* **Independent Variables (Features):** 2  
* **Dependent Variable (Target):** 1  

Each row represents a user and whether they purchased the product.

---

## 🧾 Data Dictionary

### 🔹 Independent Variables

| Feature          | Description                    |
|------------------|--------------------------------|
| Age              | Age of the user                |
| EstimatedSalary  | Estimated annual salary        |

---

### 🎯 Dependent Variable

| Feature   | Description                     |
|-----------|---------------------------------|
| Purchased | 0 = Not Purchased<br>1 = Purchased |

This is a **binary classification problem**.

---

## 🛠️ Project Steps (k_nearest_neighbors.ipynb)

1. Import required libraries 📦  
2. Load the dataset 📂  
3. Separate features and target ⚙️  
4. Apply feature scaling 🔄  
5. Train K-NN classifier 🤝  
6. Predict test set results 🔮  
7. Visualize training and test results 📈  

---

## 📊 Visualize Model Prediction

### 🔹 Training Set Results

![K-NN Training Set](assets/knn_training_set.png)

This plot shows how the K-NN model learns decision boundaries from the **training data**:

* **Red region (0):** Users predicted as not purchasing  
* **Blue region (1):** Users predicted as purchasing  
* Points represent actual data samples

---

### 🔹 Test Set Results

![K-NN Test Set](assets/knn_test_set.png)

This plot visualizes the model’s performance on **unseen test data**.  
The similarity between training and test decision regions indicates that the model generalizes reasonably well.

---

## ✅ Conclusion

The K-Nearest Neighbors model effectively classifies users based on **age and estimated salary** by relying on distance to nearby data points. This project helps in understanding **instance-based learning**, **feature scaling importance**, and **decision boundary visualization** in classification problems.
