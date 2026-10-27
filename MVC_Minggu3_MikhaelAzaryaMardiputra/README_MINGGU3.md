# Laporan Praktikum Pemrograman Framework - Minggu 3 (MVC)
- **Mata Kuliah:** Pemrograman Framework (RPL512203)[cite: 1]
- **Nama:** Mikhael Azarya Mardiputra[cite: 9]
- **NIM:** C2455201057[cite: 9]
- **Kelas/Semester:** S-1 Teknik Informatika / Semester V[cite: 1, 9]

---

## 1. Environment & Teknologi
- **PHP Version:** ( Jalankan `php -v` di terminal Laragon )[cite: 3, 9]
- **Framework:** Laravel (pada environment Laragon Windows)[cite: 3]
- **Web Server:** Apache / Nginx (Laragon)[cite: 3]

---

## 2. Struktur File MVC yang Dibuat
- **Model:** `app/Models/KegiatanModel.php` (Menyediakan data contoh array kegiatan lengkap dengan kuota dan lokasi)[cite: 3, 5, 8, 9]
- **Controller:** 
  - `app/Http/Controllers/SapaController.php` (Menangani endpoint sapa statis dan parameter)[cite: 3, 4]
  - `app/Http/Controllers/KegiatanController.php` (Menangani logika katalog dan detail kegiatan serta validasi 404)[cite: 3, 6]
- **View & Partials:**
  - `resources/views/partials/header.blade.php`[cite: 3, 7]
  - `resources/views/partials/footer.blade.php`[cite: 3, 7]
  - `resources/views/sapa.blade.php`[cite: 3, 4]
  - `resources/views/kegiatan/index.blade.php`[cite: 3, 7]
  - `resources/views/kegiatan/detail.blade.php`[cite: 3, 7]
- **Routing:** `routes/web.php`[cite: 3, 4]

---

## 3. Langkah Menjalankan Aplikasi
1. Pastikan layanan server di aplikasi **Laragon** sudah dalam status *Start All*[cite: 3].
2. Buka terminal atau Command Prompt pada direktori project Anda[cite: 3].
3. Jalankan server lokal Laravel (jika tidak menggunakan auto-domain Laragon):
   ```bash
   php artisan serve