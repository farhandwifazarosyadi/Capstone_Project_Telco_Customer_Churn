# Capstone_Project_Telco_Customer_Churn

# Prediksi Customer Churn pada Perusahaan Telekomunikasi

## Deskripsi Proyek

Customer churn merupakan kondisi ketika pelanggan berhenti menggunakan layanan suatu perusahaan. Dalam industri telekomunikasi, churn menjadi salah satu tantangan utama karena dapat menyebabkan hilangnya pendapatan berulang serta meningkatnya biaya untuk mendapatkan pelanggan baru.

Proyek ini bertujuan untuk membangun model Machine Learning yang mampu memprediksi apakah seorang pelanggan berpotensi melakukan churn berdasarkan karakteristik layanan, kontrak, dan perilaku penggunaan layanan telekomunikasi. Hasil prediksi ini dapat membantu perusahaan melakukan strategi retensi pelanggan secara lebih efektif dan tepat sasaran.

---

## Latar Belakang Masalah

Perusahaan telekomunikasi sering mengalami kehilangan pelanggan akibat churn. Tanpa sistem prediksi yang baik, perusahaan akan kesulitan mengidentifikasi pelanggan yang berisiko tinggi berhenti berlangganan sehingga program retensi menjadi kurang efektif.

Melalui pendekatan Data Science dan Machine Learning, perusahaan dapat memanfaatkan data pelanggan untuk mengidentifikasi pola-pola yang berkaitan dengan churn dan melakukan tindakan pencegahan lebih awal.

---

## Tujuan Proyek

Tujuan utama dari proyek ini adalah:

* Menganalisis faktor-faktor yang memengaruhi customer churn.
* Melakukan eksplorasi dan pembersihan data pelanggan.
* Membangun model klasifikasi untuk memprediksi churn pelanggan.
* Membandingkan performa beberapa algoritma Machine Learning.
* Mengidentifikasi fitur yang paling berpengaruh terhadap churn.
* Memberikan insight yang dapat digunakan untuk strategi retensi pelanggan.

---

## Dataset

Dataset yang digunakan berisi informasi pelanggan telekomunikasi dengan beberapa fitur sebagai berikut:

| Fitur            | Deskripsi                           |
| ---------------- | ----------------------------------- |
| Dependents       | Status tanggungan pelanggan         |
| tenure           | Lama pelanggan berlangganan (bulan) |
| OnlineSecurity   | Status layanan keamanan online      |
| OnlineBackup     | Status layanan backup online        |
| InternetService  | Jenis layanan internet              |
| DeviceProtection | Status perlindungan perangkat       |
| TechSupport      | Status layanan dukungan teknis      |
| Contract         | Jenis kontrak pelanggan             |
| PaperlessBilling | Status tagihan digital              |
| MonthlyCharges   | Biaya bulanan pelanggan             |
| Churn            | Status pelanggan churn atau tidak   |

Target yang diprediksi:

* **0** = Tidak Churn
* **1** = Churn

---

## Tahapan Proyek

### 1. Business Understanding

* Memahami permasalahan churn pada perusahaan telekomunikasi.
* Menentukan tujuan bisnis dan target prediksi.

### 2. Data Understanding

* Memahami struktur dataset.
* Menganalisis tipe data dan karakteristik setiap fitur.

### 3. Data Cleaning

* Pengecekan missing value.
* Analisis pola missing value menggunakan Missingno.
* Pengecekan dan penghapusan data duplikat.
* Standarisasi tipe data.
* Transformasi target menjadi bentuk numerik.

### 4. Exploratory Data Analysis (EDA)

* Analisis distribusi tenure.
* Analisis distribusi MonthlyCharges.
* Analisis distribusi target churn.
* Analisis hubungan fitur numerik terhadap churn.
* Analisis hubungan fitur kategorikal terhadap churn.
* Analisis tingkat churn berdasarkan jenis kontrak pelanggan.

### 5. Feature Engineering

* Membuat fitur tambahan yang relevan untuk meningkatkan kemampuan model dalam mengenali pola churn.

### 6. Data Preprocessing

* Encoding data kategorikal.
* Feature scaling.
* Pembagian data training dan testing.
* Penanganan ketidakseimbangan kelas menggunakan Random Over Sampling.

### 7. Pemodelan Machine Learning

Model yang digunakan dalam proyek ini meliputi:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Random Forest
* XGBoost
* LightGBM

### 8. Evaluasi Model

Performa model dievaluasi menggunakan:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC AUC

Fokus utama evaluasi adalah **Recall** dan **ROC AUC** karena kemampuan mendeteksi pelanggan yang berpotensi churn lebih penting dibandingkan hanya memperoleh akurasi tinggi.

---

## Hasil Analisis

Beberapa insight yang diperoleh dari proses analisis data:

* Pelanggan dengan masa berlangganan yang lebih pendek cenderung memiliki risiko churn lebih tinggi.
* Pelanggan dengan biaya bulanan yang lebih tinggi memiliki tingkat churn yang lebih besar.
* Pelanggan dengan kontrak bulanan (*Month-to-Month*) memiliki tingkat churn tertinggi dibandingkan kontrak tahunan.
* Layanan seperti Tech Support dan Online Security memiliki hubungan terhadap tingkat churn pelanggan.
* Jenis kontrak menjadi salah satu faktor yang paling berpengaruh terhadap churn.

---

## Teknologi yang Digunakan

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Missingno
* Scikit-Learn
* XGBoost
* LightGBM
* Imbalanced-Learn
* Category Encoders

---

## Struktur Proyek

```text
├── data/
│   └── data_telco_customer_churn.csv
│
├── notebook/
│   └── Capstone_Project_Telco_Customer_Churn.ipynb
│
├── model/
│   └── saved_model.pkl
│
├── README.md
└── requirements.txt
```

---

## Kesimpulan

Proyek ini menunjukkan bagaimana Machine Learning dapat digunakan untuk memprediksi customer churn pada industri telekomunikasi. Dengan melakukan analisis data, preprocessing, feature engineering, dan pemodelan klasifikasi, perusahaan dapat mengidentifikasi pelanggan yang berisiko churn lebih awal sehingga strategi retensi dapat dilakukan secara lebih efektif dan berbasis data.
