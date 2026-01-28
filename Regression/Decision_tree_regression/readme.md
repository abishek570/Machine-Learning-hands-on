# 🌳 Salary Prediction using Decision Tree Regression

This project demonstrates a **Decision Tree Regression model** to predict **employee salary** based on their **position level**. The project is designed to be **simple and beginner-friendly**, highlighting how tree-based models learn step-wise patterns from data.

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

## 🛠️ Project Steps (Decision_tree_regression.ipynb)

1. Import required libraries 📦  
2. Load the dataset 📂  
3. Separate features and target ⚙️  
4. Train Decision Tree Regression model 🌳  
5. Predict salary values 🔮  
6. Visualize model predictions 📈  

---

## 📊 Visualize Model Prediction

![Predictions Plot](assets/predictions_plot.png)

This plot illustrates how the **Decision Tree Regression model** predicts salaries:

* **Red points:** Actual salary values  
* **Blue line:** Predicted salary values  

The step-wise pattern occurs because Decision Trees split data into discrete regions and assign a constant prediction within each region. This behavior makes the model effective for capturing **non-linear relationships**, but it can also lead to sharp jumps in predictions.

---

## ✅ Conclusion

The Decision Tree Regression model successfully predicts salaries by learning **rule-based splits** from the data. This project helps in understanding **tree-based regression models**, their strengths in modeling non-linear data, and their characteristic step-wise prediction behavior.
