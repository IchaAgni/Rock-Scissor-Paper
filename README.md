# 🪨✂️🧻 Rock-Scissor-Paper Image Classification

Proyek ini merupakan implementasi model klasifikasi gambar menggunakan TensorFlow dan Keras untuk mengenali gesture tangan dalam permainan **batu-gunting-kertas (rock-paper-scissors)**. Proyek ini dibuat sebagai submission untuk kelas **Belajar Machine Learning untuk Pemula** dari Dicoding.

## 📁 Deskripsi Proyek

Model ini dilatih untuk mengklasifikasikan gambar ke dalam 3 kelas:
- `rock` (batu)
- `paper` (kertas)
- `scissors` (gunting)

Dataset yang digunakan adalah dataset publik dari [Rock Paper Scissors Dataset by Laurence Moroney](https://laurencemoroney.com/rock-paper-scissors-dataset/) melalui TensorFlow Datasets (`tfds`).

## 🚀 Teknologi dan Library

- Python 3.x
- TensorFlow
- Keras
- Matplotlib
- NumPy
- OS, pathlib, shutil
- Google Colab (opsional)

## 🧠 Arsitektur Model

Model Convolutional Neural Network (CNN) dengan struktur sebagai berikut:

- `Conv2D` + `MaxPooling2D` (3 blok)
- `Flatten`
- `Dense` (hidden layer)
- `Dense` (output layer, softmax)

Model dikompilasi menggunakan:
- Loss function: `categorical_crossentropy`
- Optimizer: `adam`
- Metrics: `accuracy`

## 📊 Hasil Pelatihan

Model mencapai akurasi validasi lebih dari **90%**, tergantung jumlah epoch dan augmentasi yang digunakan.

## 📂 Struktur Proyek
  rock-scissor-classification/
  │
  ├── Submission_Belajar_ML_untuk_Pemula.ipynb # Notebook utama
  
  ├── README.md # Dokumentasi ini
  
  └── dataset/ # (jika menggunakan dataset lokal)

## ✅ Cara Menjalankan

1. Buka file `Submission_Belajar_ML_untuk_Pemula.ipynb` menggunakan Jupyter Notebook atau Google Colab.
2. Jalankan sel satu per satu.
3. Model akan mengunduh dataset, melakukan augmentasi, pelatihan, dan evaluasi.
4. Untuk pengujian, dapat digunakan `model.predict()` pada gambar baru.

## 💡 Pengembangan Selanjutnya

- Menambahkan teknik augmentasi lanjutan
- Menggunakan transfer learning (misalnya MobileNetV2)
- Menyimpan model ke file `.h5` dan digunakan dalam aplikasi web atau mobile

## 📝 Lisensi

Proyek ini disusun untuk keperluan edukasi. Dataset merupakan milik publik yang disediakan oleh TensorFlow Datasets.


