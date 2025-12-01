# 🪨📄✂️ Rock–Paper–Scissors Image Classification
### Image Classification using Convolutional Neural Network (CNN) & TensorFlow

Project ini merupakan implementasi fundamental machine learning untuk mengenali gesture tangan Batu (Rock), Kertas (Paper), dan Gunting (Scissors) menggunakan deep learning berbasis Convolutional Neural Network (CNN).

---

## Deskripsi Project

Project ini bertujuan untuk membangun model klasifikasi gambar yang dapat mengenali gesture tangan: rock, paper, dan scissors. Dataset yang digunakan berasal dari Dicoding Academy, yang berisi kumpulan gambar tangan dengan pose berbeda.Model dilatih menggunakan TensorFlow dan Keras, dilengkapi dengan image augmentation untuk meningkatkan performa generalisasi model.

---

## Dataset

Dataset yang digunakan adalah:
- Rock-Paper-Scissors Dataset
  
  Sumber: Dicoding Academy
  Link: https://github.com/dicodingacademy/assets/releases/download/release/rockpaperscissors.zip

| Kelas | Jumlah Gambar |
|-----------|-------|
| Rock | 726 |
| Paper | 712 |
| Scissors | 750 |

Dataset kemudian dibagi menjadi:
- 60% data training
- 40% data validation

Pembagian dilakukan dengan "train_test_split" dari Scikit-learn.

---

## Tujuan Project

- Membangun model deep learning untuk mengenali gambar batu/kertas/gunting.
- Melakukan preprocessing & image augmentation untuk meningkatkan akurasi model.
- Melatih model CNN menggunakan TensorFlow.
- Melakukan evaluasi model berdasarkan akurasi dan loss.
- Menguji model dalam memprediksi gambar yang di-upload pengguna.

---

## Arsitektur Model

Model menggunakan arsitektur CNN Sequential dengan struktur berikut:
- Conv2D(32 filters) + MaxPooling
- Conv2D(64 filters) + MaxPooling
- Conv2D(128 filters) + MaxPooling
- Flatten
- Dropout(0.5)
- Dense 128 (ReLU)
- Dense 3 (Softmax) → output 3 kelas

Optimizer: Adam
Loss function: Categorical Crossentropy

---

## Hasil Model

Model mencapai performa berikut:
- Akurasi Training: ± 90–97%
- Akurasi Validasi: ± 85–95%

Grafik training & validasi meliputi:
- Accuracy vs Validation Accuracy
- Loss vs Validation Loss
