# Unsupervised Learning Notes

"""
After supervised learning, the next widely used type of machine learning is unsupervised learning.
Don't let the name fool you — unsupervised learning is just as powerful as supervised learning.
"""

#  1. Definition 
"""
Unsupervised learning is a type of machine learning where the algorithm is given data without 
any associated output labels (y). The goal is to find patterns, structures, or interesting 
insights in the data automatically.

Key points:
- No supervision (no labeled outputs)
- Algorithm identifies patterns or clusters
- Useful when labeling data is expensive or impossible
"""

#  2. Example 
"""
Supervised Learning Example (Classification):
- Each example has a label y
- Example: Tumor classification as benign or malignant
  Input: Tumor size, Patient age
  Output: Label (benign/malignant)
  
Unsupervised Learning Example:
- Data has no labels
- Example: Patients' tumor size and age without benign/malignant label
- Task: Find patterns, structures, or clusters in the data
"""

#  3. Goal of Unsupervised Learning 
"""
- Discover hidden structures in data
- Group similar data points together
- Reduce dimensionality or summarize data
- Generate insights without explicit guidance
"""

#  4. Types of Unsupervised Learning 
# 4.1 Clustering
"""
- Groups data points into clusters based on similarity
- Example: Two clusters of patients based on tumor size and age
- Applications:
  - Customer segmentation
  - Image segmentation
  - Document clustering (e.g., Google News groups related news articles)

Clustering Visualization:

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

Explanation:
- Each 'o' or 'x' represents a data point
- Algorithm automatically assigns similar points to the same cluster
- No labels are provided
"""

# 4.2 Dimensionality Reduction
"""
- Reduce the number of features while preserving important information
- Techniques: PCA (Principal Component Analysis), t-SNE
- Applications:
  - Data visualization
  - Noise reduction
  - Feature extraction
"""

#  5. Key Characteristics 
"""
- Works on unlabeled data
- Finds intrinsic patterns
- Often exploratory
- Helps understand the underlying structure of data
"""

#  6. Summary 
"""
Unsupervised learning allows machines to:
1. Explore data without explicit answers
2. Discover patterns, clusters, or structures
3. Assist in data analysis, feature extraction, and grouping

Important applications:
- Clustering (grouping similar data points)
- Dimensionality reduction (simplifying complex data)
- Market segmentation, recommendation systems, anomaly detection
"""
