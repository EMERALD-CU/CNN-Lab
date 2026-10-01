# CNN Klasifikasi Citra Biner (Cats vs Dogs) - Tugas Praktik Sesi 6

Repositori ini memuat implementasi Convolutional Neural Network (CNN) dari awal (scratch) menggunakan PyTorch untuk mengklasifikasikan gambar Kucing dan Anjing. Proyek ini dibangun untuk memenuhi Tugas Praktik Sesi 6.

## Lingkungan Pengembangan (Environment)
*   **Library Utama:** 
    *   `torch`, `torchvision` (PyTorch)
    *   `scikit-learn` (Evaluasi metrik)
    *   `matplotlib` (Visualisasi kurva)
    *   `Pillow` (Pemrosesan gambar awal)
    *   `kagglehub` (Pengunduhan dataset otomatis)

**Instalasi Dependensi:**
Jalankan perintah berikut pada terminal Anda:
```bash
pip install torch torchvision scikit-learn matplotlib pillow kagglehub
```

**Catatan Eksekusi:** 
   * Anda tidak perlu mengunduh dataset secara manual. Skrip akan otomatis memanggil `kagglehub.dataset_download` untuk menarik dataset Kaggle `shaunthesheep/microsoft-catsvsdogs-dataset` dan menyimpannya di cache lokal.
   * Proses verifikasi ~25.000 gambar akan berjalan di awal komputasi dan memakan waktu sekitar 2–5 menit. Jangan hentikan program secara paksa (Ctrl+C) selama tahap ini.
   * Setelah pelatihan selesai, program akan otomatis menampilkan grafik kurva *Loss* dan visualisasi 3 gambar misklasifikasi.