# Supervised Learning Notes

## 1. Supervised Learning

Supervised learning is a type of machine learning where the algorithm learns **input-to-output mappings**.  

   x  ----------->  y
input  -----------> output


We provide the algorithm with examples that have the **correct output (y)** for each input (x). After practicing on many such examples, the algorithm learns to predict the output y for **new inputs x**, even if the correct output is unknown.  

These predictions can be used to make precautionary or informed decisions for the future.

---

## Examples of Supervised Learning

| Input (x)             | Output (y)                 | Application                    |
|-----------------------|----------------------------|--------------------------------|
| Email                 | Spam (0 or 1)             | Spam Filtering                 |
| Audio                 | Text scripts              | Speech Recognition             |
| English               | Spanish                   | Machine Translation            |
| Ad, user info         | Click (0 or 1)            | Online Advertising             |
| Image, radar info     | Position of other cars    | Self-Driving Cars              |
| Image of phone        | Defect? (0 or 1)          | Visual Inspection              |

---

## 2. Types of Supervised Learning

1. **Classification Supervised Learning**  
2. **Regression Supervised Learning**

---

## 2.1 Classification Supervised Learning

In classification, the algorithm predicts **discrete outputs**.  

#### Example: Breast Cancer Detection  

Dataset: Tumor labeled as **benign (0)** or **malignant (1)** based on tumor size:

| Tumor Size (cm) | Diagnosis |
|-----------------|-----------|
| 2               | 0         |
| 5               | 1         |
| 1               | 0         |
| 7               | 1         |

#### Graphical Representation

Tumor Diagnosis vs Tumor Size
Diagnosis
1 │        █         █
  │
0 │  █         █
  │
  └────────────────────────
      1   2   3   5   7
         Tumor Size (cm)


**Explanation:**  
- Algorithm is trained on labeled data to predict if a tumor is benign (0) or malignant (1).  
- Once trained, it predicts for new inputs without knowing the correct output.  

**Applications:** Diagnostic tools, spam detection, image classification, etc.

---

## 2.2 Regression Supervised Learning

In regression, the algorithm predicts **continuous outputs**.  

#### Example: Predicting House Prices

| House Size (ft²) | Price ($1000s) |
|-----------------|----------------|
| 500             | 100            |
| 700             | 150            |
| 1000            | 200            |
| 1500            | 300            |
| 2000            | 350            |

#### Graphical Representation

House Price vs House Size
Price ($1000s)
400 │                  █       █
350 │             █     █
300 │         █   █
200 │     █   █
100 │  █
  0 │──────────────────────────
      500 1000 1500 2000 2500
          House Size (ft²)


**Explanation:**  
- Regression predicts continuous values, like house prices.  
- Algorithm fits a line or curve to predict expected output.  

**Applications:** House price prediction, stock price forecasting, sales prediction, etc.

---

## Key Differences Between Classification and Regression

| Feature                | Classification                  | Regression                  |
|------------------------|--------------------------------|-----------------------------|
| Output Type            | Discrete (0,1, labels)         | Continuous (numeric)       |
| Example                | Tumor: benign/malignant         | House price prediction      |
| Goal                   | Categorize input               | Predict exact/approx. value |
| Graph Representation   | Step or scatter plot with labels | Scatter plot with fitted curve |

