# Laravel Movie Database

## About Laravel Movie DB

Ini adalah sistem basis data film yang dibangun dengan Laravel untuk mata kuliah Konstruksi dan Evolusi Perangkat Lunak pada Program Teknologi Rekayasa Perangkat Lunak, Jurusan Teknologi Informasi, Politeknik Negeri Padang.

## Perubahan Refactoring

Basis kode telah mengalami perbaikan signifikan untuk meningkatkan kualitas kode, kemudahan perawatan, dan keamanan. Perbaikan berikut telah diterapkan:

### 1. Pembuatan URL yang Konsisten
- Mengganti URL hardcoded dengan rute bernama Laravel menggunakan helper `route()`
- Menambahkan nama rute yang hilang dalam file rute
- Meningkatkan kemudahan perawatan dengan memusatkan definisi rute

### 2. Pola Akses Data yang Konsisten
- Akses properti model terstandarisasi menggunakan notasi objek (`$movie->property`) alih-alih mencampurnya dengan notasi array
- Peningkatan keterbacaan kode dan pengurangan potensi kesalahan

### 3. Penanganan Gambar yang Ditingkatkan
- Menerapkan helper `asset()` untuk semua jalur gambar
- Menambahkan teks alt deskriptif untuk gambar guna meningkatkan aksesibilitas
- Konstruksi jalur gambar terpusat

### 4. Struktur Bentuk yang Ditingkatkan
- Menambahkan tampilan kesalahan validasi ke semua formulir
- Menerapkan retensi input lama untuk menyimpan input pengguna pada kesalahan validasi
- Menambahkan tindakan dan metode formulir yang konsisten
- Menambahkan tombol batal/kembali untuk pengalaman pengguna yang lebih baik

### 5. Peningkatan Keamanan
- Menerapkan perlindungan CSRF yang tepat untuk semua formulir
- Mengubah operasi penghapusan dari GET ke permintaan POST/DELETE
- Menambahkan dialog konfirmasi untuk tindakan yang merusak

### 6. Organisasi Kode
- Mengurangi duplikasi kode di seluruh tampilan
- Peningkatan konsistensi penamaan
- Peningkatan keterbacaan dengan indentasi dan spasi yang tepat
