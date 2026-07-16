# 📊 Outlier Detection and Removal using Z-Score Method

This project demonstrates how to detect and remove outliers from a dataset using the **Z-Score Method**. Outlier detection is an important preprocessing step in Machine Learning as it helps improve model performance by removing extreme values.

---

## 📖 What is an Outlier?

An **outlier** is a data point that differs significantly from other observations. Outliers may occur due to:

- Data entry errors
- Measurement errors
- Experimental errors
- Genuine rare events

Removing unnecessary outliers often improves the quality of the dataset.

---

## 📐 Z-Score Formula

The Z-score measures how many standard deviations a data point is away from the mean.

\[
Z = \frac{x-\mu}{\sigma}
\]

Where:

- **x** = Data point
- **μ** = Mean of the feature
- **σ** = Standard deviation

---

## 🎯 Rule

Generally,

- **|Z| < 3** → Normal observation
- **|Z| > 3** → Outlier

---

## 📂 Files

```
12-Outlier Detection and Removal using Z-score Method/
│
├── Z Score Method.ipynb
├── placement.csv
└── README.md
```

---

## 🛠️ Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

---

## 📊 Workflow

1. Load the dataset.
2. Visualize the data distribution.
3. Calculate mean and standard deviation.
4. Compute the Z-score for each observation.
5. Identify observations with |Z| > 3.
6. Remove outliers.
7. Compare the dataset before and after removal.

---

## 📈 Advantages

- Easy to understand
- Fast computation
- Works well for normally distributed data
- Widely used in statistical analysis

---

## ⚠️ Limitations

- Assumes data follows a normal distribution.
- Not suitable for highly skewed datasets.
- Sensitive to extreme values since mean and standard deviation are affected by outliers.

---

## 📚 Learning Outcomes

After completing this notebook, you will understand:

- What outliers are
- Why outlier detection is important
- How the Z-Score method works
- How to remove outliers using Python
- When to use the Z-Score technique

---

## 🚀 Next Steps

You can compare the Z-Score method with:

- IQR (Interquartile Range)
- Percentile Method
- Isolation Forest
- DBSCAN
- Local Outlier Factor (LOF)

---

## 👨‍💻 Author

**Mohit Khangar**

GitHub: https://github.com/mohitkhangar

---

⭐ If you found this notebook useful, consider starring the repository!
