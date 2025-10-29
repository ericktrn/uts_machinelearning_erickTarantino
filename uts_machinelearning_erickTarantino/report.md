# Laporan Singkat — Tugas UTS Machine Learning (Klasifikasi)

**Nama Mahasiswa**: Erick Tarantino  
**NIM**: (231011403335)  
**Kelas/Semester**: Semester 5

---

**Judul**: Klasifikasi Dataset Iris menggunakan Logistic Regression dan Decision Tree  
**Mata Kuliah**: Machine Learning  
**Dosen Pengampu**: (isi sesuai e-learning)

---

## Deskripsi Dataset

Dataset **Iris** berisi 150 sampel bunga iris dengan empat fitur numerik:

- Sepal length
- Sepal width
- Petal length
- Petal width

Target (label) terdiri dari tiga kelas:

1. Setosa
2. Versicolor
3. Virginica

Sumber dataset: _scikit-learn built-in dataset (Anderson, 1936)_.

---

## Model yang Digunakan

1. **Logistic Regression**  
   Model linear untuk klasifikasi multikelas (menggunakan metode _one-vs-rest_).  
   Data diskalakan dengan _StandardScaler_.

2. **Decision Tree Classifier**  
   Model berbasis pohon keputusan tanpa memerlukan scaling.  
   Dapat menangkap hubungan non-linear antar fitur.

---

## Evaluasi Model

Metode evaluasi yang digunakan:

- Confusion Matrix
- Accuracy, Precision, Recall, F1-score
- ROC Curve (micro-average, multiclass)

Hasil evaluasi disimpan dalam folder `output_files/`:

- `confusion_matrix_LogisticRegression.png`
- `confusion_matrix_DecisionTree.png`
- `roc_models_comparison.png`
- `results_summary.csv`
- `results_summary.json`

---

## Hasil dan Pembahasan

Kedua model menunjukkan performa tinggi karena dataset Iris relatif mudah diklasifikasikan.

- Logistic Regression memberikan hasil stabil dan efisien.
- Decision Tree lebih fleksibel terhadap pola non-linear namun berpotensi overfitting.

Untuk pengembangan lebih lanjut, bisa ditambahkan:

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Cross-validation untuk meningkatkan generalisasi.

---

## Kesimpulan

Kedua model berhasil mengklasifikasikan data bunga iris dengan akurasi yang tinggi.  
Perbedaan utama terletak pada interpretabilitas model:

- Logistic Regression lebih mudah dijelaskan,
- Decision Tree lebih visual namun memerlukan pengaturan parameter agar tidak overfit.

---

**Dibuat oleh:**  
🧑‍🎓 Erick Tarantino  
Semester 5 — Universitas Pamulang  
Tugas UTS Machine Learning 2025
