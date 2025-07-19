# NeurIPS - Ariel Data Challenge 2025

## Deskripsi
Notebook ini dibuat untuk mengikuti kompetisi **Ariel Data Challenge 2025** di NeurIPS. Tujuan utama kompetisi ini adalah memprediksi spektrum transmisi planet ekstrasurya berdasarkan data time-series dari instrumen AIRS-CH0 dan FGS1, serta metadata terkait bintang dan planet. Notebook ini mencakup seluruh pipeline mulai dari eksplorasi data, ekstraksi fitur, baseline model, hingga deep learning dan ensembling.

## Struktur Notebook
1. **Setup & Environment**: Instalasi dan import library yang dibutuhkan.
2. **Load & Verifikasi Data**: Memuat data utama (CSV & Parquet), kalibrasi ADC, dan verifikasi struktur data.
3. **Exploratory Data Analysis (EDA)**: Visualisasi spektrum transmisi, distribusi parameter bintang, dan analisis time-series.
4. **Preprocessing & Feature Engineering**: Ekstraksi fitur time-series dari sinyal terkalibrasi, detrending, dan statistik deskriptif.
5. **Baseline Model**: Ridge Regression, XGBoost, dan LightGBM dengan fitur PCA spektrum.
6. **Deep Learning Model**: Implementasi model InceptionTime untuk prediksi spektrum dari data time-series.
7. **Evaluation & Hyperparameter Tuning**: Cross-validation, tuning hyperparameter (scikit-learn & Keras Tuner).
8. **Ensembling & Submission**: Kombinasi model dan pembuatan file submission untuk kompetisi.

## Cara Menjalankan
1. **Persiapkan Data**: Pastikan struktur folder dan file dataset sesuai dengan path di notebook (misal `/kaggle/input/ariel-data-challenge-2025/`).
2. **Instalasi Library**: Jalankan cell instalasi jika di luar lingkungan Kaggle (`pip install kaggle pyarrow lightgbm xgboost keras-tuner`).
3. **Jalankan Notebook**: Eksekusi cell secara berurutan dari atas ke bawah.
4. **Training & Evaluasi**: Notebook menyediakan baseline model dan deep learning, serta tuning hyperparameter.
5. **Submission**: Hasil prediksi dapat disimpan ke `submission.csv` sesuai format kompetisi.

## Kebutuhan Library
- numpy
- pandas
- pyarrow
- matplotlib
- seaborn
- scikit-learn
- xgboost
- lightgbm
- tensorflow
- torch (opsional)
- keras-tuner

## Catatan Penting
- Pastikan path data sudah benar, terutama jika menjalankan di luar Kaggle.
- Notebook ini dapat dikembangkan lebih lanjut, misal dengan menambah fitur, model, atau teknik ensembling lain.
- Untuk inference pada data test, pastikan fungsi kalibrasi dan ekstraksi fitur sudah sesuai dengan data test.

## Referensi
- [Ariel Data Challenge 2025 - Kaggle](https://www.kaggle.com/competitions/ariel-data-challenge-2025)
- [Ariel Mission](https://arielmission.space/) 