# Bank Marketing Customer Segmentation

## Overview
This project aims to segment customers using clustering techniques on a bank marketing dataset. The main objective is to identify customer groups based on behavior and characteristics to support more effective marketing strategies.

---

## Dataset
The dataset used is the **Bank Marketing Dataset**, which contains demographic, financial, and historical information about customers' interactions with the bank.

---

## Methods
Several clustering methods used in this project:
- K-Means with Gower Distance
- K-Means with FAMD
- K-Prototypes
- K-Prototypes + FAMD (Best Model)

---

## Key Results

- Best method: **K-Prototypes + FAMD**
- Silhouette Score increased from **0.186 → 0.253**
- Optimal number of clusters: **3–4 clusters**

### Cluster Distribution (Final Model)
- Cluster 2: **82.3%** (majority of customers)
- Cluster 1: **9.7%**
- Cluster 0: **8.0%**

---

## Key Insights

- Segmentation is more influenced by:
- **pdays (time since last contact)**
- **previous (number of previous contacts)**
- **age**

- Financial factors such as insufficient balance influential

---

## Business Insights

- **82% of customers** haven't been contacted much → great opportunity for campaigns
- **~10% of customers** are contacted too often → need a new strategy
- **~8% of customers** haven't been contacted for a long time → suitable for re-engagement

👉 Conclusion:
Marketing strategies must be based on **behavior (interaction)**, not just customer profiles.

---

## TechStack
- Python
- Pandas, NumPy
- Scikit-learn
- KModes (K-Prototypes)
- Prince (FAMD)
- Matplotlib, Seaborn

---

## How to Run

1. Clone repository:
```bash
git clone https://github.com/Underag3/bank-marketing-clustering.git
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
Run notebook:
2. Install dependencies:
```bash
jupyter notebook
```
Author

Mohammad Tyas Subianto
