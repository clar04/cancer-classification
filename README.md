# 📊 Biomedical Cancer Publication Classifier

Proyek ini bertujuan untuk mengklasifikasikan publikasi teks biomedis ke dalam jenis kanker spesifik menggunakan teknik machine learning berbasis **Apache Spark (PySpark)** dan pustaka Python.

---

## 📝 Deskripsi Proyek

Tujuan utama dari proyek ini adalah mengembangkan model machine learning yang mampu mengklasifikasikan **publikasi biomedis** ke dalam tiga kategori kanker:

- **Kanker Tiroid**  
- **Kanker Paru-paru**  
- **Kanker Usus Besar**

Proses pengembangan meliputi:
- Pemuatan dan eksplorasi dataset
- Pembersihan dan prapemrosesan teks
- Pelatihan dan evaluasi beberapa model klasifikasi

---

## ⚙️ Tools & Pustaka yang Digunakan

### Framework Utama
- **Apache Spark (PySpark)** — Pemrosesan data skala besar dan algoritma machine learning terdistribusi

### Pustaka Python
- `pandas`, `numpy` — Manipulasi dan analisis data
- `seaborn`, `matplotlib` — Visualisasi data, termasuk *confusion matrix*
- `tensorflow.keras.preprocessing.text.Tokenizer` — Prapemrosesan teks biomedis
- `sklearn.metrics.confusion_matrix` — Evaluasi kinerja model
- `tqdm` — Menampilkan progres bar interaktif

---

## 📂 Dataset

Dataset yang digunakan adalah dari Kaggle:  
**Biomedical Text Publication Classification**  
Dataset ini berisi kumpulan abstrak teks biomedis dengan label jenis kanker.  
🔗 [Link Dataset (Kaggle)](https://www.kaggle.com/datasets/falgunipatel19/biomedical-text-publication-classification)  

---

## 🧪 Hasil Evaluasi Model

Setelah proses prapemrosesan dan pembagian data (80% pelatihan, 20% pengujian), tiga model klasifikasi diuji:

### 1. 🔹 Logistic Regression
- **Akurasi**: 0.9974
- **F1-Score**:
  - Kanker Tiroid: 0.9965
  - Kanker Usus Besar: 0.9981
  - Kanker Paru-paru: 0.9976

### 2. 🌲 Random Forest
- **Akurasi**: 0.9473
- **F1-Score**:
  - Kanker Tiroid: 0.9368
  - Kanker Usus Besar: 0.9313
  - Kanker Paru-paru: 0.9811

### 3. 🌿 Decision Tree
- **Akurasi**: 0.9184
- **F1-Score**:
  - Kanker Tiroid: 0.8878
  - Kanker Usus Besar: 0.8924
  - Kanker Paru-paru: 0.9939

📌 **Kesimpulan**:  
Model **Logistic Regression** memberikan performa terbaik dengan akurasi dan F1-score yang sangat tinggi di seluruh kelas.

---
