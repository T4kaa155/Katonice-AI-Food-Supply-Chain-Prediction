# KatoNice AI - Supply Chain Intelligence

## Deskripsi
KatoNice adalah sistem berbasis AI untuk menganalisis dan memprediksi stabilitas rantai pasok pangan di Indonesia, dengan fokus pada integrasi data produksi, lingkungan, distribusi, dan permintaan pasar.

---

## Dataset
Dataset terdiri dari dua jenis:

- **Raw Dataset**
  - Mengandung missing value, duplicate, dan anomali
  - Merepresentasikan kondisi data nyata

- **Clean Dataset**
  - Sudah melalui proses data cleaning
  - Digunakan untuk model AI

---

## Metodologi
1. Data Collection
2. Data Cleaning
3. Feature Engineering (gap = supply-demand)
4. Model Machine Learning (Random Forest)
5. Evaluation & Insight

---

## Model
Model yang digunakan:
- Random Forest Regressor

Target:
- Prediksi harga komoditas

---

## Insight
- Supply-demand gap menjadi faktor utama harga
- Ketidakseimbangan distribusi menyebabkan fluktuasi
- Faktor lingkungan berpengaruh terhadap produksi

---

## Struktur Project
katonice-ai/
├── data/
    └── katonice_dataset_clean.csv
    └── katonice_dataset_realistic_raw.csv
├── notebooks/
├── models/
├── src/
└── README.md

---

## Tools
- Python
- Pandas
- Scikit-learn
- Matplotlib

---

## Tujuan
Meningkatkan efisiensi distribusi, mengurangi food waste, dan menjaga stabilitas harga pangan melalui pendekatan data-driven.
