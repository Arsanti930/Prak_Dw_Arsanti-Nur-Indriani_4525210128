# Tugas Praktikum Desain Web — Pertemuan 6

## Biodata Mahasiswa

| Keterangan | Identitas |
|---|---|
| Nama | Arsanti Nur Indriani |
| NIM | 4525210128 |
| Program Studi | Teknik Informatika |
| Mata Kuliah | Praktikum Desain Web A |
| Pertemuan | 6 — Mockup, Visual Hierarchy, Warna, dan Tipografi |

## Tujuan Tugas

Mengembangkan dashboard mahasiswa dari source `Contoh2` menggunakan HTML5 dan CSS3 murni. Struktur informasi utama tetap dipertahankan, yaitu navigasi, ringkasan akademik, jadwal, pengumuman, dan tabel mata kuliah. Visual dashboard disusun ulang dengan Simple Design System dan layout responsif untuk desktop maupun mobile.

## Fitur yang Dikerjakan

1. Dashboard mahasiswa dengan identitas Arsanti Nur Indriani dan NIM 4525210128.
2. Sidebar navigasi, ringkasan akademik, jadwal perkuliahan, pengumuman, serta tabel mata kuliah.
3. Halaman dokumentasi `design-system.html` yang menampilkan palet warna, tipografi, skala spacing, tombol, form controls, dan card.
4. Layout responsif menggunakan CSS Grid, Flexbox, dan media query.
5. Fokus keyboard dan struktur HTML semantik menggunakan `header`, `nav`, `main`, `section`, `aside`, dan `footer`.

## Struktur Folder

```text
pertemuan6/
├── Contoh1/                 # Source contoh dari materi
├── Contoh2/                 # Dashboard awal yang dikembangkan
├── quiz/                    # Latihan/kuis dari materi
└── Tugas/
    ├── css/
    │   └── style.css
    ├── DesignSystem/
    │   ├── design-system-desktop.png
    │   └── design-system-mobile.png
    ├── images/
    │   ├── before-desktop.png
    │   ├── before-mobile.png
    │   ├── after-desktop.png
    │   └── after-mobile.png
    ├── design-system.html
    ├── index.html
    └── README.md
```

## Simple Design System

| Area | Aturan |
|---|---|
| Colors | Primary `#185B55`, secondary `#D27A55`, accent `#8E82BD`, neutral, success, warning, dan info. |
| Typography | System font stack, ukuran 12, 14, 16, 18, 20, 24, dan judul fluid. |
| Spacing | Skala kelipatan 4 px: 4, 8, 12, 16, 20, 24, 32, 40, 48, dan 64 px. |
| Buttons | Primary, secondary, outline, dan disabled. Tinggi minimum 44 px dengan hover/focus state. |
| Form controls | Label, input, select, dan textarea memakai border, radius, dan focus state konsisten. |
| Cards | Surface putih, border netral, radius 14 px, padding seragam, dan shadow ringan. |

Semua token visual didefinisikan sebagai CSS custom properties pada `:root` di `css/style.css`.

## Hasil Screenshot

### Dashboard

- `images/before-desktop.png` dan `images/before-mobile.png` menampilkan source `Contoh2` sebelum pengembangan, dengan identitas Arsanti.
- `images/after-desktop.png` dan `images/after-mobile.png` adalah hasil redesign untuk Arsanti.

### Design System

- `DesignSystem/design-system-desktop.png`
- `DesignSystem/design-system-mobile.png`

## Analisis Perubahan

1. **Palet warna belum memiliki aturan bersama.** Solusi: menetapkan token warna pada `:root` dan menggunakannya secara konsisten.
2. **Hierarki konten kurang terarah.** Solusi: memisahkan hero, statistik, jadwal, pengumuman, dan tabel dengan ukuran heading serta jarak yang berbeda.
3. **Komponen visual perlu konsisten.** Solusi: menggunakan class reusable seperti `.panel`, `.button`, `.badge`, `.stat-card`, dan `.status-pill`.
4. **Tampilan desktop tidak ideal bila dipersempit.** Solusi: mengubah sidebar menjadi navigasi horizontal, mengubah grid menjadi satu kolom, dan mempertahankan tabel dalam area scroll horizontal.
5. **Elemen form tidak terlihat pada dashboard.** Solusi: menampilkan kontrol form pada halaman dokumentasi Design System, sesuai cakupan komponen yang diminta.

## Cara Menjalankan

1. Ekstrak folder proyek.
2. Buka `pertemuan6/Tugas/index.html` pada browser.
3. Pilih tautan **Lihat Design System** untuk membuka dokumentasi komponen.
4. Gunakan Developer Tools dan device emulation untuk memeriksa breakpoint mobile.

## Catatan

Angka IPK, SKS, jadwal, dan progres pada dashboard merupakan data contoh untuk kebutuhan mockup, bukan data akademik resmi. Implementasi hanya menggunakan HTML dan CSS tanpa framework maupun JavaScript.
