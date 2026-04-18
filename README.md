# Bank Marketing Customer Segmentation

## Overview
Project ini bertujuan untuk melakukan segmentasi nasabah menggunakan teknik clustering pada dataset bank marketing. Tujuan utama adalah mengidentifikasi kelompok nasabah berdasarkan perilaku dan karakteristik untuk mendukung strategi pemasaran yang lebih efektif.

---

## Dataset
Dataset yang digunakan adalah **Bank Marketing Dataset**, yang berisi informasi demografis, finansial, dan riwayat interaksi nasabah dengan bank.

---

## Methods
Beberapa metode clustering yang digunakan dalam project ini:
- K-Means dengan Gower Distance
- K-Means dengan FAMD
- K-Prototypes
- K-Prototypes + FAMD (Best Model)

---

## Key Results

- Metode terbaik: **K-Prototypes + FAMD**
- Silhouette Score meningkat dari **0.186 → 0.253**
- Jumlah cluster optimal: **3–4 cluster**

### Distribusi Cluster (Final Model)
- Cluster 2: **82.3%** (mayoritas nasabah)
- Cluster 1: **9.7%**
- Cluster 0: **8.0%**

---

## Key Insights

- Segmentasi lebih dipengaruhi oleh:
  - **pdays (waktu sejak kontak terakhir)**
  - **previous (jumlah kontak sebelumnya)**
  - **age**

- Faktor finansial seperti balance kurang berpengaruh

---

## Business Insights

- **82% nasabah** belum banyak dihubungi → peluang besar untuk campaign
- **~10% nasabah** terlalu sering dihubungi → perlu strategi baru
- **~8% nasabah** sudah lama tidak dihubungi → cocok untuk re-engagement

👉 Kesimpulan:
Strategi marketing harus berbasis **behavior (interaksi)**, bukan hanya profil nasabah.

---

## Tech Stack
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
Install dependencies:
pip install -r requirements.txt
Jalankan notebook:
jupyter notebook

Author

Mohammad Tyas Subianto
