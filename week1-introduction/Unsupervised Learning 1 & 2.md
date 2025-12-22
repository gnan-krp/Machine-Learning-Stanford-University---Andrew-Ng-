# Unsupervised Learning Notes

After **supervised learning**, the next widely used type of machine learning is **unsupervised learning**.  

> Don’t let the name “unsupervised” fool you — it is just as powerful and widely used as supervised learning.

---

## 1. Definition

Unsupervised learning is a type of machine learning where the algorithm learns **patterns or structure in data without labeled outputs**.  

- Unlike supervised learning, we **do not provide output labels (y)** for each input.  
- The algorithm must **figure out patterns, relationships, or clusters** in the data on its own.  

**Example dataset:**

| Patient | Tumor Size (cm) | Age (years) |
|---------|----------------|-------------|
| 1       | 2              | 30          |
| 2       | 3              | 32          |
| 3       | 5              | 68          |
| 4       | 7              | 70          |

- Here, we **don’t know if tumors are benign or malignant**.  
- The goal is to **discover patterns or groupings** in the data.

---

## 2. Key Concepts

### 2.1 Clustering
Clustering is one of the main types of unsupervised learning.  

- It **groups data points into clusters** based on similarity.  
- No prior labels are required — the algorithm **learns the grouping from the data itself**.  

**Applications of clustering:**

- **Google News:** Groups related news articles together.  
- **Customer segmentation:** Groups customers based on buying behavior.  
- **Image compression:** Groups similar pixels or patterns.  
- **Medical data:** Groups patients with similar symptoms for study.  

### 2.2 Dimensionality Reduction
Another type of unsupervised learning.  

- Reduces the number of variables while keeping important information.  
- Helps **visualize high-dimensional data**.  
- Common techniques: **PCA (Principal Component Analysis)**, **t-SNE**.  

---

## 3. How Unsupervised Learning Works

1. **Input:** Unlabeled dataset.  
2. **Process:** Algorithm searches for patterns, correlations, or groups.  
3. **Output:** Groups (clusters), associations, or compressed representations.  

**Example:** Tumor dataset with only **size and age**.  

- Cluster 1: Younger patients, smaller tumors.  
- Cluster 2: Older patients, larger tumors.  

The algorithm does **not know the correct answer** but identifies meaningful structures.  

---

## 4. Example: Clustering Graph (Two Clusters)

```markdown
Tumor Size vs Age (Two Clusters)

Age →
70 │        █   █   █   █
   │        █   █   █
   │        █   █
60 │
50 │
40 │
30 │  █   █   █   █
   │  █   █   █
   │  █   █
   └────────────────────────
     1   2   3   5   7
       Tumor Size (cm)

## 5. Summary of Unsupervised Learning

- **Supervised learning:** Predicts outputs from labeled data.  
- **Unsupervised learning:** Finds patterns and clusters in unlabeled data.  
- **Key techniques:**  
  - **Clustering:** Groups similar data points.  
  - **Dimensionality reduction:** Simplifies high-dimensional data.  
- **Applications:** News grouping, customer segmentation, image compression, exploratory data analysis.  

> Unsupervised learning lets the algorithm **discover structure in the data on its own**, making it powerful for understanding complex datasets without labels.

---

## 6. Advantages of Unsupervised Learning

- Does **not require labeled data**, saving time and cost.  
- Can **discover hidden patterns** in the data.  
- Useful for **exploratory data analysis**.  
- Can **improve supervised learning** by preprocessing or extracting features.  

---

## 7. Limitations of Unsupervised Learning

- Harder to **evaluate performance** without ground-truth labels.  
- Results can be **sensitive to the choice of algorithm and parameters**.  
- Clusters or patterns found may **not always have real-world significance** — interpretation is required.  
