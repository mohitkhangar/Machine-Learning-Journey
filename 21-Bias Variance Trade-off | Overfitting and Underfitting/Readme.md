# Bias-Variance Trade-off | Overfitting and Underfitting

## Introduction

One of the biggest challenges in Machine Learning is building a model that performs well on both training data and unseen data.

A model should neither memorize the training data nor be too simple to learn useful patterns. This balance is achieved through the **Bias-Variance Trade-off**.

Understanding bias, variance, overfitting, and underfitting is essential for developing robust machine learning models.

---

## What is Bias?

Bias is the error introduced because the model makes simplifying assumptions about the data.

A model with **high bias** is too simple and cannot capture the underlying relationship in the dataset.

Characteristics:

- Oversimplifies the data
- High training error
- High testing error
- Leads to Underfitting

---

## What is Variance?

Variance measures how much a model changes when trained on different datasets.

A model with **high variance** learns even the noise present in the training data.

Characteristics:

- Fits the training data extremely well
- Very low training error
- High testing error
- Leads to Overfitting

---

## Bias vs Variance

| Bias | Variance |
|------|----------|
| Simple model | Complex model |
| Underfits data | Overfits data |
| High training error | Low training error |
| High testing error | High testing error |
| Stable predictions | Sensitive predictions |

---

# Underfitting

## What is Underfitting?

Underfitting occurs when the model is too simple to capture the underlying relationship between features and the target variable.

The model performs poorly on both training and testing datasets.

### Characteristics

- High Bias
- Low Variance
- Poor Accuracy
- Cannot learn patterns

---

## Example

Trying to fit a straight line to highly curved data.

```
Curved Data

       ●

    ●

  ●

●

-------------------------
Straight Line
```

The model cannot represent the actual relationship.

---

## Causes of Underfitting

- Very simple model
- Insufficient training
- Too few features
- Excessive regularization

---

## How to Reduce Underfitting?

- Increase model complexity
- Add more features
- Train for more epochs
- Reduce regularization

---

# Overfitting

## What is Overfitting?

Overfitting occurs when a model learns not only the actual pattern but also the noise present in the training data.

The model performs extremely well on training data but poorly on unseen data.

### Characteristics

- Low Bias
- High Variance
- Excellent Training Accuracy
- Poor Testing Accuracy

---

## Example

A very high-degree polynomial passing through every training point.

```
●~~~~●~~●~~~~●~~~~●

Training Data

Model memorizes every point
```

---

## Causes of Overfitting

- Complex model
- Too many features
- Small dataset
- Training for too many epochs
- No regularization

---

## How to Reduce Overfitting?

- Collect more training data
- Feature Selection
- Regularization (L1/L2)
- Cross Validation
- Early Stopping
- Reduce model complexity
- Pruning (Decision Trees)
- Dropout (Neural Networks)

---

# Bias-Variance Trade-off

The goal of Machine Learning is to achieve the perfect balance between Bias and Variance.

```
High Bias
      ↓
Underfitting

------------ Best Model ------------

High Variance
      ↓
Overfitting
```

An ideal model has

- Low Bias
- Low Variance
- Good Generalization

---

## Training vs Testing Error

| Model | Training Error | Testing Error |
|--------|----------------|---------------|
| Underfitting | High | High |
| Good Fit | Low | Low |
| Overfitting | Very Low | High |

---

## Real-Life Example

Suppose you are preparing for an exam.

### Underfitting

You study only one chapter.

Result:

- Poor performance everywhere.

### Good Fit

You study all important topics.

Result:

- Good performance.

### Overfitting

You memorize only previous year's questions.

Result:

- Excellent if the same questions appear.
- Poor if new questions are asked.

This is exactly how machine learning models behave.

---

## Applications

Understanding the Bias-Variance Trade-off is important in

- Linear Regression
- Polynomial Regression
- Decision Trees
- Random Forest
- Support Vector Machines
- Neural Networks
- Deep Learning

---

## Techniques to Balance Bias and Variance

- Cross Validation
- Regularization
- Ensemble Learning
- Bagging
- Boosting
- Feature Engineering
- Hyperparameter Tuning

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Folder Structure

```text
21-Bias Variance Trade-off | Overfitting and Underfitting
│
├── Bias Variance Tradeoff.ipynb
├── Underfitting vs Overfitting.ipynb
└── Readme.md
```

---

## Learning Outcomes

After completing this topic, you will understand:

- What is Bias
- What is Variance
- Difference between Bias and Variance
- What is Underfitting
- What is Overfitting
- Training vs Testing Error
- Bias-Variance Trade-off
- Techniques to improve model generalization

---

## Conclusion

Bias and Variance are two fundamental sources of error in Machine Learning.

A model with **high bias** underfits the data, while a model with **high variance** overfits the data.

The objective is to build a model that achieves the right balance between bias and variance, resulting in good performance on both training and unseen data.
