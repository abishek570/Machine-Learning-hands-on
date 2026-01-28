# ❤️ Heart Disease Prediction using Logistic Regression

This project demonstrates a **beginner-friendly Logistic Regression model** to predict the presence of heart disease using clinical patient data.

---

## 📊 Dataset Description

The dataset contains **14 columns**:

* **13 independent variables (features)**
* **1 dependent variable (target)**

Each row represents medical information of a patient used to predict heart disease.

---

## 🧾 Data Dictionary

### 🔹 Independent Variables

| Feature  | Description                     | Values                                                                                |
| -------- | ------------------------------- | ------------------------------------------------------------------------------------- |
| age      | Age of the patient              | Years                                                                                 |
| sex      | Gender                          | 1 = Male, 0 = Female                                                                  |
| cp       | Chest pain type                 | 0 = Typical angina<br>1 = Atypical angina<br>2 = Non-anginal pain<br>3 = Asymptomatic |
| trestbps | Resting blood pressure          | mm Hg                                                                                 |
| chol     | Serum cholesterol               | mg/dl                                                                                 |
| fbs      | Fasting blood sugar > 120 mg/dl | 1 = True, 0 = False                                                                   |
| restecg  | Resting ECG results             | 0 = Normal<br>1 = ST-T abnormality<br>2 = LV hypertrophy                              |
| thalach  | Maximum heart rate achieved     | Numeric                                                                               |
| exang    | Exercise-induced angina         | 1 = Yes, 0 = No                                                                       |
| oldpeak  | ST depression by exercise       | Numeric                                                                               |
| slope    | Peak exercise ST slope          | 0 = Upsloping<br>1 = Flat<br>2 = Downsloping                                          |
| ca       | Major vessels colored           | 0 – 3                                                                                 |
| thal     | Thalassemia                     | 0 = Error<br>1 = Fixed defect<br>2 = Normal<br>3 = Reversible defect                  |

---

### 🎯 Target Variable

| Feature | Meaning                                            |
| ------- | -------------------------------------------------- |
| target  | 0 = No heart disease ❤️‍🩹<br>1 = Heart disease ❤️ |

This is a **binary classification problem**.

---

## 🛠️ Project Steps (LogisticRegression.ipynb)

1. Import required libraries 📦
2. Load and inspect the dataset 📂
3. Perform basic data analysis 🔍
4. Split features and target ⚙️
5. Train-test split ✂️
6. Train Logistic Regression model 🧪
7. Make predictions 🔮
8. Evaluate model performance 📈

---

## 📊 Evaluation / Classification Report

### 🔹 Confusion Matrix

![Confusion Matrix](assets/Screenshot%202026-01-20%20140855.png)

The confusion matrix shows how well the model classifies patients:

* **True Negatives (22):** Correctly predicted no heart disease
* **True Positives (30):** Correctly predicted heart disease
* **False Positives (5):** Predicted disease when not present
* **False Negatives (4):** Missed disease cases

This indicates the model performs well with relatively few misclassifications.

---

### 🔹 Classification Report Heatmap

![Classification Report Heatmap](assets/Screenshot%202026-01-20%20140911.png)

The heatmap summarizes key performance metrics:

* **Precision:** ~0.85–0.86 (reliable positive predictions)
* **Recall:** ~0.81–0.88 (good ability to detect disease cases)
* **F1-score:** ~0.83–0.87 (balanced performance)
* **Overall Accuracy:** ~85%

---

## ✅ Conclusion

The Logistic Regression model predicts whether a patient has heart disease based on clinical features. This project is ideal for **machine learning beginners** and **healthcare-based classification problems**.
