# 🚀 Proyek Analisis Sentimen dan Scraping Data 🕵️‍♂️

Proyek ini berfokus pada pengumpulan data menggunakan teknik web scraping 🛠️ dan menganalisis sentimen data tersebut melalui pendekatan pemodelan machine learning 🤖. Folder ini berisi dua file notebook utama yang saling berkaitan untuk menjalankan pipeline ini:

1. **📂 ScrappingData.ipynb** - Notebook untuk scraping data.
2. **📂 AnalisisSentimenModels.ipynb** - Notebook untuk memproses data hasil scraping dan menjalankan analisis sentimen.

---

## 🗺️ Alur Kerja Proyek

### 1. 🕵️‍♂️ Scraping Data dengan `ScrappingData.ipynb`

Notebook **ScrappingData.ipynb** bertanggung jawab untuk mengumpulkan data mentah dari sumber tertentu menggunakan teknik web scraping. Berikut langkah-langkah utama yang dilakukan:

- **🔍 Pendefinisian Sumber Data**: Notebook ini mengidentifikasi URL atau API sebagai sumber data. Sumber bisa berupa situs web ulasan, forum, atau media sosial.
  
- **🧹 Pembersihan Data Awal**: Data yang dikumpulkan mungkin berisi elemen-elemen yang tidak relevan, seperti tag HTML, whitespace, atau karakter khusus. Notebook ini melakukan pembersihan data awal.

- **💾 Penyimpanan Data**: Setelah data dikumpulkan dan dibersihkan, notebook ini menyimpan hasilnya dalam format CSV atau JSON yang akan digunakan pada tahap analisis berikutnya.

**📤 Hasil Output**:
- File data mentah yang siap digunakan untuk analisis sentimen pada tahap berikutnya.

---

### 2. 📊 Analisis Sentimen dengan `AnalisisSentimenModels.ipynb`

Notebook **AnalisisSentimenModels.ipynb** memanfaatkan data hasil scraping untuk melakukan analisis sentimen. Berikut langkah-langkah utama yang dilakukan:

- **📥 Load Data**: Notebook ini membaca data yang dihasilkan oleh **ScrappingData.ipynb**.
  
- **🧽 Pembersihan Data Lanjutan**: Data mungkin memerlukan pembersihan tambahan, seperti menghilangkan stopwords, stemming, atau lemmatization.

- **🔎 Eksplorasi Data**: Visualisasi awal dilakukan untuk memahami distribusi sentimen, frekuensi kata, atau pola-pola lainnya.

- **🔧 Preprocessing**:
  - Tokenisasi teks.
  - Normalisasi teks.
  - Pembagian data menjadi set pelatihan dan pengujian.

- **🤖 Model Machine Learning**:
  - Membangun model machine learning untuk analisis sentimen menggunakan algoritma seperti Naive Bayes, Logistic Regression, atau deep learning.
  - Evaluasi model dengan metrik seperti akurasi, precision, recall, dan F1-score.

- **📊 Visualisasi Hasil**:
  - Hasil analisis sentimen ditampilkan melalui grafik dan tabel untuk mempermudah interpretasi.

**📤 Hasil Output**:
- Model analisis sentimen yang terlatih.
- Visualisasi hasil analisis untuk mendukung wawasan bisnis atau riset.

---

## 🛠️ Cara Menggunakan Proyek Ini

### 1. Persyaratan Sistem
- **🐍 Python**: Versi 3.8 atau lebih baru.
- **📦 Pustaka Python**: Pastikan pustaka berikut sudah terinstal:
  - `pandas`
  - `numpy`
  - `beautifulsoup4`
  - `requests`
  - `scikit-learn`
  - `matplotlib`
  - `nltk` atau pustaka pemrosesan teks lainnya.

### 2. Langkah-langkah Eksekusi

1. **🕵️‍♀️ Scraping Data**:
   - Jalankan **ScrappingData.ipynb**.
   - Pastikan koneksi internet stabil jika scraping data dari situs online.
   - Simpan hasil scraping ke dalam folder `data/`.

2. **📊 Analisis Sentimen**:
   - Jalankan **AnalisisSentimenModels.ipynb** setelah scraping data selesai.
   - Lakukan preprocessing, training, dan evaluasi model.
   - Visualisasikan hasil analisis untuk mendapatkan wawasan mendalam.
