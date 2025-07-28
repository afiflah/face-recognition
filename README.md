# 🧠 Face Recognition with Waifu Dataset

Proyek ini merupakan implementasi face recognition berbasis Python dengan tambahan dataset waifu untuk pengujian algoritma deteksi dan pencocokan wajah.

> 🎓 Tugas UAS Mata Kuliah Kecerdasan Buatan  
> 👨‍💻 Mahasiswa: Muhammad Fathir Afif (NIM: 2370231013)  
> 📅 Tahun: 2025

---

## 📁 Struktur Proyek

├── generate_encodings.py # Generate encoding wajah real manusia
├── generate_waifu_encodings.py # Generate encoding dari gambar waifu
├── realtime_detect.py # Deteksi wajah secara real-time
├── realtime_matcher.py # Mencocokkan wajah dengan data yang ada
├── requirements.txt # Dependensi Python yang dibutuhkan
├── .gitignore # File yang diabaikan Git (zip, npy, cache)

yaml
Copy
Edit

---

## ⚙️ Cara Menjalankan

1. **Clone repository**
   ```bash
   git clone https://github.com/afiflah/recognition.git
   cd recognition
Install dependensi

bash
Copy
Edit
pip install -r requirements.txt
Siapkan gambar wajah

Letakkan gambar wajah di folder faces/ atau waifus/ (jika kamu menggunakannya).

File besar seperti images.zip tidak disertakan di repo (lihat .gitignore).

Generate encoding

bash
Copy
Edit
python generate_encodings.py
python generate_waifu_encodings.py
Jalankan deteksi real-time

bash
Copy
Edit
python realtime_detect.py
Jalankan pencocokan wajah

bash
Copy
Edit
python realtime_matcher.py
💡 Catatan
Encoding wajah akan disimpan dalam file .npy.

Pastikan kamera aktif jika menjalankan realtime_detect.py.

Gambar waifu digunakan untuk eksperimen pengenalan wajah non-manusia (novelty dataset).

🧩 Dependensi
Beberapa library utama:

face_recognition

opencv-python

numpy

dlib

Lihat file requirements.txt untuk daftar lengkap.
