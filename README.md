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

## 📊 Dataset

Dataset yang digunakan bersumber dari **Kaggle** (dataset publik). _(tambahkan link dataset Kaggle-nya di sini kalau ada)_

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
