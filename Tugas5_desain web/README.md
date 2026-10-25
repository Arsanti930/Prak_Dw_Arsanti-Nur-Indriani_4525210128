# Wireframe Toko Online - Layout & Anotasi

## Identitas Mahasiswa

| Keterangan        | Isi                                    |
| ----------------- | -------------------------------------- |
| **Nama**          | ARSANTI NUR INDRIANI                   |
| **NPM**           | 4525210128                             |
| **Program Studi** | Teknik Informatika                     |
| **Semester**      | 3                                      |
| **Kampus**        | Fakultas Teknik, Universitas Pancasila |

---

## Deskripsi

Proyek ini adalah **wireframe halaman utama Toko Online** yang dibuat dengan HTML dan CSS. Wireframe berfokus pada **tata letak (layout)** dan **anotasi** di setiap bagian halaman, bukan pada tampilan visual akhir. Konten masih berupa *placeholder* seperti `[ LOGO TOKO ]` dan `Rp XXX.XXX`.

## Struktur Layout

| Bagian               | Tag HTML    | Fungsi                                                                                         |
| -------------------- | ----------- | ---------------------------------------------------------------------------------------------- |
| **Header**           | `<header>`  | Logo toko, kolom pencarian, keranjang `Cart (0)`, dan akun pengguna                            |
| **Navigasi**         | `<nav>`     | Menu kategori produk (Kategori 1-3) dan Promo                                                  |
| **Hero Banner**      | `<section>` | Banner promosi utama dengan tombol ajakan bertindak (CTA) "Belanja Sekarang"                   |
| **Produk Terpopuler**| `<main>`    | Grid 4 kartu produk, masing-masing berisi gambar, nama, harga, dan tombol "+ Keranjang"        |
| **Footer**           | `<footer>`  | Tiga kolom informasi (tentang kami, layanan pelanggan, metode pembayaran) dan hak cipta        |

Setiap bagian dilengkapi blok **anotasi** (`.annotation`) yang menjelaskan fungsi bagian tersebut.

## Class CSS yang Digunakan

- `.wireframe-block` : pembungkus setiap blok layout
- `.annotation` : catatan penjelasan fungsi tiap bagian
- `.brand`, `.search-bar`, `.nav-icons` : elemen di dalam header
- `.hero` : bagian banner promosi
- `.btn-placeholder` : tombol *placeholder*
- `.product-grid`, `.product-card`, `.img-box` : grid dan kartu produk
- `.footer-cols` : kolom-kolom pada footer

## Struktur Berkas

```
TokoOnline/
├── TokoOnline.html   # Halaman wireframe
├── style.css         # Stylesheet
└── README.md         # Dokumentasi proyek
```

> **Catatan:** `TokoOnline.html` memanggil `style.css`, jadi kedua berkas harus berada dalam satu folder.

## Cara Menjalankan

1. Clone atau unduh repositori ini.
2. Pastikan `TokoOnline.html` dan `style.css` berada dalam satu folder.
3. Buka `TokoOnline.html` di browser (klik dua kali, atau gunakan ekstensi *Live Server* di VS Code).

## Teknologi

- HTML5
- CSS3
- Visual Studio Code

---

&copy; 2026 **Arsanti Nur Indriani** (4525210128) — Fakultas Teknik, Universitas Pancasila.