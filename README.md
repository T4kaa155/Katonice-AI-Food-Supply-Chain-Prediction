# KatoNice AI – Food Supply Chain Intelligence

## Deskripsi
KatoNice AI adalah solusi berbasis Artificial Intelligence yang bertujuan untuk menganalisis dan memprediksi harga pangan berdasarkan faktor supply-demand, kondisi lingkungan, dan distribusi logistik.

Sistem ini dirancang untuk membantu menjaga stabilitas harga pangan serta meningkatkan efisiensi rantai pasok agrikultur.

---

## Tujuan
- Menganalisis faktor yang mempengaruhi harga pangan
- Mengidentifikasi ketidakseimbangan supply-demand
- Membangun model prediksi harga berbasis AI
- Memberikan insight strategis untuk stabilisasi harga

---

## Dataset
Dataset yang digunakan bersifat sintetis realistis dan merepresentasikan kondisi dunia nyata, meliputi:

- Lokasi
- Komoditas
- Tanggal
- Suhu
- Curah hujan
- pH tanah
- Produksi (kg)
- Permintaan (kg)
- Harga (per kg)
- Distribusi (jam)


---

## Metodologi

### 1. Exploratory Data Analysis (EDA)
- Analisis missing value, duplikasi, dan anomali
- Visualisasi distribusi data
- Analisis korelasi antar variabel

### 2. Data Cleaning
- Imputasi missing value
- Penghapusan duplikasi
- Filtering data anomali

### 3. Feature Engineering
- Pembuatan fitur **gap (produksi - permintaan)**
- Ekstraksi bulan dari tanggal

### 4. Modeling
Model yang digunakan:
- **Random Forest Regressor**

Evaluasi model:
- RMSE
- MAE
- R² Score

---

## Hasil Model

- Model mampu memprediksi harga dengan akurasi tinggi
- Nilai R² mendekati 1 menunjukkan performa yang sangat baik
- Prediksi mengikuti pola data aktual dengan baik

---

## Insight

- Supply-demand gap merupakan faktor utama yang mempengaruhi harga
- Ketika permintaan lebih tinggi dari produksi, harga meningkat
- Distribusi dan faktor lingkungan turut mempengaruhi stabilitas harga

---

## Insight Strategis

- Jika gap negatif → perlu tambahan distribusi/impor
- Jika gap positif → distribusi ke wilayah kekurangan
- Monitoring harga dapat dilakukan secara real-time dengan AI

---

## Implementasi Azure

Solusi ini dirancang untuk dapat di-deploy menggunakan layanan Microsoft Azure:

- **Azure Machine Learning** → training & deployment model
- **Azure Blob Storage** → penyimpanan dataset
- **Azure App Service** → API prediksi real-time

### Arsitektur:
User → API → Model → Prediksi Harga

Sistem ini memungkinkan monitoring harga pangan secara scalable dan real-time.

---

## Pipeline Sistem

1. Data dikumpulkan
2. Data dibersihkan
3. Feature engineering dilakukan
4. Model dilatih
5. Model disimpan (model.pkl)
6. Model digunakan untuk prediksi

---
