# Accounting Hub 2026

PWA + Android APK build for the four Accounting/Finance Excel reports.

## Struktur
- `www/` — aplikasi PWA dan data JSON
- `capacitor.config.json` — konfigurasi APK Android
- `package.json` — dependency Capacitor
- `.github/workflows/android.yml` — build APK otomatis
- `.github/workflows/pages.yml` — deploy ke GitHub Pages

## Cara pakai di GitHub
1. Buat repository baru, misalnya `accounting-hub-2026`.
2. Upload seluruh isi folder ini ke branch `main`.
3. Buka **Settings → Pages** dan pilih **GitHub Actions** sebagai source.
4. Jalankan workflow **Build Accounting Hub APK** dari tab **Actions**.
5. Setelah selesai, buka workflow tersebut → **Artifacts** → download `accounting-hub-2026-apk`.

APK yang dihasilkan adalah **debug APK** untuk instalasi/pengujian. Untuk APK release yang ditandatangani dan siap distribusi, tambahkan Android ke repo secara permanen dan gunakan signing keystore di GitHub Secrets.
