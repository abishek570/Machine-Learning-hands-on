# 📈 Startup Profit Prediction using Multiple Linear Regression

This project demonstrates a **Multiple Linear Regression model** to predict **startup profit** based on spending across different departments and the state in which the startup operates. The project is designed to be **simple and beginner-friendly**.

---

## 📊 Dataset Description

The dataset used is **50_Startups.csv** and contains information about startup investments and profits.

* **Independent Variables (Features):** 4
* **Dependent Variable (Target):** 1

Each row represents one startup.

---

## 🧾 Data Dictionary

### 🔹 Independent Variables

| Feature         | Description                            |
| --------------- | -------------------------------------- |
| R&D Spend       | Money spent on Research & Development  |
| Administration  | Money spent on Administration          |
| Marketing Spend | Money spent on Marketing               |
| State           | Location where the startup is situated |

---

### 🎯 Dependent Variable

| Feature | Description                        |
| ------- | ---------------------------------- |
| Profit  | Final profit earned by the startup |

This is a **regression problem**, as the output is a continuous numerical value.

---

## 🛠️ Project Steps (Copy_of_multiple_linear_regression.ipynb)

1. Import required libraries 📦
2. Load the dataset 📂
3. Encode categorical data (State) 🔄
4. Split dataset into features and target ⚙️
5. Train-test split ✂️
6. Train Multiple Linear Regression model 🧪
7. Predict profit values 🔮
8. Evaluate model performance 📈

---

## 📊 Manual Evaluation (Actual vs Predicted Values)

![Actual vs Predicted Values](assets/plot.png)

This scatter plot compares:

* **Red points:** Actual profit values (y_test)
* **Blue points:** Predicted profit values (y_pred)

The closeness between red and blue points indicates that the model predictions are reasonably accurate, showing a good linear fit between input features and profit.

---

## ✅ Conclusion

The Multiple Linear Regression model successfully predicts startup profits based on departmental spending and location. This project serves as a strong foundation for understanding **regression analysis**, **feature impact**, and **model evaluation** in machine learning.
