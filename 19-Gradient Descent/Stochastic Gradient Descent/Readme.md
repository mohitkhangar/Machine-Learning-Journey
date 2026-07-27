# Stochastic Gradient Descent (SGD)

## Introduction

Gradient Descent is one of the most important optimization algorithms used in Machine Learning to minimize the loss function by updating model parameters.

Instead of using the entire dataset to compute gradients like **Batch Gradient Descent**, **Stochastic Gradient Descent (SGD)** updates the parameters after processing **one training example at a time**.

This makes SGD much faster for large datasets and enables the model to start learning immediately.

---

## What is Stochastic Gradient Descent?

Stochastic Gradient Descent (SGD) is an optimization algorithm in which the model parameters are updated after every single training sample.

Unlike Batch Gradient Descent, which waits until all training examples have been processed, SGD performs an update instantly after computing the error for one sample.

Mathematically,

For each training sample

\[
(x_i,\;y_i)
\]

Update

\[
w=w-\eta\frac{\partial J_i}{\partial w}
\]

\[
b=b-\eta\frac{\partial J_i}{\partial b}
\]

where

- \(w\) = weight
- \(b\) = bias/intercept
- \(\eta\) = learning rate
- \(J_i\) = loss for a single training example

---

## Working of SGD

1. Initialize weights and intercept.
2. Pick one training sample.
3. Predict the output.
4. Calculate the error.
5. Compute gradients.
6. Update weights immediately.
7. Move to the next sample.
8. Repeat until all samples are processed.
9. Continue for multiple epochs.

---

## Algorithm

```text
Initialize weights and bias

Repeat for each epoch

    Shuffle training data

    For each training sample

        Predict output

        Calculate error

        Compute gradients

        Update weights

        Update bias

Return optimized parameters
```

---

## Why Shuffle Data?

Before every epoch, the training data is shuffled so that:

- The model doesn't learn any unwanted order.
- Updates become more random.
- Convergence becomes more stable.

---

## Advantages

- Much faster than Batch Gradient Descent.
- Suitable for very large datasets.
- Can escape shallow local minima because of noisy updates.
- Requires very little memory.
- Supports online learning.

---

## Disadvantages

- Loss function fluctuates heavily.
- Takes an irregular path toward the minimum.
- May require more epochs.
- Sensitive to learning rate.

---

## Batch Gradient Descent vs Stochastic Gradient Descent

| Feature | Batch GD | SGD |
|----------|----------|-----|
| Data used | Entire dataset | One sample |
| Updates | One per epoch | After every sample |
| Speed | Slower | Faster |
| Memory | High | Low |
| Convergence | Smooth | Noisy |
| Suitable for | Small datasets | Large datasets |

---

## Applications

- Linear Regression
- Logistic Regression
- Neural Networks
- Deep Learning
- Large-scale Machine Learning

---

## Files

```text
Stochastic Gradient Descent
│
├── STOCHASTIC GRADIENT DESCENT.ipynb
└── Readme.md
```

---

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

## Learning Outcomes

After completing this notebook, you will understand:

- What SGD is
- Difference between Batch GD and SGD
- Why stochastic updates are faster
- Effect of noisy gradients
- Weight updates after every sample
- Practical implementation of SGD from scratch
