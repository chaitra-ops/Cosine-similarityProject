# 🛒 Grocery Basket Similarity using Cosine Similarity

## 📌 Overview

This project was developed as part of the **Silicon Synapses Club** under the **Department of Artificial Intelligence & Machine Learning** at Vasavi College of Engineering.

The project analyzes customer purchasing patterns by measuring the similarity between grocery baskets using **Cosine Similarity**. By identifying baskets with similar item compositions, retailers can gain valuable insights into customer behavior, improve product recommendations, and optimize inventory management.

---

## 🎯 Problem Statement

Retail stores generate large amounts of transaction data every day. Analyzing customer purchase behavior manually is difficult and time-consuming.

The objective of this project is to develop a system that:

- Measures similarity between customer grocery baskets.
- Identifies customers with similar purchasing patterns.
- Provides insights for recommendation systems and targeted marketing.

---

## 🚀 Objectives

- Compute similarity between grocery baskets using Cosine Similarity.
- Identify baskets with similar purchase behavior.
- Generate a similarity matrix for analysis.
- Support customer segmentation and product recommendation strategies.

---

## 🧠 Concept Used

### Cosine Similarity

Cosine Similarity measures the similarity between two vectors by calculating the cosine of the angle between them.

### Formula

\[
CosineSimilarity(A,B)=\frac{A \cdot B}{||A|| \times ||B||}
\]

Where:

- **A** and **B** are basket vectors.
- **A · B** is the dot product.
- **||A||** and **||B||** are vector magnitudes.

### Interpretation

| Similarity Score | Meaning |
|------------------|----------|
| 1 | Exactly Similar |
| 0 | Completely Different |
| Between 0 and 1 | Partially Similar |

---

## 🛠️ Technologies Used

- Python
- Google Colab

### Libraries

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📂 Dataset

Dataset Used:

**Market_Basket_Optimisation.csv**

Features:

- Each row represents a customer transaction.
- Contains multiple purchased items.
- Used for market basket analysis.

---

## ⚙️ Methodology

### Step 1: Data Collection

Load the market basket dataset containing customer transactions.

### Step 2: Data Preprocessing

- Handle missing values.
- Extract purchased items.
- Prepare data for encoding.

### Step 3: Binary Encoding

Convert each basket into a binary vector:

- 1 → Item Purchased
- 0 → Item Not Purchased

Example:

| Milk | Bread | Butter |
|-------|--------|--------|
| 1 | 1 | 0 |

### Step 4: Similarity Calculation

Use Scikit-learn's cosine similarity function to compute pairwise basket similarities.

```python
from sklearn.metrics.pairwise import cosine_similarity
```

### Step 5: Similarity Matrix Generation

Generate a similarity matrix showing relationships between all baskets.

### Step 6: Visualization

Visualize similarity scores using heatmaps and matrices.

### Step 7: Analysis

Identify highly similar baskets and understand purchasing trends.

---

## 📊 Results

- Successfully computed pairwise basket similarities.
- Identified basket groups with similarity scores greater than **0.8**.
- Generated similarity matrices for visualization.
- Derived insights into customer buying behavior.
- Demonstrated potential use in recommendation systems.

<img width="619" height="748" alt="Screenshot 2026-06-25 at 22 36 13" src="https://github.com/user-attachments/assets/46116db5-f6b6-401d-952e-b165cf434bea" />
<img width="553" height="604" alt="Screenshot 2026-06-25 at 22 36 35" src="https://github.com/user-attachments/assets/be3c4945-fcf6-4a34-a2b2-a89acfa8e379" />


---

## 📈 Applications

### Product Recommendation Systems

Recommend products based on similar customer baskets.

### Market Basket Analysis

Discover purchasing patterns and frequently bought-together items.

### Customer Segmentation

Group customers with similar shopping behavior.

### Targeted Marketing

Create personalized promotions and offers.

### Inventory Management

Predict demand for related products.

---

## 🔍 Sample Workflow

```
Transaction Data
       ↓
Data Cleaning
       ↓
Binary Encoding
       ↓
Cosine Similarity Calculation
       ↓
Similarity Matrix
       ↓
Visualization & Analysis
       ↓
Business Insights
```

---

## 📚 Key Learnings

- Understanding vector-based similarity measures.
- Applying Cosine Similarity in real-world datasets.
- Data preprocessing and feature encoding.
- Working with Scikit-learn libraries.
- Visualizing high-dimensional data using heatmaps.
- Understanding customer behavior analytics.

---


## 🏛️ Organization

**Silicon Synapses Club**  
Department of Artificial Intelligence & Machine Learning  
Vasavi College of Engineering

---

## 🔮 Future Enhancements

- Implement real-time recommendation systems.
- Compare multiple similarity metrics (Jaccard, Euclidean, Pearson).
- Build an interactive dashboard using Streamlit.
- Integrate clustering algorithms for customer segmentation.
- Deploy the project as a web application.

---

## ⭐ Conclusion

This project demonstrates how Cosine Similarity can effectively measure relationships between grocery baskets and uncover valuable customer purchasing patterns. The insights generated can help businesses improve recommendation systems, marketing strategies, and inventory management processes.
