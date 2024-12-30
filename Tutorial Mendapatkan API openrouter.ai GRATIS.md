# Panduan Lengkap Mendapatkan API dari OpenRouter.ai

## Pendahuluan
OpenRouter.ai adalah platform API yang memungkinkan Anda untuk menggunakan model AI canggih seperti GPT untuk berbagai aplikasi. Untuk menggunakan API dari OpenRouter.ai, Anda memerlukan **API Key** yang dapat diperoleh melalui proses pendaftaran di situs web resmi mereka. Artikel ini akan memandu Anda langkah demi langkah untuk mendapatkan API Key tersebut.

---

## Langkah-Langkah Mendapatkan API dari OpenRouter.ai

### 1. Kunjungi Situs Web OpenRouter.ai
- Buka browser favorit Anda.
- Masuk ke halaman utama OpenRouter.ai melalui URL berikut:
  ```
  https://openrouter.ai
  ```

---

### 2. Daftar Akun Baru atau Login
- Jika Anda belum memiliki akun:
  1. Klik tombol **Sign Up** di pojok kanan atas.
  2. Isi formulir pendaftaran dengan informasi berikut:
     - Nama lengkap
     - Email aktif
     - Kata sandi
  3. Verifikasi email Anda dengan membuka tautan yang dikirimkan ke kotak masuk email.

- Jika Anda sudah memiliki akun:
  1. Klik tombol **Login**.
  2. Masukkan email dan kata sandi Anda.

---

### 3. Akses Halaman API Key
- Setelah login, navigasikan ke menu **Dashboard** atau **API Management**.
- Klik tab atau opsi yang bertuliskan **API Keys**.

---

### 4. Generate API Key
1. Klik tombol **Create New API Key** atau **Generate API Key**.
2. Berikan deskripsi singkat untuk API Key Anda (misalnya: "Project Video Generator").
3. Klik **Generate**.
4. API Key Anda akan muncul di layar. **Catatan penting:**
   - Salin API Key tersebut dan simpan di tempat yang aman.
   - Jangan bagikan API Key Anda kepada siapa pun.

---

### 5. Konfigurasi Penggunaan API Key
Setelah mendapatkan API Key, Anda dapat menggunakannya untuk mengakses layanan API dari OpenRouter.ai. Gunakan API Key ini dalam header setiap permintaan API Anda:

```bash
Authorization: Bearer <API_KEY_ANDA>
```

---

### 6. Uji Coba API Key Anda
Anda dapat menguji API Key dengan melakukan permintaan sederhana menggunakan alat seperti **Postman**, **curl**, atau langsung dalam aplikasi Anda. Berikut contoh permintaan menggunakan `curl`:

```bash
curl -X POST https://openrouter.ai/api/v1/chat/completions \
-H "Authorization: Bearer <API_KEY_ANDA>" \
-H "Content-Type: application/json" \
-d '{
  "model": "gpt-3.5",
  "messages": [{"role": "user", "content": "Halo, apa kabar?"}]
}'
```

---

## Tips Keamanan API Key
1. **Jaga Kerahasiaan API Key**
   - Jangan pernah menyimpan API Key dalam kode sumber yang dapat diakses publik (misalnya di GitHub).
   - Gunakan variabel lingkungan untuk menyimpan API Key dalam aplikasi Anda.

2. **Gunakan IP Whitelist (Jika Ada)**
   - Beberapa platform API menyediakan opsi untuk membatasi penggunaan API Key berdasarkan alamat IP tertentu.

3. **Monitor Penggunaan API Key**
   - Periksa dashboard Anda secara berkala untuk memastikan tidak ada aktivitas yang mencurigakan.

---

## Kesimpulan
Anda sekarang telah mengetahui cara mendapatkan API Key dari OpenRouter.ai dan langkah-langkah untuk menggunakannya dengan aman. Dengan API Key ini, Anda dapat mulai mengintegrasikan layanan AI OpenRouter ke dalam aplikasi Anda. Selamat mencoba!

---

## Referensi
- [OpenRouter.ai Official Website](https://openrouter.ai)
