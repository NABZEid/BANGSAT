# APK Builder

Aplikasi Android (WebView) untuk membuat APK lewat GitHub Actions. Login lewat akun dari bot Telegram.

## Cara mendapatkan APK

1. Buat repo baru di GitHub, lalu upload seluruh isi folder ini (termasuk folder `.github`).
   Paling mudah lewat browser di komputer atau `git push` (Termux juga bisa).
2. Buka tab Actions, jalankan workflow "Build APK" (otomatis jalan saat push ke `main`).
3. Setelah selesai (sekitar 3-6 menit), APK ada di halaman Releases repo itu.

## Mengatur server login

Ubah `app/src/main/assets/config.js` lalu isi `LOGIN_API` dengan alamat server bot.
Bisa juga dikosongkan dulu: alamat bisa diisi dari layar login aplikasi lewat menu "Server".

## Kontrak API server login

Lihat file PROMPT_BOT_TELEGRAM.md (endpoint /api/login, /api/verify, /api/logout).
