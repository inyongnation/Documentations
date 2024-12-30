### Tutorial Lengkap Menjalankan Skrip "Auto WP Poster AI Featured Image"

#### **1. Persiapan Lingkungan**
1. **Install Python**:
   Pastikan Python versi 3.7+ telah terinstall di perangkat Anda.
   - Periksa versi Python:
     ```bash
     python --version
     ```
   - Jika belum terinstall, unduh dari [python.org](https://www.python.org/downloads/).

2. **Install Paket Pendukung**:
   Pastikan perangkat Anda memiliki akses internet untuk mengunduh dependensi.

#### **2. Membuat File Skrip**
1. Buat file bernama `main.py`:
   ```bash
   nano main.py
   ```
2. Salin kode Python yang disediakan ke dalam file tersebut, lalu simpan.

#### **3. Membuat File Konfigurasi**
1. Buat file `config.py` di direktori yang sama:
   ```bash
   nano config.py
   ```
2. Isi dengan detail berikut:
   ```python
   OPENROUTER_API_KEY = "Masukkan_API_Key_Anda"
   PEXELS_API_KEY = "Masukkan_API_Key_Anda"
   WP_USERNAME = "Masukkan_Username_WordPress"
   WP_PASSWORD = "Masukkan_Password_WordPress"
   WP_URL = "https://yourwordpresssite.com/wp-json/wp/v2/posts"
   CATEGORIES = {
       "Teknologi": 1,
       "Kesehatan": 2,
       "Gaya Hidup": 3
   }
   POST_INTERVAL = 600  # Dalam detik, misalnya 600 untuk 10 menit
   ```
   Sesuaikan kategori dan ID kategori sesuai konfigurasi situs WordPress Anda.

#### **4. Menjalankan Skrip**
1. Pastikan Anda berada di direktori skrip.
   ```bash
   cd /path/to/your/script/
   ```
2. Jalankan skrip:
   ```bash
   python main.py
   ```

#### **5. Fungsi-Fungsi dalam Skrip**
- **`ensure_libraries_installed()`**: Menginstal library yang diperlukan secara otomatis.
- **`generate_title(category)`**: Membuat judul artikel berdasarkan kategori menggunakan AI.
- **`generate_article(category)`**: Membuat artikel berdasarkan judul yang dihasilkan.
- **`get_featured_image(keyword)`**: Mengambil gambar unggulan dari Pexels menggunakan kata kunci.
- **`post_article(title, content, category_id, image_url)`**: Memposting artikel ke WordPress.

#### **6. Troubleshooting**
- **Masalah instalasi library**: Pastikan pip terinstall dan jalankan:
  ```bash
  pip install -r requirements.txt
  ```
  Buat file `requirements.txt` jika diperlukan:
  ```
  requests
  ```
- **Kesalahan API**: Periksa validitas API Key Anda dan pastikan koneksi internet stabil.
- **Kategori tidak sesuai**: Pastikan ID kategori di `config.py` sesuai dengan ID kategori di WordPress.

#### **7. Penghentian Skrip**
- Tekan `Ctrl+C` untuk menghentikan proses kapan saja.

#### **Catatan Tambahan**
- **Interval Waktu**: Anda dapat mengubah waktu antar posting melalui variabel `POST_INTERVAL` di `config.py`.
