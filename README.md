# Katonice AI – Food Supply Chain Intelligence

## Deskripsi
KatoNice AI adalah solusi berbasis Artificial Intelligence yang dirancang untuk menganalisis dan memprediksi dinamika harga pangan berdasarkan faktor supply-demand, kondisi lingkungan, serta distribusi logistik.

Sistem ini bertujuan untuk meningkatkan efisiensi rantai pasok agrikultur, menjaga stabilitas harga, serta mendukung ketahanan pangan melalui pendekatan berbasis data (data-driven decision making).

---

## Proposal
Dokumen lengkap dapat diakses melalui:
https://docs.google.com/document/d/1WGjoIuOXC4bZK6i5tp1fbkcgzc2sY_8f/edit?usp=sharing&ouid=102420860608877519115&rtpof=true&sd=true

---

## Tujuan
- Menganalisis faktor utama yang mempengaruhi harga pangan
- Mengidentifikasi ketidakseimbangan supply-demand (gap)
- Membangun model prediksi harga berbasis AI
- Memberikan insight strategis untuk stabilisasi harga dan distribusi

---

## Dataset
Dataset yang digunakan bersifat sintetis realistis yang merepresentasikan kondisi dunia nyata, dengan variabel sebagai berikut:

- Lokasi
- Komoditas
- Tanggal
- Suhu (°C)
- Curah hujan (mm)
- pH tanah
- Produksi (kg)
- Permintaan (kg)
- Harga (per kg)
- Distribusi (jam)

Dataset ini dirancang untuk mensimulasikan kondisi supply chain agrikultur secara komprehensif.

---

## Metodologi

### 1. Exploratory Data Analysis (EDA)
- Analisis missing value, duplikasi, dan outlier
- Visualisasi distribusi data
- Analisis korelasi antar variabel

### 2. Data Cleaning
- Imputasi missing value
- Penghapusan data duplikat
- Filtering data anomali

### 3. Feature Engineering
- Pembuatan fitur **gap (produksi - permintaan)** sebagai indikator supply-demand
- Ekstraksi fitur waktu (bulan) dari tanggal

### 4. Modeling
Model yang digunakan:
- **Random Forest Regressor**

Evaluasi model menggunakan:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

---

## Hasil Model
- Model mampu memprediksi harga dengan tingkat akurasi yang tinggi
- Nilai R² mendekati 1 menunjukkan performa model yang sangat baik
- Pola prediksi mengikuti tren data aktual secara konsisten

---

## Insight Data-Driven
- Supply-demand gap merupakan faktor paling dominan dalam menentukan harga
- Ketika permintaan melebihi produksi, harga cenderung meningkat signifikan
- Distribusi dan faktor lingkungan (cuaca, tanah) berpengaruh terhadap stabilitas supply chain

---

## Insight Strategis
- Gap negatif → diperlukan tambahan distribusi atau impor
- Gap positif → dilakukan distribusi ke wilayah dengan kekurangan
- Monitoring harga dan supply dapat dilakukan secara real-time menggunakan AI

---

## Implementasi Azure
Solusi ini dirancang untuk scalable deployment menggunakan Microsoft Azure:

- **Azure Machine Learning**  
  Training, deployment, dan monitoring model AI  

- **Azure Blob Storage**  
  Penyimpanan dataset dan model  

- **Azure App Service**  
  Penyediaan API untuk prediksi real-time  

### Arsitektur Sistem
User → API → Model AI → Prediksi Harga → Insight

Sistem ini memungkinkan integrasi AI dalam aplikasi nyata secara real-time dan scalable.

---

## Pipeline Sistem
1. Data dikumpulkan dari berbagai sumber
2. Data dibersihkan dan diproses
3. Feature engineering dilakukan
4. Model AI dilatih
5. Model disimpan dalam format (`model.pkl`)
6. Model digunakan untuk prediksi dan analisis

---

## Kesimpulan
KatoNice AI berhasil mengimplementasikan pendekatan berbasis AI untuk menganalisis dan memprediksi harga pangan secara efektif.

Sistem ini tidak hanya memberikan prediksi, tetapi juga menghasilkan insight yang dapat digunakan untuk:
- Menjaga stabilitas harga pangan
- Mengoptimalkan distribusi
- Mengurangi potensi food waste
- Mendukung pengambilan keputusan berbasis data

Dengan pengembangan lebih lanjut, sistem ini berpotensi menjadi solusi nyata dalam mendukung ketahanan pangan berbasis teknologi AI.
