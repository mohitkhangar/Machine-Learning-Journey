# 🚀 Gradient Descent from Scratch

## 📌 Overview

This project demonstrates how **Gradient Descent** works by implementing **Simple Linear Regression from scratch** using Python and NumPy, without relying on Scikit-learn's `LinearRegression` model.

Instead of using a built-in algorithm, the model learns the optimal **weight (m)** and **bias (b)** by minimizing the Mean Squared Error (MSE) using Gradient Descent.

This implementation helps in understanding the mathematics behind how machine learning models learn from data.

---

## 🎯 Objectives

- Understand the working of Gradient Descent.
- Implement Linear Regression without Scikit-learn.
- Learn how model parameters are updated iteratively.
- Visualize the learning process.
- Compare the custom implementation with Scikit-learn.

---

## 📚 Concepts Covered

- Simple Linear Regression
- Gradient Descent
- Cost Function (Mean Squared Error)
- Learning Rate
- Epochs
- Weight (Slope)
- Bias (Intercept)
- Model Training
- Prediction
- R² Score Evaluation

---

## 🛠 Libraries Used

- NumPy
- Matplotlib
- Scikit-learn (Dataset & Evaluation Only)

---

## 📂 Dataset

A synthetic regression dataset is generated using:

```python
from sklearn.datasets import make_regression
```

Dataset Configuration:

- Samples: 100
- Features: 1
- Informative Features: 1
- Noise: 20
- Random State: 13

The dataset is then divided into training and testing sets using `train_test_split`.

---

## ⚙️ Workflow

1. Generate a regression dataset.
2. Visualize the data.
3. Split the dataset into training and testing sets.
4. Create a custom `GDRegressor` class.
5. Initialize weight and bias.
6. Compute gradients.
7. Update parameters using Gradient Descent.
8. Repeat for multiple epochs.
9. Predict test data.
10. Evaluate using the R² Score.

---

## 🧠 Gradient Descent Equations

### Weight Update

```text
m = m - α × (∂Loss/∂m)
```

### Bias Update

```text
b = b - α × (∂Loss/∂b)
```

Where:

- **m** = Slope (Weight)
- **b** = Bias (Intercept)
- **α** = Learning Rate

---

## 🏗 Custom Model

A custom class named **GDRegressor** is implemented with:

- `__init__()`
- `fit()`
- `predict()`

The `fit()` method updates the model parameters using Gradient Descent, while `predict()` generates predictions for new data.

---

## 📊 Model Evaluation

The model performance is evaluated using the **R² Score**.

```text
Example R² Score:

0.63
```

(The exact value may vary depending on random initialization and hyperparameters.)

---

## 📈 Learning Process

During each epoch:

- Predict output using current parameters.
- Compute gradients.
- Update slope and bias.
- Reduce prediction error.
- Move closer to the optimal regression line.

This iterative optimization is the core idea behind Gradient Descent.

---

## 📁 Files Included

- Gradient Descent from Scratch Notebook
- Custom GDRegressor Implementation
- Dataset Generation
- Data Visualization
- Model Training
- Prediction
- Performance Evaluation

---

## 🎓 Learning Outcomes

After completing this project, you will be able to:

- Understand the mathematics behind Gradient Descent.
- Implement Linear Regression from scratch.
- Build your own machine learning algorithm.
- Update model parameters using derivatives.
- Evaluate regression models using the R² Score.
- Appreciate how optimization algorithms train machine learning models.

---

## 🔮 Future Improvements

- Add Cost Function visualization.
- Plot Loss vs Epochs.
- Implement Batch Gradient Descent.
- Implement Stochastic Gradient Descent (SGD).
- Implement Mini-Batch Gradient Descent.
- Add Early Stopping.
- Compare results with Scikit-learn's `LinearRegression`.

---

## ⭐ Key Takeaway

Building Gradient Descent from scratch provides a deeper understanding of how machine learning models optimize their parameters. This project serves as a strong foundation for learning advanced algorithms such as Logistic Regression, Neural Networks, and Deep Learning.

---

⭐ **Difficulty:** Intermediate

🏷️ **Tags:** Machine Learning, Gradient Descent, Linear Regression, Optimization, NumPy, Python, From Scratch
