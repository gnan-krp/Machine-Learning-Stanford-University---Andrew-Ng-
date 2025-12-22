# Machine Learning – Linear Regression (Model 1)
*Notes from Andrew Ng’s Coursera/Stanford Lecture

---

## 1. Goal of This Lecture
- Introduce the **first machine learning model**: **linear regression** with one variable.
- Focus on **supervised learning** – learning from labeled data.
- Learn to predict continuous outputs from input features.

---

## 2. Supervised Learning Overview
- Supervised learning uses a **training set** of examples with known inputs and outputs.
- Goal: Learn a relationship between **inputs (x)** and **outputs (y)** to predict new data.
- Example: Predict house prices based on house size.

---

## 3. Example Problem: Housing Prices
- Task: Predict **house prices** based on **size of the house** (square feet).
- Sample training data:

| Size (x) | Price (y) |
|-----------|-----------|
| 852       | 178       |
| 1416      | 232       |
| 1534      | 315       |
| 2104      | 460       |

- Number of training examples: \(m\)

---

## 4. Notation
- \(x\) = input feature (e.g., house size)
- \(y\) = target/output (e.g., house price)
- Training example: \((x^{(i)}, y^{(i)})\), where \(i\) indexes the example.

---

## 5. Hypothesis
- A **hypothesis** \(h\) is a function that maps **inputs to predicted outputs**.
- For a new house with size \(x\), the predicted price is \(h(x)\).

---

## 6. Linear Model Representation
- Assume a linear relationship between input \(x\) and output \(y\):
\[
h_\theta(x) = \theta_0 + \theta_1 x
\]

- Where:
  - \(\theta_0\) = intercept (where the line crosses the y-axis)
  - \(\theta_1\) = slope (how much y changes with x)

---

## 7. Why Linear Model?
- Linear function is the **simplest assumption** to model the relationship.
- Serves as a **baseline** before exploring more complex models.

---

## 8. Summary
- **Supervised learning** uses labeled training data.
- A training example: \((x^{(i)}, y^{(i)})\)
- Hypothesis: \(h_\theta(x) = \theta_0 + \theta_1 x\)
- Parameters \(\theta_0, \theta_1\) define model predictions.
- Linear regression predicts a continuous variable from a single feature.

---

