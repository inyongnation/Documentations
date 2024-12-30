# Panduan Lengkap Mendapatkan API Key Pexels

Pexels menyediakan API gratis yang memungkinkan Anda mengakses jutaan foto dan video berkualitas tinggi untuk proyek Anda. Berikut adalah langkah-langkah lengkap untuk mendapatkan API Key Pexels:

## Langkah 1: Membuat Akun Pexels
1. **Kunjungi Situs Web Pexels**
   - Buka [https://www.pexels.com/](https://www.pexels.com/).

2. **Daftar atau Login**
   - Jika Anda belum memiliki akun, klik tombol `Join Free` di pojok kanan atas.
   - Isi formulir pendaftaran dengan email, nama, dan kata sandi, atau daftar menggunakan akun Google atau Facebook.
   - Jika Anda sudah memiliki akun, klik `Log In` dan masukkan kredensial Anda.

## Langkah 2: Mengakses Halaman API
1. **Buka Halaman API Pexels**
   - Setelah login, navigasikan ke [https://www.pexels.com/api/](https://www.pexels.com/api/).

2. **Klik Tombol "Get Started"**
   - Pada halaman tersebut, klik tombol `Get Started` untuk memulai proses pengajuan API.

## Langkah 3: Mendapatkan API Key
1. **Isi Informasi Aplikasi Anda**
   - Pada halaman aplikasi API, masukkan nama aplikasi atau proyek Anda.
   - Deskripsikan secara singkat tujuan penggunaan API, seperti "Membuat aplikasi pencarian gambar" atau "Menggunakan foto Pexels untuk pembuatan video."

2. **Setujui Ketentuan Penggunaan**
   - Centang kotak persetujuan untuk menerima `Terms and Conditions`.

3. **Kirim Permohonan**
   - Klik tombol `Submit`.

4. **Salin API Key Anda**
   - Setelah permohonan disetujui, Anda akan mendapatkan API Key unik Anda.
   - Salin API Key tersebut dan simpan di tempat yang aman.

## Langkah 4: Mulai Menggunakan API
1. **Baca Dokumentasi API**
   - Kunjungi [Dokumentasi API Pexels](https://www.pexels.com/api/documentation/) untuk mempelajari cara menggunakan endpoint, parameter, dan fitur API.

2. **Uji API Key Anda**
   - Gunakan tool seperti Postman atau cURL untuk menguji API Key Anda.
   - Contoh permintaan API untuk mencari gambar:
     ```bash
     curl -H "Authorization: Bearer API_KEY_ANDA" \
     "https://api.pexels.com/v1/search?query=nature&per_page=1"
     ```

3. **Integrasikan ke dalam Proyek Anda**
   - Tambahkan API Key ke aplikasi Anda sesuai dengan kebutuhan proyek.

## Tips Keamanan
- **Jangan Bagikan API Key Anda**
  - Pastikan API Key hanya digunakan dalam aplikasi Anda dan tidak diunggah ke repositori publik.
- **Gunakan Variabel Lingkungan**
  - Simpan API Key dalam variabel lingkungan untuk menghindari kebocoran data.

## Bantuan dan Dukungan
Jika Anda menghadapi masalah:
- Kunjungi [Halaman Bantuan Pexels](https://help.pexels.com/hc/en-us).
- Hubungi tim dukungan melalui email yang tersedia di situs.

Anda sekarang siap menggunakan API Pexels untuk mengakses gambar dan video berkualitas tinggi untuk proyek Anda!
