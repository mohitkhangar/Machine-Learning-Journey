# 📦 Outlier Detection using IQR Method

This project demonstrates how to detect and remove outliers using the **Interquartile Range (IQR) Method**. The IQR method is a robust statistical technique that identifies extreme values without assuming a normal distribution, making it ideal for skewed datasets.

---

## 📖 Overview

Outliers are data points that significantly differ from the rest of the observations. The **Interquartile Range (IQR)** measures the spread of the middle 50% of the data and is widely used for outlier detection.

The IQR is calculated as:

\[
IQR = Q3 - Q1
\]

Where:

- **Q1** = First Quartile (25th Percentile)
- **Q3** = Third Quartile (75th Percentile)

Outliers are identified using:

- **Lower Bound = Q1 − 1.5 × IQR**
- **Upper Bound = Q3 + 1.5 × IQR**

---

## 📂 Files

```
15-IQR-Method/
│
├── IQR Method.ipynb
└── README.md
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

- Understanding Quartiles
- Calculating IQR
- Detecting Outliers
- Box Plot Visualization
- Removing Outliers
- Comparing Data Before and After Cleaning

---

## 📊 Workflow

1. Load the dataset.
2. Explore the data distribution.
3. Calculate Q1 and Q3.
4. Compute the Interquartile Range (IQR).
5. Determine lower and upper bounds.
6. Detect outliers.
7. Remove or cap extreme values.
8. Compare the cleaned dataset with the original dataset.

---

## 📐 IQR Formula

```
IQR = Q3 - Q1

Lower Bound = Q1 - 1.5 × IQR
Upper Bound = Q3 + 1.5 × IQR
```

---

## 🚀 Advantages

- Does not assume a normal distribution
- Robust against extreme values
- Easy to understand and implement
- Works well for skewed datasets

---

## ⚠️ Limitations

- May remove valid extreme observations
- Less effective for very small datasets
- Threshold (1.5 × IQR) may need adjustment for specific applications

---

## 📈 Applications

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Financial Data Analysis
- Healthcare Analytics
- Customer Behavior Analysis
- Machine Learning Preprocessing

---

## 🎯 Learning Outcomes

After completing this notebook, you will understand:

- What quartiles and IQR are
- How to calculate the Interquartile Range
- How to detect outliers using the IQR method
- How to remove or cap outliers
- When to use the IQR method instead of Z-Score

---

## 🔗 Related Topics

- Z-Score Method
- Percentile Method
- Box Plots
- Feature Scaling
- Missing Value Handling
- Exploratory Data Analysis (EDA)

---

## 👨‍💻 Author

**Mohit Khangar**

GitHub: https://github.com/mohitkhangar

---

⭐ If you found this notebook helpful, consider starring the repository!
