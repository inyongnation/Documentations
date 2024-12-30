# Langkah-langkah Instalasi Kali Linux dengan Andronix di Termux (CLI Only)

## 1. Update dan Install Paket Termux
Jalankan perintah ini untuk memperbarui repositori dan paket:

```bash
pkg update && pkg upgrade
pkg install wget proot tar -y
```

## 2. Unduh dan Jalankan Skrip Andronix
Skrip Andronix memungkinkan Anda untuk menginstal berbagai distribusi Linux, termasuk Kali Linux, di Termux. Gunakan perintah berikut:

```bash
wget https://raw.githubusercontent.com/AndronixApp/AndronixOrigin/master/Installer/Kali/kali.sh
```

## 3. Berikan Izin Eksekusi dan Jalankan Skrip
Setelah skrip berhasil diunduh, beri izin eksekusi dan jalankan skrip dengan perintah:

```bash
chmod +x kali.sh
./kali.sh
```

## 4. Masuk ke Kali Linux
Setelah skrip selesai berjalan, Anda dapat masuk ke lingkungan Kali Linux dengan perintah berikut:

```bash
./start-kali.sh
```

Dengan ini, Anda akan mendapatkan akses ke lingkungan Kali Linux CLI langsung dari Termux tanpa menggunakan NetHunter.
