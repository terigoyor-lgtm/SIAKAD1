# SIAKAD Sekolah — Admin Panel Front-End

Proyek demonstrasi **Pemrograman Web 2 (Client-Side Programming)** untuk tema Sistem Informasi Akademik Sekolah (SIAKAD). Antarmuka menggunakan pendekatan **Material Design**: warna primer biru, permukaan/kartu, jarak konsisten, tipografi Inter, navigasi responsif, dan komponen dengan status yang jelas.

## Fitur

- Halaman login demo.
- Dashboard ringkasan siswa, guru, kelas, aktivitas, dan grafik siswa per kelas.
- Data master siswa: pencarian, filter kelas/status, tambah, edit, hapus dengan modal konfirmasi.
- Validasi NIS unik, nama, email, kelas, status, serta nilai rata-rata 0–100.
- Laporan dengan filter, cetak, dan ekspor CSV yang dapat dibuka melalui Excel atau spreadsheet.
- Sidebar responsif untuk desktop dan perangkat mobile.
- Mock data awal dan penyimpanan perubahan menggunakan `localStorage` browser.

## Menjalankan proyek

1. Ekstrak ZIP proyek.
2. Buka folder `siakad-admin` menggunakan Visual Studio Code atau editor pilihan.
3. Jalankan `index.html` dengan ekstensi Live Server (disarankan), atau buka langsung di browser.
4. Masuk menggunakan akun demo:
   - **Username:** `admin`
   - **Password:** `admin123`
5. Coba menu Dashboard, Data Master Siswa, Tambah Siswa, dan Laporan Akademik.

> Catatan: Grafik memakai Chart.js dari CDN sehingga grafik memerlukan koneksi internet. Fitur data utama tetap dapat dicoba tanpa database server. Data siswa hanya tersimpan di browser/perangkat yang dipakai.

## Struktur folder

```text
siakad-admin/
├── index.html
├── README.md
├── docs/
│   ├── PERANCANGAN.md
│   ├── wireframe-dashboard.svg
│   └── wireframe-data-master.svg
├── assets/
│   ├── css/style.css
│   ├── js/
│   │   ├── common.js
│   │   ├── dashboard.js
│   │   ├── data.js
│   │   ├── login.js
│   │   ├── reports.js
│   │   ├── student-form.js
│   │   └── students.js
│   └── img/
└── pages/
    ├── dashboard.html
    ├── data-master.html
    ├── form.html
    ├── layout.html
    └── laporan.html
```

## Deploy ke GitHub Pages atau Vercel

1. Buat repository baru di GitHub.
2. Upload seluruh isi folder proyek ini (termasuk `index.html`, `pages`, `assets`, dan `docs`).
3. Untuk GitHub Pages: buka **Settings → Pages**, pilih branch utama dan folder root, kemudian simpan.
4. Untuk Vercel: impor repository GitHub baru ke Vercel. Tidak membutuhkan build command untuk proyek HTML/CSS/JS statis; output directory gunakan root proyek.
5. Uji tautan setelah deploy, terutama login dan navigasi ant halaman.

## Yang perlu dilengkapi sendiri sebelum dikumpulkan

- Ganti identitas sekolah dan data contoh jika dosen meminta identitas tertentu.
- Buka `docs/PERANCANGAN.md` dan tambahkan tautan publik project Figma/Stitch milik sendiri. File wireframe SVG yang ada adalah acuan tata letak lokal, bukan tautan project Figma/Stitch yang telah diterbitkan.
- Ambil screenshot hasil rancangan final dari Figma/Stitch dan lampirkan di dokumentasi/repositori jika diwajibkan dosen.
- Sesuaikan struktur menu dan komponen berdasarkan feedback dosen.

## Batasan demo

Tidak menggunakan backend atau database server. Login hanya simulasi sisi klien dan **bukan autentikasi aman untuk aplikasi produksi**. Jangan gunakan password atau data siswa sebenarnya.
