# Heart Disease Diagnosis using Machine Learning 🫀

**UAS Informatika Biomedik**

Project ini merupakan replikasi dan eksperimen lanjutan dari framework machine learning untuk diagnosis penyakit jantung, mengacu pada paper:

> **"A Machine Learning-Based Framework for Heart Disease Diagnosis Using a Comprehensive Patient Cohort"**
> Saadia Tabassum, Fazal Muhammad, Muhammad Ayaz Khan, Muhammad Uzair Khan, Dawar Awan, Neelam Gohar, Shahid Khan, Amal Al-Rasheed

Model dibangun ulang berdasarkan metodologi pada paper tersebut, dengan eksperimen tambahan untuk melihat dampak _outlier removal_ terhadap performa model.

**Presented by:** Dian Pratiwi

## 🎯 Tujuan

Membangun dan mengevaluasi model machine learning untuk diagnosis penyakit jantung berdasarkan data kohort pasien, serta menganalisis pengaruh penanganan outlier terhadap performa model yang dihasilkan.

## 🔬 Eksperimen yang Dilakukan

- Pengujian model **tanpa outlier removal**
- Pengujian model **dengan outlier removal**
- Analisis dampak outlier terhadap performa model
- Perbandingan performansi antar eksperimen berdasarkan:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
- Analisis ROC Curve

## 🛠️ Teknologi yang Digunakan

- Python
- Jupyter Notebook
- (sertakan library yang dipakai, misal: scikit-learn, pandas, numpy, matplotlib/seaborn)

📈 Hasil Eksperimen
Experiment 1 — Tanpa Outlier Removal
Model	Accuracy	Precision	Recall	F1	AUC
Logistic Regression	0.8949	0.8974	0.9150	0.9061	0.9326
Naive Bayes	0.8659	0.8867	0.8693	0.8779	0.9173
Bagging	0.8696	0.8774	0.8889	0.8831	0.9153
AdaBoost	0.8732	0.8882	0.8824	0.8852	0.9185
XGBoost	0.8768	0.8993	0.8758	0.8874	0.9354
Experiment 2 — Dengan Outlier Removal (Isolation Forest)
Model	Accuracy	Precision	Recall	F1	AUC
Logistic Regression	0.8678	0.8504	0.9076	0.8780	0.9174
Naive Bayes	0.8634	0.8667	0.8740	0.8703	0.9145
Bagging	0.8150	0.8407	0.7983	0.8190	0.8973
AdaBoost	0.8546	0.8525	0.8740	0.8631	0.9024
XGBoost	0.8282	0.8175	0.8655	0.8408	0.9032

Dari kedua eksperimen ini, model dengan performa terbaik secara keseluruhan adalah Logistic Regression dan XGBoost — keduanya konsisten unggul di hampir semua metrik. Menariknya, penerapan Isolation Forest untuk outlier removal pada eksperimen ini justru menurunkan performa sebagian besar model dibanding tanpa outlier removal, sehingga penanganan outlier bukan selalu berdampak positif dan perlu dievaluasi secara empiris untuk tiap dataset.

## 📊 Dataset

Dataset yang digunakan bersumber dari **Kaggle** (dataset publik). _(https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction/data)_

## 📁 Struktur Project

```
├── notebook.ipynb        # Notebook utama berisi eksperimen & analisis
├── data/                  # Dataset yang digunakan
└── README.md
```

## 🚀 Cara Menjalankan

1. Clone repository ini
2. Install dependency yang dibutuhkan:
   ```
   pip install -r requirements.txt
   ```
3. Buka file notebook dengan Jupyter Notebook/JupyterLab, atau langsung lewat Google Colab
4. Jalankan cell secara berurutan dari atas ke bawah

## 📖 Referensi

Tabassum, S., Muhammad, F., Khan, M.A., Khan, M.U., Awan, D. et al. (2025). A Machine Learning-Based Framework for Heart Disease Diagnosis Using a Comprehensive Patient Cohort. _Computers, Materials & Continua, 84(1)_, 1253–1278. https://doi.org/10.32604/cmc.2025.065423

## 📄 Lisensi

Project ini dibuat untuk keperluan tugas akademik (UAS Informatika Biomedik).
