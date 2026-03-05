# ChatApp Backend (Vercel Functions)

Backend API untuk aplikasi chat, dideploy ke Vercel project `chatapp-backend`.

## Endpoint Utama

- `GET /api/users`
- `GET /api/conversations`

## Jalankan Lokal

1. Masuk folder project:
   ```bash
   cd chatpp-backend
   ```
2. Copy `.env.example` jadi `.env`, lalu isi kredensial database.
3. Install dependency:
   ```bash
   npm install
   ```
4. Jalankan server lokal:
   ```bash
   npm start
   ```
5. Test endpoint:
   - `http://localhost:3000/api/users`
   - `http://localhost:3000/api/conversations`

## Push ke GitHub Repo `chatapp-backend`

Contoh jika remote belum ada:

```bash
git init
git add .
git commit -m "setup backend for vercel"
git branch -M main
git remote add origin https://github.com/<username>/chatapp-backend.git
git push -u origin main
```

Jika remote sudah ada:

```bash
git add .
git commit -m "update backend for vercel"
git push
```

## Deploy ke Vercel Project `chatapp-backend`

1. Import repo `chatapp-backend` di Vercel.
2. Tambahkan Environment Variables:
   - `DB_HOST`
   - `DB_USER`
   - `DB_PASSWORD`
   - `DB_NAME`
   - `DB_PORT`
3. Deploy.

## Integrasi ke Frontend Astro

Di project frontend (`chatapp`), set:

```env
PUBLIC_API_BASE_URL=https://chatapp-backend-lh6y8i35j-zzanarif16s-projects.vercel.app
```

Frontend production saat ini:

- `https://chatapp-ekwhv4a7b-zzanarif16s-projects.vercel.app/`
