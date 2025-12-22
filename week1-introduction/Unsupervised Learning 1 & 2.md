# Unsupervised Learning

After **supervised learning**, the next widely used form of machine learning is **unsupervised learning**.  

> Don’t let the name “unsupervised” fool you — it is just as powerful as supervised learning.

---

## 1. What is Unsupervised Learning?

In **supervised learning**, each example is associated with an **output label (y)**, such as “benign” or “malignant” for a tumor.  

In **unsupervised learning**, the data **does not have any output labels**. For example:  

| Patient | Tumor Size (cm) | Age (years) |
|---------|----------------|-------------|
| 1       | 2              | 45          |
| 2       | 5              | 50          |
| 3       | 1              | 35          |
| 4       | 7              | 60          |

- Notice that we **don’t know** if the tumor is benign or malignant.  
- The goal is **not to predict labels**, but to **find structure, patterns, or interesting insights** in the data.

---

## 2. How Unsupervised Learning Works

- The algorithm is **not given correct answers**.  
- Instead, it tries to **figure out patterns or clusters** in the data.  
- For example, an algorithm might find that the data naturally separates into **two groups**:

Tumor Size vs Age (Two Clusters)

Age →
90 │        █   █   █   █
80 │        █   █   █
70 │        █   █
60 │
50 │
40 │
30 │  █   █   █   █
   │  █   █   █
   │  █   █
   └────────────────────────
     1   2   3   5   7
       Tumor Size (cm)



- These groups are called **clusters**.  

---

## 3. Clustering Algorithms

- Clustering is a type of **unsupervised learning** that assigns **unlabeled data into different clusters**.  
- Example applications:  
  - **Google News:** Groups related news articles together every day.  
  - **Customer segmentation:** Groups customers with similar behavior.  
  - **Image compression:** Groups similar pixels or patterns.  

> In short, unsupervised learning is about letting the algorithm **discover structure in the data on its own**.

