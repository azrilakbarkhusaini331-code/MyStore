MyStore Android Project — build APK gratis melalui GitHub Actions

ISI
- Proyek Android Java dengan WebView yang memuat aplikasi MyStore dari assets/index.html.
- Workflow GitHub Actions untuk membangun APK debug otomatis.
- APK belum dibangun di dalam paket ZIP ini. APK akan dibuat oleh workflow setelah proyek diunggah ke repository GitHub.

LANGKAH DARI HP ANDROID
1. Unduh dan ekstrak ZIP ini.
2. Masuk ke github.com melalui browser dan buat akun / masuk.
3. Buat repository baru bernama MyStore, sebaiknya Private selama pengujian.
4. Unggah semua file dan folder di dalam folder MyStore_Android_Project ke repository. Pastikan folder .github/workflows ikut terunggah (GitHub kadang menyembunyikan folder bertitik; gunakan tampilan Desktop jika perlu).
5. Buka tab Actions pada repository. Pilih "Build MyStore APK", lalu tekan Run workflow. Jika workflow tidak terlihat, pastikan file .github/workflows/build-apk.yml berada di branch main.
6. Tunggu workflow selesai dengan status hijau. Buka run yang selesai, scroll ke Artifacts, lalu unduh "MyStore-debug-apk".
7. Ekstrak artifact ZIP, lalu buka app-debug.apk di HP. Android mungkin meminta izin instal aplikasi dari sumber tersebut; aktifkan hanya untuk browser/file manager yang digunakan dan nonaktifkan kembali sesudahnya.
8. Uji dengan data contoh. Jangan masukkan data toko nyata sampai sudah memiliki rencana backup.

CATATAN
- Ini APK debug untuk uji coba, bukan rilis Google Play yang ditandatangani dengan kunci produksi.
- APK dibangun di GitHub Actions; tidak ada APK final di ZIP ini.
- Data disimpan lokal di WebView perangkat. Data tidak tersinkron, dan bisa hilang jika data aplikasi dihapus. Ekspor JSON dari menu Laporan secara berkala.
- Aplikasi tidak meminta izin internet atau izin sensitif karena fitur dasarnya offline.
- Untuk publikasi komersial, lakukan pengujian keamanan, backup, privasi, dan penandatanganan release yang sesuai.
