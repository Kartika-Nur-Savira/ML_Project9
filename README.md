# ML_Project9

Klasifikasi Status Kesehatan Berdasarkan Faktor Gaya Hidup Menggunakan Metode Ensemble Learning

## Deskripsi Project 
Klasifikasi Status Kesehatan Berdasarkan Faktor Gaya Hidup adalah sebuah proyek machine learning yang bertujuan untuk memprediksi status kesehatan umum (General Health) seseorang hanya menggunakan indikator non-klinis seperti gaya hidup, kondisi fisik, dan sosiodemografi.

## Dataset
Dataset yang digunakan adalah Behavioral Risk Factor Surveillance System (BRFSS) 2022 yang dipublikasikan oleh Centers for Disease Control and Prevention dan tersedia melalui platform Kaggle. Dataset ini berisi data survei kesehatan masyarakat dengan ratusan ribu responden. Penelitian ini menggunakan 23 fitur non-klinis yang mencakup karakteristik demografis, gaya hidup, kondisi fisik, dan riwayat pemeriksaan kesehatan. Variabel target yang diprediksi adalah GeneralHealth, yaitu status kesehatan umum yang terdiri dari lima kategori ordinal: Poor, Fair, Good, Very Good, dan Excellent. 

## Latar Belakang:
Status kesehatan umum (general health) seseorang merupakan cerminan menyeluruh dari kondisi fisik, mental, gaya hidup yang dijalaninya sehari-hari terbukti menjadi prediktor kuat terhadap kematian dini, kejadian penyakit, serta tingginya biaya pengobatan [1] . Indonesia sebagai negara dengan jumlah penduduk lebih dari 270 juta jiwa menghadapi tantangan besar dalam pemantauan status kesehatan masyarakat secara menyeluruh, terutama di wilayah-wilayah yang memiliki keterbatasan akses terhadap fasilitas pelayanan kesehatan. Kondisi ini menyebabkan banyak individu tidak memiliki rekam medis atau data riwayat penyakit yang lengkap, sehingga pendekatan prediksi yang bergantung pada data klinis menjadi sulit diterapkan secara luas.
Peneliti sebelumnya menunjukkan bahwa faktor-faktor non-klinis seperti aktivitas fisik, status sosial ekonomi, dan perilaku kesehatan memiliki peran penting yang sangat signifikan terhadap status kesehatan, bahkan tanpa bergantung pada data riwayat penyakit [1], [3]. Temuan ini membuka peluang untuk mengembangkan model prediksi status kesehatan berbasis data yang mudah diperoleh tanpa prosedur medis, yang sangat relevan dengan Riskesdas (Riset Kesehatan Dasar).
Oleh karena itu, penelitian ini berfokus pada prediksi status kesehatan hanya berdasarkan informasi yang dapat diperoleh tanpa diagnosis medis menggunakan perbandingan algoritma Logistic Regression, Random Forest, dan XGBoost untuk mengklasifikasikan ‘GeneralHealth’. Jika terbukti efektif, pendekatan ini berpotensi diadaptasi ke dalam sistem pemantauan kesehatan masyarakat di Indonesia, membantu tenaga kesehatan dan pembuat kebijakan dalam mengidentifikasi masyarakat berisiko secara lebih cepat dan efisien

## Alur Penelitian 
Proyek ini bertujuan untuk membangun model klasifikasi penyakit jantung (Heart Disease Prediction) menggunakan beberapa algoritma machine learning dan membandingkan performanya untuk mendapatkan model terbaik.
1. Exploratory Data Analysis (EDA)
Tahap awal dilakukan untuk memahami karakteristik dataset, meliputi:
- Pemeriksaan tipe data setiap fitur.
- Analisis distribusi fitur dan target.
- Deteksi missing value.
- Deteksi outlier.
- Analisis ketidakseimbangan kelas (class imbalance).
- Analisis korelasi antar fitur.
2. Data Splitting
Dataset dibagi menjadi data latih dan data uji dengan rasio 80:20 untuk memastikan evaluasi model dilakukan pada data yang belum pernah dilihat sebelumnya.
3. Data Preprocessing
Tahap preprocessing dilakukan untuk meningkatkan kualitas data sebelum proses pelatihan model, yang mencakup:
- Data Cleaning
- Penanganan missing value.
- Penanganan outlier.
- Penghapusan data duplikat.
- Feature Engineering
- Feature Scaling untuk menstandarkan rentang nilai fitur.
- Feature Selection untuk memilih fitur yang paling relevan.
- Encoding untuk mengubah data kategorikal menjadi format numerik.
4. Handling Class Imbalance
Metode SMOTE (Synthetic Minority Oversampling Technique) diterapkan pada data latih untuk mengatasi ketidakseimbangan kelas dan meningkatkan kemampuan model dalam mengenali kelas minoritas.
5. Post-Processing EDA
Analisis ulang dilakukan setelah preprocessing dan SMOTE untuk memastikan kualitas data telah meningkat serta distribusi kelas menjadi lebih seimbang.
6. Model Development
Beberapa algoritma machine learning digunakan dan dibandingkan, yaitu:
- Logistic Regression
- Random Forest
- XGBoost
- CatBoost
7. Model Evaluation
Setiap model dievaluasi menggunakan metrik performa yang relevan, kemudian dilakukan perbandingan untuk menentukan model dengan kinerja terbaik.

