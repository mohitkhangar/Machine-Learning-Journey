# 📉 Gradient Descent

## 📌 Overview

Gradient Descent is one of the most important optimization algorithms in Machine Learning. It is used to minimize the loss (cost) function by iteratively updating model parameters in the direction of the negative gradient.

Almost every machine learning algorithm that learns parameters—such as Linear Regression, Logistic Regression, and Neural Networks—uses Gradient Descent or one of its variants.

---

## 🎯 Objectives

- Understand why optimization is required.
- Learn the intuition behind Gradient Descent.
- Understand the role of the Cost Function.
- Learn how weights and bias are updated.
- Visualize how Gradient Descent reaches the minimum point.
- Study the effect of the Learning Rate.

---

## 📚 Concepts Covered

- Optimization
- Cost Function
- Gradient
- Derivatives
- Learning Rate (α)
- Weight Update Rule
- Bias Update Rule
- Convergence
- Local vs Global Minimum
- Batch Gradient Descent
- Stochastic Gradient Descent (SGD)
- Mini-Batch Gradient Descent

---

## 🧠 Intuition

Imagine standing on top of a hill while blindfolded.

Your goal is to reach the lowest point of the hill.

You take one small step at a time in the direction where the slope decreases the most.

Eventually, you reach the bottom.

Gradient Descent works in exactly the same way—it repeatedly updates the model parameters until the cost function reaches its minimum value.

---

## 📐 Gradient Descent Formula

### Weight Update

```text
w = w - α × (∂J/∂w)
```

### Bias Update

```text
b = b - α × (∂J/∂b)
```

Where:

- **w** = Weight
- **b** = Bias
- **α** = Learning Rate
- **J** = Cost Function

---

## 🚀 Workflow

1. Initialize weights and bias.
2. Make predictions.
3. Calculate the cost (loss).
4. Compute gradients.
5. Update weights and bias.
6. Repeat until convergence.

---

## 📊 Types of Gradient Descent

### Batch Gradient Descent

- Uses the entire dataset.
- Stable updates.
- Slower for large datasets.

### Stochastic Gradient Descent (SGD)

- Uses one training example at a time.
- Faster updates.
- More noisy.

### Mini-Batch Gradient Descent

- Uses small batches of data.
- Balances speed and stability.
- Most commonly used in practice.

---

## ⚙️ Learning Rate

The learning rate controls the size of each update.

- Very Small Learning Rate
  - Slow convergence.
- Very Large Learning Rate
  - May overshoot the minimum.
- Optimal Learning Rate
  - Faster and stable convergence.

---

## 🛠 Libraries Used

- NumPy
- Matplotlib
- Scikit-learn

---

## 📈 Applications

Gradient Descent is used in:

- Linear Regression
- Logistic Regression
- Neural Networks
- Deep Learning
- Recommendation Systems
- Computer Vision
- Natural Language Processing

---

## 🎓 Learning Outcomes

After completing this module, you will be able to:

- Explain why Gradient Descent is required.
- Understand how machine learning models learn from data.
- Update weights using gradient calculations.
- Differentiate between Batch, SGD, and Mini-Batch Gradient Descent.
- Choose an appropriate learning rate.
- Understand the optimization process used in modern machine learning algorithms.

---

## 📂 Files Included

- Gradient Descent Theory
- Mathematical Explanation
- Python Implementation
- Visualizations
- Practice Examples

---

⭐ This module forms the foundation for understanding how machine learning and deep learning models are trained.
