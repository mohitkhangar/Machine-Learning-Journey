# 📈 Outlier Detection using Percentile Method

This project demonstrates how to identify and handle outliers using the **Percentile Method**. Unlike statistical methods such as Z-Score, the Percentile Method identifies extreme values based on the distribution of the data, making it useful for skewed datasets.

---

## 📖 Overview

Outliers are observations that lie significantly outside the normal range of a dataset. The Percentile Method detects these values by defining lower and upper percentile thresholds.

For example:

- Lower Threshold → 1st or 5th Percentile
- Upper Threshold → 95th or 99th Percentile

Any value outside these limits can be treated as an outlier.

---

## 📂 Files

```
13-Outlier-detection-using-Percentile-Method/
│
├── Percentile Method.ipynb
├── README.md
```

---

## 🛠️ Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📚 Topics Covered

- Introduction to Outliers
- Understanding Percentiles
- Calculating Percentile Values
- Detecting Outliers
- Removing Extreme Values
- Visualizing Data Before and After Outlier Removal

---

## 📊 Workflow

1. Load the dataset.
2. Explore the data distribution.
3. Calculate lower and upper percentile thresholds.
4. Detect observations outside the selected percentile range.
5. Remove or cap outliers.
6. Compare the dataset before and after preprocessing.

---

## 🎯 Common Percentile Thresholds

| Lower Percentile | Upper Percentile | Usage |
|-----------------|------------------|-------|
| 1% | 99% | Extreme outlier detection |
| 5% | 95% | Moderate outlier removal |
| 10% | 90% | Aggressive filtering |

---

## 🚀 Advantages

- Easy to implement
- Works well with skewed data
- Does not assume a normal distribution
- Flexible threshold selection

---

## ⚠️ Limitations

- Threshold selection is subjective
- May remove valid extreme observations
- Can lead to information loss if used aggressively

---

## 📈 Applications

- Financial Data Analysis
- Salary Prediction
- Customer Analytics
- Healthcare Data
- Fraud Detection
- Sales and Revenue Analysis

---

## 🎯 Learning Outcomes

After completing this notebook, you will understand:

- What percentiles are
- How percentile-based outlier detection works
- How to calculate percentile thresholds using Pandas
- How to remove or cap extreme values
- When to prefer the Percentile Method over Z-Score

---

## 🔗 Related Topics

- Z-Score Method
- IQR Method
- Box Plots
- Feature Scaling
- Data Cleaning
- Exploratory Data Analysis (EDA)

---

## 👨‍💻 Author

**Mohit Khangar**

GitHub: https://github.com/mohitkhangar

---

⭐ If you found this notebook helpful, consider starring the repository!
