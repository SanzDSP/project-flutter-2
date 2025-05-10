# 🖼️ Image Classification Project

Proyek ini merupakan implementasi deep learning untuk klasifikasi gambar ke dalam beberapa kategori menggunakan Convolutional Neural Networks (CNN) dengan TensorFlow dan Keras. Model ini juga dikonversi ke dalam format **TensorFlow Lite** dan **TensorFlow.js** untuk kebutuhan deployment di perangkat mobile dan web.

---

## 📁 Struktur Direktori

submission/

├───tfjs_model/ # Model dalam format TensorFlow.js

│ ├───group1-shard1of1.bin

│ └───model.json

├───tflite/ # Model dalam format TFLite

│ ├───model.tflite

│ └───label.txt

├───saved_model/ # Model dalam format SavedModel

│ ├───saved_model.pb

│ └───variables/

├───notebook.ipynb # Notebook utama berisi pelatihan dan konversi model

├───README.md # File dokumentasi proyek ini (Anda disini)

└───requirements.txt # Daftar dependensi/proyek

---

## 🔍 Dataset

Dataset tersimpan dalam direktori `dataset/` dan terdiri dari beberapa kategori:
- Gambar bunga (`flower_image`)
- Gambar mobil (`car_image`)
- Gambar kucing (`cat_image`)

Dataset dibagi secara otomatis menjadi data training, validation, dan testing menggunakan `ImageDataGenerator`.

---

## 🧠 Model Arsitektur

Model CNN terdiri dari:
- 3 blok Conv2D + MaxPooling2D
- Flatten layer
- Fully Connected (Dense) layer dengan Dropout
- Output layer menggunakan softmax

---

## 📊 Hasil Pelatihan

- **Akurasi Training (epoch 2):** 98.46%
- **Akurasi Validasi:** 98.27%
- **Akurasi Testing:** 98.91%
- **Prediksi Sample:** `✅ Prediksi: flower (confidence: 1.00)`

---

## 🚀 Deployment

Model dikonversi ke:
- **TensorFlow Lite (.tflite)** untuk mobile (Android/iOS)
- **TensorFlow.js** untuk aplikasi web interaktif

---

## 📦 Cara Install Dependensi

```bash
pip install -r requirements.txt

```
--- 

## 🤖 Tools & Library
Python 3

- TensorFlow & Keras

- TensorFlow Lite Converter

- TensorFlow.js Converter

- Scikit-Learn, Pandas, Matplotlib

---
