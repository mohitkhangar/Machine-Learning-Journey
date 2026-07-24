# 📊 Regression Metrics

## 📌 Overview

This project focuses on understanding the most important evaluation metrics used in **Regression Models**. These metrics help measure how well a regression model predicts continuous values and allow us to compare different models.

Understanding regression metrics is essential before moving to optimization techniques like Gradient Descent and advanced machine learning algorithms.

---

## 🎯 Objectives

- Understand how regression models are evaluated
- Learn the difference between various error metrics
- Interpret model performance correctly
- Compare regression models using standard evaluation metrics

---

## 📚 Metrics Covered

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score (Coefficient of Determination)
- Adjusted R² Score

---

## 📖 Metric Descriptions

### 1️⃣ Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted values.

**Formula**

\[
MAE = \frac{1}{n}\sum |y_i-\hat{y_i}|
\]

**Advantages**

- Easy to understand
- Less sensitive to outliers

---

### 2️⃣ Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted values.

**Formula**

\[
MSE=\frac{1}{n}\sum (y_i-\hat{y_i})^2
\]

**Advantages**

- Penalizes large errors heavily
- Smooth and differentiable
- Used as the Cost Function in Linear Regression

---

### 3️⃣ Root Mean Squared Error (RMSE)

Square root of Mean Squared Error.

**Formula**

\[
RMSE=\sqrt{MSE}
\]

**Advantages**

- Same unit as the target variable
- Easier to interpret than MSE

---

### 4️⃣ R² Score

Measures how well the regression model explains the variance in the target variable.

**Range**

- 1 → Perfect Fit
- 0 → Model performs like predicting the mean
- Negative → Poor model

---

### 5️⃣ Adjusted R² Score

An improved version of R² Score that penalizes unnecessary features.

Useful in **Multiple Linear Regression**.

---

## 📂 Libraries Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

## 📈 Learning Outcomes

After completing this project, I learned:

- How to evaluate regression models
- Difference between MAE, MSE, and RMSE
- Why Linear Regression uses MSE as its Cost Function
- How to interpret R² Score
- When to use Adjusted R² Score

---

## 🚀 Future Scope

The concepts learned here form the foundation for:

- Gradient Descent
- Batch Gradient Descent
- Stochastic Gradient Descent
- Mini Batch Gradient Descent
- Polynomial Regression
- Regularization Techniques
- Deep Learning Loss Functions

---

## ⭐ Author

**Mohit Khangar**

Machine Learning Journey 🚀
