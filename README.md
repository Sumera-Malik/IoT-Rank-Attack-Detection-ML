# IoT-Rank-Attack-Detection-ML
This project presents a complete machine learning pipeline for detecting **Rank Attacks** in **RPL (Routing Protocol for Low Power and Lossy Networks)** — a critical security threat in IoT systems. The solution explores both **supervised and unsupervised learning techniques** using a custom dataset derived from RPL traffic simulations.

Project Objectives

- Preprocess real-world RPL traffic data
- Handle class imbalance using SMOTE
- Build and evaluate supervised models like **Random Forest**
- Apply **unsupervised learning**: One-Class SVM and KMeans
- Compare results using key metrics: Accuracy, Precision, Recall, F1-Score
- Enable scalable anomaly detection for smart IoT systems

---

## 📁 Files Included

- `ML-Project-Final.ipynb` — Core Jupyter Notebook containing full ML pipeline
- `Rank_Attack_Report.pdf` — Project report with detailed methodology and results
- `requirements.txt` — Python dependencies for reproducibility

---

## 🔍 Dataset Overview

- **Name:** `Rank.csv`
- **Labels:** `PCKT_LABEL` → 0 (Normal), 1 (Rank Attack)
- **Features:** Extracted from simulated RPL network traffic
- **Size:** Includes over 40 relevant features after preprocessing

---

## 🧠 Models Used

### ✅ Supervised
- **Random Forest**
  - With and without SMOTE oversampling
  - Best results achieved using SMOTE

### 🧪 Unsupervised
- **One-Class SVM**
- **KMeans Clustering**

---

## 📊 Results Summary

| Method                | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Random Forest (orig) | 1.00     | 1.00      | 1.00   | 1.00     |
| RF (shuffled)        | 0.24     | 0.30      | 0.23   | 0.26     |
| RF + SMOTE           | 1.00     | 1.00      | 1.00   | 1.00     |
| One-Class SVM        | 0.94     | 0.17      | 1.00   | 0.30     |
| KMeans               | 0.90     | 0.85      | 0.90   | 0.88     |

---
## 📥 Dataset Access

Due to size/restrictions, the dataset is not hosted here.
