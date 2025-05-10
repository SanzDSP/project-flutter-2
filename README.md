# 🖼️ Image Classification Project

Proyek ini merupakan implementasi deep learning untuk klasifikasi gambar ke dalam beberapa kategori menggunakan Convolutional Neural Networks (CNN) dengan TensorFlow dan Keras. Model ini juga dikonversi ke dalam format **TensorFlow Lite** dan **TensorFlow.js** untuk kebutuhan deployment di perangkat mobile dan web.

---

## 📁 Struktur Direktori
```bash
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
```
---

## 🔍 Dataset

Dataset tersimpan dalam direktori `dataset/` dan terdiri dari beberapa kategori:

| Kategori       | Format File     | Link Dataset                                                                                  |
|----------------|------------------|-----------------------------------------------------------------------------------------------|
| 🐱 cat_image    | `.png`, `.jpg`   | [Google Drive](https://drive.google.com/drive/folders/1MrzZwGCUnE1mORZ8votd6yxrHllqFxk5?usp=drive_link) |
| 🚗 car_image1   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1-gK5XGUqNEOx5E25kR1mytco-LfE6xwP?usp=drive_link) |
| 🚗 car_image2   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1XdJsHKxA1cDYa5P-k3CdDkd_XhTu2i6c?usp=drive_link) |
| 🚗 car_image3   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1ZF1o8QETklAu1yHPO8vkzY4JU6QsQXhX?usp=drive_link) |
| 🚗 car_image4   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1_-Bz4VtuaLaX2EW99n5YiUbXb4qo1Hvb?usp=drive_link) |
| 🚗 car_image5   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1u-gySSMaa44T28lQnaB1SHTnZvAzMYPY?usp=drive_link) |
| 🚗 car_image6   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1EppOA47fqLf_pELEuM1pa62HWVF4x28a?usp=drive_link) |
| 🚗 car_image7   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1IoVHgWV3ncba7BnAQZpnMgdDM7R6RMwp?usp=drive_link) |
| 🚗 car_image8   | `.jpeg`          | [Google Drive](https://drive.google.com/drive/folders/1JwKwHZQuCXJzpj3pGhsmoa77PfD6duYs?usp=drive_link) |
| 🌻 flower_image1| `.jpg`           | [Google Drive](https://drive.google.com/drive/folders/12JhgAcSUwMAO62qVLTIYg6W06r6GhtJV?usp=drive_link) |
| 🌼 flower_image2| `.jpg`           | [Google Drive](https://drive.google.com/drive/folders/1hDKl19jo4oYBQFE9gHeu7V-8MBUlc29S?usp=drive_link) |
| 🌼 flower_image3| `.jpg`           | [Google Drive](https://drive.google.com/drive/folders/132IYg7i2r5O2dvZCBgoD_boI4Whb7TzN?usp=drive_link) |

📌 **Catatan:**  
Resolusi gambar dalam dataset sangat bervariasi, mulai dari kecil (misal 64x64 piksel) hingga sedang (misal 256x256 piksel), dan memiliki berbagai format file (`.jpg`, `.png`, `.jpeg`). Hal ini menegaskan bahwa preprocessing diperlukan untuk menyamakan ukuran gambar sebelum pelatihan model.

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
