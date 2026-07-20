# 🧹 Handling Missing Data using Mean and Mode Imputation (SimpleImputer)

## 📌 Overview

Missing values are one of the most common problems in real-world datasets. Most Machine Learning algorithms cannot work directly with missing data, so it is important to handle them before training a model.

In this project, I learned how to use **SimpleImputer** from **Scikit-learn** to replace missing values using:

- Mean Imputation (for numerical features)
- Mode (Most Frequent) Imputation (for categorical features)

---

## 🎯 Objectives

- Understand why missing values occur.
- Learn different strategies for handling missing data.
- Apply Mean Imputation to numerical columns.
- Apply Mode Imputation to categorical columns.
- Use Scikit-learn's `SimpleImputer`.
- Prepare clean data for Machine Learning models.

---

## 📂 Dataset

The dataset contains missing values in both numerical and categorical features.

Examples:
- Age
- Salary
- Gender
- Purchased

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

---

## 📚 Concepts Covered

### Mean Imputation
Used for numerical columns.

Example:

Before

```
Age
22
25
NaN
30
28
```

After

```
Age
22
25
26.25
30
28
```

The missing value is replaced by the **average** of the column.

---

### Mode Imputation

Used for categorical columns.

Before

```
City

Delhi
Mumbai
NaN
Delhi
```

After

```
City

Delhi
Mumbai
Delhi
Delhi
```

The missing value is replaced by the **most frequent value**.

---

## 💻 Implementation

This notebook demonstrates:

- Loading the dataset
- Detecting missing values
- Applying Mean Imputation
- Applying Mode Imputation
- Transforming the dataset using `SimpleImputer`

---

## 📈 Libraries Used

```python
import pandas as pd
import numpy as np

from sklearn.impute import SimpleImputer
```

---

## 📖 What I Learned

- Importance of handling missing values.
- Difference between Mean and Mode Imputation.
- When to use each strategy.
- How `SimpleImputer` works internally.
- Preparing datasets before feature engineering and model training.

---

## 🚀 Future Improvements

- Median Imputation
- Constant Value Imputation
- KNN Imputer
- Iterative Imputer
- Missing Indicator Features

---

## 📚 References

- Scikit-learn Documentation
- Pandas Documentation

---

⭐ This project is part of my **Machine Learning Journey**, where I document every preprocessing technique, algorithm, and practical implementation while learning Machine Learning from scratch.
