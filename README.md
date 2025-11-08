# Super App Kenang (Web) 🎨🔥

Versi web-friendly dari aplikasi Flutter sederhana dengan tema **merah → oranye**, animasi, dan splash screen.
Terdiri dari 3 halaman: **Login**, **Dashboard**, **Profile**.

## Fitur
- Splash screen singkat (2 detik)
- Animasi transisi antarhalaman (fade + slide)
- Tema gradien merah → oranye
- Responsif untuk web & mobile
- Siap untuk di-push ke GitHub dan di-deploy ke GitHub Pages

## Cara Menjalankan (lokal)
Pastikan sudah menginstal Flutter dan browser (Chrome).

1. Buka terminal di folder proyek.
2. Ambil dependency:
```bash
flutter pub get
```
3. Jalankan di Chrome:
```bash
flutter run -d chrome
```

## Build untuk Web
```bash
flutter build web
```
Hasil build akan berada di `build/web/`. Untuk deploy ke GitHub Pages, kamu bisa:
1. Buat repo GitHub dan push seluruh project.
2. Build web (`flutter build web`).
3. Push isi folder `build/web` ke branch `gh-pages` (bisa manual atau pakai `gh-pages` action).

Contoh (manual):
```bash
# dari root project
flutter build web
cd build/web
git init
git add .
git commit -m "Deploy web build"
git branch -M gh-pages
git remote add origin https://github.com/<username>/super_app_kenang_web.git
git push -f origin gh-pages
```

---
Dibuat otomatis oleh Super AI untuk Kenang Dheanirham Setyanto.