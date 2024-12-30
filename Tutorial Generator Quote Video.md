# Tutorial Lengkap Menjalankan Skrip "Video Quote Generator"

## Pendahuluan
Skrip "Video Quote Generator" adalah alat untuk membuat video berkualitas HD yang menampilkan epigraf menarik sesuai tema yang diinginkan.

---

## Persiapan

### 1. Prasyarat Sistem
- **Python 3.x**
- Internet stabil untuk API
- **API Key** dari layanan berikut:
  - OpenRouter
  - Pexels
  - Rclone (untuk penyimpanan cloud)

### 2. Instalasi Library yang Dibutuhkan
Skrip ini membutuhkan beberapa library berikut:
- `moviepy`
- `requests`
- `pyfiglet`

Jika library belum diinstal, skrip akan secara otomatis menginstalnya.

### 3. Konfigurasi API Keys
Pastikan Anda memiliki API Keys yang valid:
- Tambahkan API Key ke file `config.py` dengan format berikut:
  ```python
  OPENROUTER_API_KEY = "<YOUR_OPENROUTER_API_KEY>"
  PEXELS_API_KEY = "<YOUR_PEXELS_API_KEY>"
  RCLONE_DESTINATION = "<YOUR_RCLONE_DESTINATION>"
  ```

---

## Menjalankan Skrip

### 1. Unduh dan Siapkan Skrip
Simpan skrip berikut ke file bernama `main.py`:
```python
# [Kode lengkap sudah diberikan sebelumnya]
```

### 2. Jalankan Skrip
Eksekusi file menggunakan Python:
```bash
python main.py
```

## Kesalahan Umum dan Solusinya

1. **Library Tidak Terinstal**
   - Pastikan koneksi internet stabil.
   - Jalankan perintah berikut secara manual:
     ```bash
     pip install moviepy requests pyfiglet
     ```

2. **Kesalahan API**
   - Periksa kembali API Keys di file `config.py`.
   - Pastikan API Keys aktif dan memiliki kuota yang cukup.

3. **Video Tidak Dapat Diunggah**
   - Pastikan rclone telah dikonfigurasi dengan benar.
   - Uji rclone secara manual:
     ```bash
     rclone move <local_file_path> <destination_path>
     ```

---

## Tips Tambahan
- Gunakan tema yang menarik untuk hasil video yang lebih menonjol.
- Pastikan resolusi gambar yang diambil cukup tinggi untuk kualitas video HD.
- Jika teks epigraf terlalu panjang, potong teks sebelum proses pembuatan video.

---

## Penutup
Skrip ini dirancang untuk mempermudah pembuatan konten video berbasis epigraf. Jika ada kendala atau Anda ingin mengembangkan fitur tambahan, silakan hubungi kami.
