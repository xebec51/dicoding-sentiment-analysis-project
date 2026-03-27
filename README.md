# 🧠 Sentiment Analysis (NLP Project)

<p align="center">
  <a href="https://github.com/xebec51">
    <img src="https://img.shields.io/badge/GitHub-xebec51-blue?logo=github" />
  </a>
  <a href="https://www.linkedin.com/in/rinaldiruslan">
    <img src="https://img.shields.io/badge/LinkedIn-rinaldiruslan-0A66C2?logo=linkedin&logoColor=white" />
  </a>
  <a href="https://www.instagram.com/rinaldiruslan/">
    <img src="https://img.shields.io/badge/Instagram-rinaldiruslan-E4405F?logo=instagram" />
  </a>
  <a href="https://www.tiktok.com/@rinaldiruslan">
    <img src="https://img.shields.io/badge/TikTok-rinaldiruslan-000000?logo=tiktok&logoColor=white" />
  </a>
  <br/>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" />
  </a>
  <img src="https://img.shields.io/badge/NLP-Sentiment%20Analysis-orange" />
</p>

---

🌐 **Submission dari Kelas**:
[Belajar Fundamental Deep Learning - Dicoding](https://www.dicoding.com/academies/185/)

📌 **Submission ke-1 dari 2 Submission pada kelas ini**

---

## 📌 Deskripsi Proyek

Proyek ini merupakan implementasi **analisis sentimen berbasis Natural Language Processing (NLP)** untuk mengklasifikasikan ulasan pengguna aplikasi menjadi:

* ✅ Positif
* 😐 Netral
* ❌ Negatif

Dataset dikumpulkan melalui **scraping mandiri dari Google Play Store (Shopee App)** sesuai dengan ketentuan submission.

Proyek ini mencerminkan **end-to-end pipeline NLP**, mulai dari data collection hingga evaluasi model.

---

## 🚀 Key Highlights

* ✅ Data scraping mandiri (≥10.000 data)
* ✅ Preprocessing teks lengkap (cleaning, normalization, dll)
* ✅ Feature engineering:

  * TF-IDF (word + character n-gram)
* ✅ Multiple model:

  * Logistic Regression (baseline)
  * BiLSTM (Deep Learning)
  * IndoBERT (Transformer)
* ✅ Model optimization (tuning + hard negative mining)
* ✅ Evaluasi lengkap:

  * Accuracy, Precision, Recall, F1-score
  * Confusion Matrix
* ✅ Error analysis & insight

---

## 📊 Dataset Overview

Dataset berisi ulasan pengguna aplikasi Shopee dari Google Play Store dengan atribut utama:

* Text review
* Rating (1–5)
* Label sentimen (negatif, netral, positif)

### 📌 Distribusi Label

* Negatif: Rating 1–2
* Netral: Rating 3
* Positif: Rating 4–5

Dataset telah melalui:

* Data cleaning
* Duplicate removal
* Normalisasi teks
* Balancing + augmentation

---

## ⚙️ Metodologi

### 1. Data Collection (Scraping)

* Library: `google-play-scraper`
* Target: Shopee App (`com.shopee.id`)
* Jumlah data: >10.000

---

### 2. Data Preprocessing

* Case folding
* Cleaning (remove symbol, angka, dll)
* Normalisasi slang
* Tokenization

---

### 3. Feature Engineering

#### 🔹 TF-IDF

* Word n-gram (1,2)
* Character n-gram

#### 🔹 Sequence Modeling

* Tokenizer + Padding

---

### 4. Modeling

#### 🔹 Logistic Regression

* Baseline model
* TF-IDF features

#### 🔹 BiLSTM

* Deep Learning model
* Embedding + Bidirectional LSTM

#### 🔹 IndoBERT

* Transformer-based model
* Fine-tuning pre-trained IndoBERT

---

## 📈 Hasil Model

| Model               | Accuracy  |
| ------------------- | --------- |
| Logistic Regression | 0.88      |
| BiLSTM              | 0.83      |
| IndoBERT            | **0.92+** |

📌 **Best Model: IndoBERT**

---

## 🔍 Insight Utama

* TF-IDF sangat efektif untuk teks pendek dan terstruktur
* LSTM tidak selalu outperform model tradisional
* IndoBERT unggul dalam menangkap konteks bahasa
* Kelas **netral** merupakan yang paling sulit diklasifikasi (ambigu)

---

### 🔗 Lihat di GitHub

* [📘 Sentiment Analysis Notebook](https://github.com/xebec51/dicoding-sentiment-analysis-project/blob/main/Sentiment_Analysis.ipynb)
* [📊 Scraping Notebook](https://github.com/xebec51/dicoding-sentiment-analysis-project/blob/main/Scraping_Data.ipynb)

---

## 📂 Struktur Proyek

```bash
.
├── Sentiment_Analysis.ipynb
├── Scraping_Data.ipynb
├── shopee_reviews_final.csv
├── shopee_reviews_raw.csv
├── requirements.txt
│
├── hasil_prediksi.csv
├── confusion_matrix.png
├── model.safetensors
├── README.md
```

---

## ▶️ Cara Menjalankan

### 1. Clone repository

```bash
git clone https://github.com/xebec51/dicoding-sentiment-analysis-project.git
```

### 2. Masuk ke folder

```bash
cd dicoding-sentiment-analysis-project
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Jalankan notebook

* Scraping_Data.ipynb
* Sentiment_Analysis.ipynb

---

## 🛠️ Teknologi yang Digunakan

* Python
* Pandas & NumPy
* Scikit-learn
* TensorFlow / PyTorch
* HuggingFace Transformers
* Matplotlib & Seaborn

---

## 👤 Author

**Muh. Rinaldi Ruslan**

* 💻 GitHub: https://github.com/xebec51
* 💼 LinkedIn: https://www.linkedin.com/in/rinaldiruslan
* 📸 Instagram: https://www.instagram.com/rinaldiruslan/
* 🎵 TikTok: https://www.tiktok.com/@rinaldiruslan

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License**.
