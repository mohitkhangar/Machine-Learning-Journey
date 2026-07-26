# 🚀 Batch Gradient Descent

Batch Gradient Descent is an optimization algorithm used to minimize the cost function by updating the model parameters using the **entire training dataset** in every iteration.

It is one of the most fundamental optimization techniques used in Machine Learning for training Linear Regression models.

---

# 📌 What is Gradient Descent?

Gradient Descent is an optimization algorithm that minimizes the error (cost function) by repeatedly updating the model parameters in the direction of the negative gradient.

The update rule is:

\[
\theta = \theta - \alpha \frac{\partial J}{\partial \theta}
\]

Where:

- θ = Model Parameters
- α = Learning Rate
- J = Cost Function

---

# 📌 What is Batch Gradient Descent?

In Batch Gradient Descent, the gradient is calculated using **all training samples** before updating the weights.

Process:

1. Predict outputs
2. Calculate error
3. Compute gradients using the complete dataset
4. Update weights
5. Repeat until convergence

---

# 📂 Dataset

This notebook uses the **Diabetes Dataset** from Scikit-Learn.

```python
from sklearn.datasets import load_diabetes
```

---

# 📊 Algorithm

Initialize:

- Weights
- Intercept

Repeat for every epoch:

1. Predict values

```python
y_hat = XW + b
```

2. Calculate gradients

```python
intercept_der = -2 * np.mean(y_train - y_hat)

coef_der = -2 * np.dot((y_train - y_hat), X_train) / X_train.shape[0]
```

3. Update parameters

```python
intercept = intercept - lr * intercept_der

weights = weights - lr * coef_der
```

Repeat until convergence.

---

# 📈 Mathematical Formula

Prediction:

\[
\hat{y}=XW+b
\]

Cost Function:

\[
J=\frac{1}{n}\sum(y-\hat y)^2
\]

Gradient for Intercept:

\[
\frac{\partial J}{\partial b}
=
-2\cdot mean(y-\hat y)
\]

Gradient for Coefficients:

\[
\frac{\partial J}{\partial W}
=
-\frac{2}{n}(y-\hat y)^TX
\]

---

# 📚 What I Learned

- Batch Gradient Descent
- Cost Function
- Gradient Calculation
- Weight Updates
- Intercept Updates
- Learning Rate
- Multiple Linear Regression from Scratch
- NumPy Matrix Operations

---

# ⚙️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn

---

# 📁 Files

```
Batch Gradient/
│
├── BATCH GRADIENT DESCENT.ipynb
└── Readme.md
```

---

# 🎯 Future Work

- Stochastic Gradient Descent
- Mini Batch Gradient Descent
- Learning Rate Scheduling
- Gradient Descent Visualization

---

⭐ This notebook is part of my **Machine Learning Journey** where I implement Machine Learning algorithms from scratch to understand the mathematics behind them.
