# 📝 Intelligent Email Writer for Students

**Cut Sula Fhatia Rahma**  (2208107010048)

Proyek ini merupakan aplikasi berbasis Web yang memungkinkan mahasiswa membuat email secara otomatis dan profesional dengan bantuan teknologi Large Language Model (LLM) dari **Gemini API**.

---

## 📦 Fitur Utama

- Memilih kategori email: Akademik, Skripsi, Magang, dll.
- Menentukan nada (tone) penulisan: formal, netral, atau santai.
- Mendukung Bahasa Indonesia dan Inggris.
- Mengisi poin-poin utama yang ingin disampaikan dalam email.
- Menghasilkan email yang profesional, jelas, dan padat secara otomatis.

---

## 📁 Struktur Proyek

```
intelligent\_email\_writer/
├── .env                     # Berisi API Key Gemini
├── app.py                  # Frontend dengan Streamlit
├── backend/
│   └── main.py             # Backend API menggunakan FastAPI
└── requirements.txt        # Dependensi backend

````

---

## ⚙️ Instalasi dan Menjalankan Proyek

### 1. Kloning repository

```bash
git clone https://github.com/csulafr/UAS_Cut-Sula-Fhatia-Rahma_2208107010048.git
cd UAS-Praktikum-Pembelajaran-Mesin
````

### 2. Setup dan jalankan Backend (FastAPI)

```bash
# Buat dan aktifkan environment
python3.10 -m venv env
source env/bin/activate   # Linux/macOS
env\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Jalankan server
uvicorn backend.main:app --reload --host 0.0.0.0 --port 8000
```

### 3. Setup dan jalankan Frontend (Streamlit)

Buka terminal baru:

```bash
# Pastikan sudah berada di direktori project
streamlit run app.py
```

---

## 🔐 Konfigurasi API Key Gemini

1. Buka [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
2. Klik **Create API Key**.
3. Copy API key dan simpan ke dalam file `.env` di root project dengan format:

```env
GEMINI_API_KEY=your_api_key_here
```

---

## 📬 Contoh Penggunaan

1. Pilih kategori dan gaya penulisan email.
2. Masukkan informasi penerima, subjek, dan poin-poin penting.
3. Klik tombol **"Buat Email"**.
4. Email hasil generate akan ditampilkan di halaman aplikasi.

## 📋 Hasil dan Tampilan Frontend

![Screenshot](images/Screenshot-hasil-1.png) <br>
![Screenshot](images/Screenshot-hasil-2.png)
