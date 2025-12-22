# Machine Learning – Linear Regression (Model 1)
*Notes from Andrew Ng’s Coursera/Stanford Lecture – First 10 minutes*

---

## 1. Goal of This Lecture
- Introduce the **first machine learning model**: **linear regression** with one variable.
- Focus on **supervised learning** – learning from labeled data.

---

## 2. Supervised Learning Overview
- Supervised learning uses a **training set** of examples with known inputs and outputs.
- Goal: Learn a relationship between **inputs (x)** and **outputs (y)** to predict new data.

---

## 3. Example Problem: Housing Prices
- Task: Predict **house prices** based on **size of the house** (square feet).
- Sample training data:

| Size (x) | Price (y) |
|-----------|-----------|
| 2104      | 460       |
| 1416      | 232       |
| 1534      | 315       |
| 852       | 178       |

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

## 8. Important Notes
- This lecture **does not cover**:
  - Cost function
  - How to choose \(\theta_0, \theta_1\)
- These are introduced in later videos.

---

## 9. Summary
- **Supervised learning** uses labeled training data.
- A training example: \((x^{(i)}, y^{(i)})\)
- Hypothesis: \(h_\theta(x) = \theta_0 + \theta_1 x\)
- Parameters \(\theta_0, \theta_1\) define model predictions.
- This lecture covers **model representation only**.

---

## 10. Graph: Linear Regression Model (Proportional)

```mermaid
%% Proportional Linear Regression Graph
%% x-axis: House Size, y-axis: Price
%% Blue points: Training data
%% Red line: Hypothesis hθ(x) = θ₀ + θ₁x

graph TD
    %% Styling
    classDef axis fill:#fff,stroke:#000,stroke-width:2px;
    classDef point fill:#1f77b4,stroke:#1f77b4,color:#fff,stroke-width:1px;
    classDef line fill:none,stroke:#f00,stroke-width:2px;

    %% Axes
    axisY[Price (y)]:::axis
    axisX[Size (x)]:::axis

    %% Training points
    P1["(2104,460)"]:::point
    P2["(1416,232)"]:::point
    P3["(1534,315)"]:::point
    P4["(852,178)"]:::point

    %% Hypothesis line (illustrative)
    L["hθ(x) = θ₀ + θ₁x"]:::line

    %% Connect line to points (illustrative)
    L --- P1
    L --- P2
    L --- P3
    L --- P4
