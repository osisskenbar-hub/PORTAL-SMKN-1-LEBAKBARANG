# Skenbar Learning Portal – APK

Aplikasi Android (WebView) yang membuka portal:
https://script.google.com/macros/s/AKfycbyDjI6KkQivX4J-EcnaO6P5mfcfHY0xFTXMdtcsA6EPj183xVUCuu_BNOJ6hkNzXvcBJg/exec

## Cara membuat APK (Android Studio)
1. Install Android Studio (https://developer.android.com/studio).
2. File → Open → pilih folder `skenbar-apk`. Tunggu proses Gradle Sync selesai.
3. Build → Build Bundle(s) / APK(s) → Build APK(s).
4. File APK ada di `app/build/outputs/apk/debug/app-debug.apk`.
5. Kirim file tersebut ke HP dan install (aktifkan "Install dari sumber tidak dikenal").

Untuk APK rilis (release): Build → Generate Signed App Bundle / APK → APK, lalu buat keystore.

## Catatan
- Ikon aplikasi memakai logo SMKN 1 Lebakbarang.
- Tarik layar ke bawah untuk memuat ulang halaman.
- Tombol kembali membuka halaman sebelumnya di dalam portal.
- Tautan ke situs luar dibuka di browser.

## Build APK gratis secara online (GitHub Actions)
1. Buat akun di https://github.com (gratis).
2. Buat repository baru (boleh public atau private), lalu upload seluruh isi folder `skenbar-apk` (termasuk folder `.github`).
3. Buka tab **Actions** di repository, pilih workflow **Build APK**, lalu klik **Run workflow** (atau cukup push ke branch `main`).
4. Tunggu sekitar 5–10 menit sampai status hijau.
5. Klik hasil run tersebut, lalu unduh **skenbar-portal-apk** di bagian Artifacts. Di dalamnya ada `app-debug.apk`.
6. Kirim APK ke HP (lewat WhatsApp, Google Drive, atau tautan) dan install.
