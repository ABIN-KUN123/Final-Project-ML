# Student Performance Prediction (Classification)

**Final Project - Pembelajaran Mesin 1** **Universitas Darussalam Gontor**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Deskripsi Proyek
Repository ini berisi dokumentasi dan kode sumber untuk Tugas Akhir mata kuliah Pembelajaran Mesin 1. Proyek ini bertujuan untuk membangun model *Machine Learning* yang dapat memprediksi kemungkinan seorang siswa lulus atau gagal berdasarkan karakteristik sosial, demografi, dan akademik mereka.

Tujuan utama dari analisis ini adalah membantu institusi pendidikan melakukan **deteksi dini** terhadap siswa yang berisiko gagal agar dapat diberikan intervensi yang tepat.

## 📂 Dataset
Dataset yang digunakan bersifat publik dan diambil dari **UCI Machine Learning Repository**.

* **Nama Dataset:** Student Performance Dataset
* **Sumber:** [UCI Repository Link](https://archive.ics.uci.edu/dataset/320/student+performance)
* **Referensi:** P. Cortez and A. Silva. *Using Data Mining to Predict Secondary School Student Performance*, 2008.

## ⚙️ Metodologi
Berdasarkan rumusan masalah untuk pengambilan keputusan (Lulus/Gagal), proyek ini menggunakan pendekatan **Klasifikasi (*Supervised Learning*)**.

* **Algoritma:** Random Forest Classifier.
* **Alasan Pemilihan:** Algoritma ini dipilih karena kemampuannya menangani fitur campuran (numerik dan kategorikal) serta memberikan akurasi yang konsisten tanpa risiko *overfitting* yang tinggi.
* **Target Variabel:** Nilai akhir (`G3`) dikonversi menjadi label biner:
    * `1` (Lulus): Nilai $\ge$ 10
    * `0` (Gagal): Nilai $<$ 10

## 📊 Hasil Analisis
Dari eksperimen yang dilakukan dalam notebook ini, ditemukan bahwa faktor-faktor berikut memiliki pengaruh terbesar terhadap kelulusan siswa (*Feature Importance*):
1.  **Failures:** Jumlah kegagalan pada kelas sebelumnya.
2.  **Absences:** Jumlah ketidakhadiran siswa.
3.  **Medu/Fedu:** Tingkat pendidikan orang tua.
4.  **Studytime:** Waktu belajar mingguan.

*(Detail visualisasi dan metrik evaluasi dapat dilihat pada file notebook)*

## 🚀 Cara Menjalankan Kode
1.  Clone repository ini:
    ```bash
    git clone [https://github.com/username-anda/ML1-Student-Performance.git](https://github.com/username-anda/ML1-Student-Performance.git)
    ```
2.  Install library yang dibutuhkan:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn ucimlrepo
    ```
3.  Jalankan file notebook:
    `final-project-mechine-learning.ipynb`

*Project ini diajukan untuk memenuhi syarat penilaian akhir semester Genap 2025-2026.*
