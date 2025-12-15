# Single Variable Linear Regression
This project implements single variable linear regression to predict a target value from one input feature, demonstrating data preprocessing, model training, evaluation, and visualization of results.

## 1️⃣ Data Preprocessing
1. Importing required libraries
2. Seperating the feature variable and dependent variable
    1. Feature variable (X)   = Years of Experience
    2. Dependent variable (y) = Salary
3. Spliting the dataset into training set and testing set.

## 2️⃣ Training the model
1. Make an instance for the linear regression model.
2. Train the model with X_train and y_train.

## 3️⃣ Predict any data
```
print(regressor.predict([[12]]))   # Change the data for predicting salary
```

## 4️⃣ Visualizing the train set
![Training Set Result](assets/images/train_set.png)

## 5️⃣ Visualizing the test set
![Test Set Result](assets/images/test_set.png)

**Successfully trained and predicted using linear regression model on single feature variable 🏆**