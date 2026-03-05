# Chatpp Backend (Express.js)

Backend API untuk aplikasi chat, menggunakan Express.js dan MySQL Clever Cloud.

## Fitur

- Koneksi ke database MySQL Clever Cloud
- Endpoint contoh: /api/users, /api/conversations
- Siap dikembangkan untuk fitur chat, kontak, grup, dsb

## Struktur Project

- `index.js` — Main Express app
- `.env.example` — Contoh konfigurasi environment
- `package.json` — Konfigurasi npm

## Cara Menjalankan Lokal

1. Clone repo ini:
   ```bash
   git clone https://github.com/zzanarif16/chatpp-backend.git
   cd chatpp-backend
   ```
2. Copy file `.env.example` menjadi `.env` dan isi dengan kredensial MySQL Clever Cloud Anda.
3. Install dependencies:
   ```bash
   npm install
   ```
4. Jalankan server:
   ```bash
   node index.js
   ```
5. Cek endpoint: [http://localhost:3000/api/users](http://localhost:3000/api/users)

## Deploy ke Railway/Render

1. Buat project baru di Railway/Render.
2. Upload semua file backend.
3. Atur environment variable sesuai file `.env`.
4. Deploy, dapatkan URL backend API publik.

## Integrasi dengan Frontend

- Frontend (Astro) fetch data dari endpoint API backend ini.
- Pastikan backend dapat diakses publik (bukan localhost).

## Lisensi

Bebas digunakan untuk pembelajaran dan pengembangan.
