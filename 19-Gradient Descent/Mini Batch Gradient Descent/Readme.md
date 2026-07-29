# Mini Batch Gradient Descent

## Introduction

Gradient Descent is one of the most widely used optimization algorithms in Machine Learning. It minimizes the loss function by iteratively updating the model parameters.

**Mini Batch Gradient Descent** combines the advantages of **Batch Gradient Descent** and **Stochastic Gradient Descent** by updating the model parameters using a small batch of training samples instead of the entire dataset or a single sample.

It is the most commonly used optimization technique in modern Machine Learning and Deep Learning because it provides a good balance between computational efficiency and stable convergence.

---

## What is Mini Batch Gradient Descent?

Mini Batch Gradient Descent divides the training dataset into small batches (for example, 32, 64, or 128 samples).

Instead of updating the weights after processing the entire dataset (Batch GD) or after every single sample (SGD), the model updates its parameters after processing one mini batch.

Mathematically,

For each mini batch,

\[
w = w - \eta \frac{\partial J_{batch}}{\partial w}
\]

\[
b = b - \eta \frac{\partial J_{batch}}{\partial b}
\]

where

- **w** = weight
- **b** = bias/intercept
- **η** = learning rate
- **Jbatch** = Loss computed over one mini batch

---

## Working of Mini Batch Gradient Descent

1. Initialize weights and bias.
2. Shuffle the training dataset.
3. Divide the dataset into mini batches.
4. Select one mini batch.
5. Predict outputs for the batch.
6. Compute the batch loss.
7. Calculate gradients.
8. Update weights and bias.
9. Repeat for every mini batch.
10. Continue for multiple epochs until convergence.

---

## Algorithm

```text
Initialize weights and bias

Repeat for each epoch

    Shuffle the dataset

    Divide data into mini batches

    For each mini batch

        Predict output

        Compute loss

        Calculate gradients

        Update weights

        Update bias

Return optimized parameters
```

---

## Why Use Mini Batches?

Mini batches provide the benefits of both Batch Gradient Descent and Stochastic Gradient Descent.

- Faster than Batch Gradient Descent.
- More stable than Stochastic Gradient Descent.
- Better utilization of CPU/GPU hardware.
- Efficient memory usage.
- Faster convergence for large datasets.

---

## Advantages

- Faster training.
- Stable convergence.
- Efficient memory usage.
- Better GPU utilization.
- Reduces noisy updates.
- Most widely used optimization technique.

---

## Disadvantages

- Choosing an appropriate batch size can be difficult.
- Very small batches behave like SGD.
- Very large batches behave like Batch Gradient Descent.
- Performance depends on learning rate and batch size.

---

## Choosing Batch Size

Common mini batch sizes are

```text
16
32
64
128
256
```

Generally,

- Smaller batch → Faster updates but noisier gradients.
- Larger batch → More stable gradients but slower updates.

---

## Batch vs Stochastic vs Mini Batch Gradient Descent

| Feature | Batch GD | Stochastic GD | Mini Batch GD |
|----------|-----------|---------------|----------------|
| Data Used | Entire dataset | One sample | Small batch |
| Updates | One per epoch | One per sample | One per batch |
| Speed | Slow | Fast | Moderate |
| Memory Usage | High | Low | Medium |
| Convergence | Smooth | Noisy | Stable |
| GPU Friendly | ❌ | ❌ | ✅ |
| Most Used | Rarely | Sometimes | ✅ Yes |

---

## Applications

Mini Batch Gradient Descent is widely used in

- Linear Regression
- Logistic Regression
- Neural Networks
- Deep Learning
- Convolutional Neural Networks (CNN)
- Recurrent Neural Networks (RNN)
- Transformers

---

## Files

```text
Mini Batch Gradient Descent
│
├── MINI BATCH GRADIENT DESCENT.ipynb
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

- What Mini Batch Gradient Descent is
- Difference between Batch, SGD and Mini Batch GD
- Why mini batches improve training efficiency
- Effect of batch size on convergence
- Weight updates using mini batches
- Practical implementation from scratch
- Why Mini Batch Gradient Descent is the standard optimizer for Deep Learning

---

## Conclusion

Mini Batch Gradient Descent is the most popular optimization algorithm used in Machine Learning and Deep Learning because it combines the stability of Batch Gradient Descent with the speed of Stochastic Gradient Descent.

It provides efficient computation, stable convergence, and excellent scalability, making it the preferred optimization method for training modern machine learning models.
