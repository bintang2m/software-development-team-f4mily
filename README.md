<p align="center">
  <img src="banner.png" alt="Novel Ku Banner" width="100%">
</p>

# Novel Ku

**Novel Ku** adalah platform membaca dan menulis novel digital yang dibangun menggunakan framework Laravel. Platform ini memfasilitasi interaksi antara pembaca dan penulis dalam satu wadah yang mudah digunakan, dilengkapi dengan berbagai fitur interaktif dan sistem manajemen konten yang komprehensif.

## Fitur Utama

### 1. Pengguna Publik (Guest)
- **Eksplorasi Novel:** Jelajahi berbagai macam novel berdasarkan genre dan popularitas.
- **Membaca Novel:** Akses dan baca bab-bab novel yang tersedia.
- **Profil Pengguna:** Lihat profil para penulis dan karya-karyanya.

### 2. Pembaca Terautentikasi (Reader)
- **Dashboard Personal:** Ringkasan aktivitas seperti riwayat membaca, jumlah bookmark, dan rekomendasi.
- **Sistem Interaksi:** Berikan komentar pada bab, *like* komentar pengguna lain, dan tulis ulasan (rating & review) untuk novel.
- **Bookmark & Riwayat:** Simpan novel favorit ke daftar *bookmark* untuk dibaca nanti dan pantau riwayat bacaan.
- **Kotak Masuk (Inbox):** Terima notifikasi terkait aktivitas interaksi dan pembaruan karya.
- **Pelaporan (Report):** Fitur untuk melaporkan novel atau komentar yang tidak pantas (melanggar ketentuan).
- **Manajemen Profil:** Edit dan perbarui profil pengguna secara mandiri.

### 3. Penulis (Writer)
- Semua fitur Pembaca, ditambah:
- **Manajemen Novel:** Buat, perbarui, dan kelola karya novel sendiri.
- **Manajemen Bab (Chapter):** Tambahkan bab-bab baru, kelola urutan, dan unggah gambar ilustrasi untuk bab.
- **Statistik Karya:** Pantau jumlah penayangan (*views*), jumlah interaksi, dan performa dari masing-masing novel.

### 4. Administrator
- **Dashboard Admin:** Pemantauan dan ringkasan seluruh aktivitas di dalam platform.
- **Manajemen Pengguna:** Kelola akun pembaca, penulis, dan admin lainnya.
- **Manajemen Konten Utama:** Kelola daftar Genre dan awasi seluruh novel yang dipublikasikan.
- **Moderasi Platform:** Kelola dan tindak lanjuti pelaporan pengguna (*reports*), serta menghapus komentar/ulasan yang melanggar aturan.
- **Manajemen Banner:** Mengatur banner promosi yang tampil di halaman utama platform.

## Teknologi yang Digunakan
- **Backend:** Laravel 12 (PHP ^8.2)
- **Frontend:** Tailwind CSS, Alpine.js, Vite
- **Database:** MySQL / SQLite
- **Autentikasi & Keamanan:** Laravel Breeze

## Cara Instalasi & Menjalankan Proyek Secara Lokal

1. **Clone repository ini**
   ```bash
   git clone <url-repository-anda>
   cd novel_Ku_1
   ```

2. **Install dependensi PHP & Node.js**
   Pastikan Anda sudah menginstal Composer dan Node.js di komputer Anda.
   ```bash
   composer install
   npm install
   ```

3. **Konfigurasi Environment**
   Salin file `.env.example` menjadi `.env`.
   ```bash
   cp .env.example .env
   ```
   Lalu buka file `.env` dan sesuaikan konfigurasi database Anda (misalnya `DB_CONNECTION`, `DB_DATABASE`, `DB_USERNAME`, dll).

4. **Generate Application Key**
   ```bash
   php artisan key:generate
   ```

5. **Jalankan Migrasi Database**
   Untuk membuat tabel-tabel di database (tambahkan `--seed` jika Anda memiliki data seeder).
   ```bash
   php artisan migrate
   ```

6. **Jalankan Development Server**
   Jalankan Vite untuk kompilasi *asset* frontend:
   ```bash
   npm run dev
   ```
   Buka terminal/tab baru, lalu jalankan server Laravel:
   ```bash
   php artisan serve
   ```

7. **Akses Aplikasi**
   Buka browser web Anda dan kunjungi `http://localhost:8000`.

## Tim Pengembang
Dikembangkan oleh **Kelompok 13** sebagai proyek pengembangan web.

---
*Proyek ini dirancang untuk memberikan pengalaman membaca dan merilis karya fiksi dengan ekosistem yang terkelola dengan baik.*
