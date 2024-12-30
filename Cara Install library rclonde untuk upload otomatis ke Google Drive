# Langkah-langkah Instalasi Rclone di Kali Linux untuk Android dan Setting ke Google Drive

## 1. Instalasi Rclone

### a. Update dan Instal Paket yang Dibutuhkan
Pastikan sistem Anda telah diperbarui dan instal paket yang diperlukan:

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install curl unzip -y
```

### b. Unduh dan Ekstrak Rclone
Unduh file rclone dari situs resminya:

```bash
curl -O https://downloads.rclone.org/rclone-current-linux-arm.zip
unzip rclone-current-linux-arm.zip
cd rclone-*
```

### c. Pindahkan Biner Rclone ke Path Sistem
Pindahkan biner rclone ke direktori `/usr/bin/`:

```bash
sudo cp rclone /usr/bin/
sudo chmod +x /usr/bin/rclone
```

### d. Verifikasi Instalasi Rclone
Periksa apakah rclone telah terinstal dengan benar:

```bash
rclone version
```

## 2. Konfigurasi Rclone untuk Google Drive

### a. Mulai Konfigurasi
Jalankan perintah konfigurasi:

```bash
rclone config
```

### b. Buat Remote Baru
Ikuti langkah-langkah ini:

1. Ketik `n` untuk membuat remote baru.
2. Berikan nama untuk remote, misalnya `gdrive`.
3. Pilih jenis penyimpanan: ketik `13` (Google Drive).
4. Biarkan client_id dan client_secret kosong (tekan Enter).
5. Pilih akses yang Anda inginkan, misalnya `1` untuk akses penuh.
6. Biarkan root_folder_id dan service_account_file kosong (tekan Enter).
7. Ketik `n` jika Anda tidak ingin menggunakan editor otomatis.

### c. Autentikasi ke Google Drive

1. Rclone akan memberikan URL, salin URL tersebut dan buka di browser.
2. Login ke akun Google Anda dan izinkan akses.
3. Salin kode autentikasi yang diberikan dan tempelkan di terminal.

### d. Verifikasi dan Simpan Konfigurasi
Setelah autentikasi berhasil:

1. Ketik `y` untuk menyimpan konfigurasi.
2. Ketik `q` untuk keluar dari wizard konfigurasi.

## 3. Uji Remote Google Drive
Verifikasi koneksi ke Google Drive dengan perintah berikut:

```bash
rclone ls gdrive:
```

Jika berhasil, Anda akan melihat daftar file dan folder di Google Drive Anda.
