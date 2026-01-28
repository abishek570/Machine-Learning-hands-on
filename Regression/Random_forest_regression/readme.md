# 🌲 Salary Prediction using Random Forest Regression

This project demonstrates a **Random Forest Regression model** to predict **employee salary** based on their **position level**. The project is designed to be **simple and beginner-friendly**, showcasing how ensemble learning improves prediction accuracy.

---

## 📊 Dataset Description

The dataset used is **Position_Salaries.csv** and contains information about employee position levels and their corresponding salaries.

* **Independent Variables (Features):** 1  
* **Dependent Variable (Target):** 1  

Each row represents an employee role within an organization.

---

## 🧾 Data Dictionary

### 🔹 Independent Variable

| Feature | Description                    |
| ------ | ------------------------------ |
| Level  | Position level of the employee |

---

### 🎯 Dependent Variable

| Feature | Description                        |
| ------ | ---------------------------------- |
| Salary | Salary corresponding to the level |

This is a **regression problem**, as the output is a continuous numerical value.

---

## 🛠️ Project Steps (Copy_of_random_forest_regression.ipynb)

1. Import required libraries 📦  
2. Load the dataset 📂  
3. Separate features and target ⚙️  
4. Train Random Forest Regression model 🌲  
5. Predict salary values 🔮  
6. Visualize model predictions 📈  

---

## 📊 Visualize Model Prediction

![Random Forest Predictions](assets/random_forest_predictions.png)

This plot illustrates how the **Random Forest Regression model** predicts salaries:

* **Red points:** Actual salary values  
* **Blue curve:** Predicted salary values  

The smoother step-wise curve is produced by averaging predictions from multiple decision trees, allowing the model to capture **complex non-linear patterns** while reducing overfitting compared to a single decision tree.

---

## ✅ Conclusion

The Random Forest Regression model effectively predicts salaries by combining multiple decision trees into an ensemble. This project helps in understanding **ensemble learning**, **variance reduction**, and why Random Forests generally perform better than individual tree-based models.
