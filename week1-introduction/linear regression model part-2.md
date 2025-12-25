# Supervised Learning & Linear Regression (Model Representation)

These notes are based on the **Andrew Ng Machine Learning course** and explain:
- How supervised learning works
- What a model is
- Linear regression with one variable
- Model representation using a straight line

---

## 1. What is Supervised Learning?

In **supervised learning**, the algorithm learns from a **training set** that contains:

- **Input features (x)** → example: size of a house
- **Output targets (y)** → example: price of the house

The output targets are the **correct answers** the model learns from.

---

Training Set
(x, y)
   ↓
Learning Algorithm
   ↓
Model f(x)
   ↓
Prediction ŷ

## 2. Training Set in Supervised Learning

A training set contains **pairs of inputs and outputs**:

(x₁, y₁)
(x₂, y₂)
(x₃, y₃)
...


Example:
- x = house size
- y = house price

---

Price (y)
  ^
  |            ●
  |         ●
  |      ●
  |   ●
  |●
  +-----------------------------> Size (x)


## 3. What Does the Learning Algorithm Do?

### Input:
- Training data (x, y)

### Output:
- A **function** called the **model**

This function learns a relationship between input and output.

---

y
^
|            /
|          /
|        /
|      /
|____/________________> x
     b        slope = w


## 4. The Model (Function f)

The learning algorithm produces a function called **f**.

- f is called the **model**
- It takes input **x**
- It outputs a prediction **ŷ (y-hat)**

### Notation:
- **x** → input feature
- **y** → actual target value
- **ŷ (y-hat)** → predicted value

---

Price (y)
  ^
  |            ●
  |         ●
  |      ●
  |   ●
  |●
  +-----------------------------> Size (x)
           Learned line f(x)=wx+b


## 5. Meaning of y vs y-hat

| Symbol | Meaning |
|------|--------|
| y | True value (known in training set) |
| ŷ | Predicted value (estimated by model) |

Example:
- True house price → y (unknown until sold)
- Predicted price → ŷ (estimated by model)

---

Actual value (y):        ●
Predicted value (ŷ):     ×

Error = |y - ŷ|


## 6. Model Representation (Linear Function)

We represent the model as a **straight line**:

f(x) = wx + b


Where:
- **w** → slope (weight)
- **b** → intercept (bias)
- **x** → input feature
- **f(x)** → predicted output (ŷ)

This is also written as:

f_w,b(x) = wx + b


---

Cost J(w,b)
  ^
  |        *
  |     *
  |   *
  | *
  |*______________> w
       Minimum


## 7. Graphical Representation

Training data plotted on a graph:

Cost J(w,b)
  ^
  |        *
  |     *
  |   *
  | *
  |*______________> w
       Minimum


- Dots → training examples
- Line → learned model

---

## 8. Why Use a Linear Function?

Reasons:
- Simple
- Easy to understand
- Easy to compute
- Good foundation for complex models

More complex models (curves, parabolas) can be used later.

---

## 9. Linear Regression

This model is called **Linear Regression**.

Specifically:
- **Linear regression with one variable**
- Also called **Univariate Linear Regression**

### Meaning:
- **Uni** → one
- **Variate** → variable

Only **one input feature (x)** is used.

---

## 10. Example of Univariate Linear Regression

Input:
- House size

Output:
- House price

Model:

Price = w × Size + b


---

## 11. Multiple Features (Future Topic)

Later, regression can use multiple inputs:
- Size
- Number of bedrooms
- Location
- Age of house

This is called **multivariate linear regression**.

---

## 12. Optional Lab (Mentioned in Video)

- Python lab to define a straight-line function
- Allows changing values of **w** and **b**
- Helps visualize predictions

(No coding required, only experimentation)

---

## 13. Why Cost Function is Needed

The model must know:
- How good or bad its predictions are

This is done using a **cost function**.

### Purpose:
- Measure prediction error
- Guide the model to improve

---

## 14. Key Learning Summary

- Supervised learning uses labeled data
- Model = function f
- Input → x
- Output → ŷ (prediction)
- Linear regression uses a straight line
- Univariate = one input variable
- Cost function is essential for learning

---

## Course Reference

- Stanford University – Andrew Ng  
- Machine Learning (Week 1)  
- IBM SkillsBuild AI Fundamentals (Aligned Concepts)

---

## Author

**Gnan Parekh**  
IT Student | Machine Learning Learner
