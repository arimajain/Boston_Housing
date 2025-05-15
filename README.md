# 🏠 Linear Regression on Boston Housing Dataset

This project demonstrates a **Linear Regression** model applied to the **Boston Housing Dataset** to predict housing prices based on 13 features. The implementation uses Python and Scikit-learn, making it ideal for beginners learning machine learning and data science concepts.

---

## 📘 Dataset Overview

- **Name:** Boston Housing Dataset
- **Source:** Originally from the StatLib library, maintained by Carnegie Mellon University.
- **Size:** 506 instances with 13 input features and 1 target variable (housing price).
- **Target Variable:** Median value of owner-occupied homes in $1000s.

---

## 🛠 Features in the Dataset

The dataset includes the following features (independent variables):

- `CRIM`: Per capita crime rate by town
- `ZN`: Proportion of residential land zoned for lots over 25,000 sq.ft.
- `INDUS`: Proportion of non-retail business acres per town
- `CHAS`: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
- `NOX`: Nitric oxides concentration (parts per 10 million)
- `RM`: Average number of rooms per dwelling
- `AGE`: Proportion of owner-occupied units built prior to 1940
- `DIS`: Weighted distances to five Boston employment centres
- `RAD`: Index of accessibility to radial highways
- `TAX`: Full-value property-tax rate per $10,000
- `PTRATIO`: Pupil-teacher ratio by town
- `B`: 1000(Bk - 0.63)^2 where Bk is the proportion of Black residents by town
- `LSTAT`: % lower status of the population

Target variable:
- `MEDV`: Median value of owner-occupied homes in $1000s

---

## 🔍 Project Steps

1. **Import Libraries & Dataset**
   - Use `fetch_openml` from `sklearn.datasets` to load the data.

2. **Explore & Prepare Data**
   - Convert ndarray to DataFrame
   - Append the `Price` (target) column
   - Display summary stats and dataset info

3. **Split the Data**
   - Use `train_test_split` to divide into training and testing sets (80/20 split)

4. **Train the Model**
   - Apply `LinearRegression` from Scikit-learn
   - Fit the model using training data

5. **Evaluate the Model**
   - Predict on the test set
   - Plot predicted vs actual values
   - Calculate Mean Squared Error (MSE) and Mean Absolute Error (MAE)

---

## 📊 Results

- **Mean Squared Error (MSE):** ~33.45  
- **Mean Absolute Error (MAE):** ~3.84  
- **Approximate Model Accuracy:** ~66.55%

> The model has moderate performance. It can be improved using more advanced models such as Random Forest, XGBoost, or by feature engineering and hyperparameter tuning.

---

## 📈 Visualization

A scatter plot is generated to visually compare the actual vs predicted housing prices:

- **X-axis:** True price
- **Y-axis:** Predicted price
- **Color:** Green points represent predictions

---
