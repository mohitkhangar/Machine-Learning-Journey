# Polynomial Regression

## Introduction

Polynomial Regression is a supervised machine learning algorithm used to model **non-linear relationships** between the independent variable(s) and the dependent variable.

Unlike Simple Linear Regression, which fits a straight line, Polynomial Regression fits a **curved line (polynomial curve)** to the data, allowing it to capture more complex patterns.

Although it models a non-linear relationship, Polynomial Regression is still considered a **Linear Model** because it is linear with respect to its parameters (coefficients).

---

## What is Polynomial Regression?

Polynomial Regression transforms the original features into higher-degree polynomial features and then applies Linear Regression.

For example,

Instead of fitting

\[
y = b_0 + b_1x
\]

Polynomial Regression fits

\[
y = b_0 + b_1x + b_2x^2 + b_3x^3 + \cdots + b_nx^n
\]

where

- \(y\) = Target variable
- \(x\) = Input feature
- \(b_0\) = Intercept
- \(b_1,b_2,\ldots,b_n\) = Model coefficients

---

## Why Do We Need Polynomial Regression?

Many real-world datasets do not follow a straight-line relationship.

Examples include

- House Prices
- Salary Prediction
- Population Growth
- Temperature Prediction
- Stock Trend Approximation
- Biological Growth Curves

In such cases, a linear model underfits the data, while Polynomial Regression can model the curved relationship more effectively.

---

## Working of Polynomial Regression

1. Collect the dataset.
2. Split the data into training and testing sets.
3. Convert features into polynomial features.
4. Train a Linear Regression model on the transformed features.
5. Predict the target values.
6. Evaluate the model using performance metrics.

---

## Mathematical Representation

### Degree 1

\[
y=b_0+b_1x
\]

### Degree 2

\[
y=b_0+b_1x+b_2x^2
\]

### Degree 3

\[
y=b_0+b_1x+b_2x^2+b_3x^3
\]

### Degree n

\[
y=b_0+b_1x+b_2x^2+\cdots+b_nx^n
\]

---

## Example

Suppose the dataset is

| Experience | Salary |
|------------|--------:|
|1|45000|
|2|50000|
|3|62000|
|4|78000|
|5|98000|

A straight line cannot fit this increasing trend accurately.

Polynomial Regression generates polynomial features

```
x

↓

[x, x², x³]
```

allowing the model to learn the curved relationship.

---

## Advantages

- Captures non-linear relationships.
- Easy to implement using Scikit-learn.
- Higher prediction accuracy for curved datasets.
- Works well for small to medium-sized datasets.

---

## Disadvantages

- Can easily overfit with a high polynomial degree.
- Sensitive to outliers.
- Degree selection is important.
- Less interpretable than Simple Linear Regression.

---

## Choosing the Degree

| Degree | Model Behaviour |
|---------|-----------------|
|1|Linear Regression|
|2|Slight Curve|
|3|Moderate Curve|
|4+|Complex Curve|
|Very High|May Overfit|

---

## Applications

Polynomial Regression is used in

- Salary Prediction
- Sales Forecasting
- Population Growth
- Medical Data Analysis
- Engineering Systems
- Financial Trend Modeling
- Weather Prediction

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
20-Polynomial-Regression
│
├── Polynomial Regression.ipynb
├── Polynomial Regression Part 2.ipynb
└── Readme.md
```

---

## Learning Outcomes

After completing this topic, you will understand

- What Polynomial Regression is.
- Why Linear Regression fails for non-linear data.
- Polynomial Feature Transformation.
- Effect of polynomial degree.
- Overfitting and underfitting.
- Model training using Scikit-learn.
- Visualization of polynomial curves.
- Performance evaluation using regression metrics.

---

## Conclusion

Polynomial Regression is an extension of Linear Regression that models curved relationships by introducing polynomial features. It provides better performance on non-linear datasets while retaining the simplicity of linear models. Selecting an appropriate polynomial degree is essential to achieve a balance between underfitting and overfitting.
