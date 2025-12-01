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

Pembagian dilakukan dengan train_test_split dari Scikit-learn.
