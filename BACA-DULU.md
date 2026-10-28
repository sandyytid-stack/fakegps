# Fake GPS: bangun APK tanpa Android Studio (lewat GitHub)

1. Buat akun di github.com (gratis), lalu **New repository** (nama bebas, mis. fakegps, Public atau Private).
2. Ekstrak zip ini. Di halaman repo: **Add file > Upload files**, seret SEMUA isi folder fakegps
   (app, build.gradle.kts, settings.gradle.kts, gradle.properties), lalu **Commit changes**.
3. File workflow ada di folder tersembunyi `.github`. Kalau tidak ikut terunggah:
   **Add file > Create new file**, isi nama `.github/workflows/build.yml`,
   salin isi file `build.yml` dari zip, lalu Commit.
4. Buka tab **Actions**. Build jalan otomatis (sekitar 3-6 menit). Tunggu sampai ada tanda centang hijau.
5. Klik build tersebut, turun ke **Artifacts**, unduh **fakegps-apk** (zip berisi app-debug.apk).
6. Ekstrak, kirim `app-debug.apk` ke ponsel, pasang (izinkan sumber tidak dikenal).
7. Sekali saja: Opsi Pengembang > Pilih aplikasi lokasi palsu > Fake GPS.
