# Latihan 4 - Landing Page Arunika Studio

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

Proyek ini adalah **Latihan 4 Desain Web A** berupa *landing page* untuk studio fiktif bernama **Arunika Studio**, yang menawarkan jasa desain dan pengembangan web. Halaman dibuat dengan **HTML5** dan **CSS3** (berkas CSS terpisah) dengan tampilan potret tegak yang responsif.

## Fitur / Isi Halaman

| Bagian         | Keterangan                                                                                   |
| -------------- | -------------------------------------------------------------------------------------------- |
| **Header**     | Logo teks dan menu navigasi (Beranda, Layanan, Kontak) dengan *smooth scroll*                |
| **Hero**       | Logo bulat, judul sambutan, deskripsi singkat, dan tombol "Lihat Layanan Kami"               |
| **Layanan**    | Tiga kartu: *Web Design (UI/UX)*, *Web Development*, dan *Branding & Identitas Visual*       |
| **Kontak**     | Informasi kontak (email, telepon/WhatsApp, lokasi) dan formulir pesan                        |
| **Footer**     | Hak cipta &copy; 2026 Arunika Studio                                                         |

## Konsep CSS yang Diterapkan

- **Box model**: `box-sizing: border-box` pada reset CSS, serta `padding`, `margin`, dan `border`
- **Class reusable**:
  - `.card-box` : kartu putih dengan sudut membulat dan bayangan
  - `.btn-primary` : tombol biru dengan efek *hover*
  - `.section-title` : judul section di tengah
- **Flexbox**: tata letak header (logo dan navigasi)
- **CSS Grid**: kartu layanan, galeri 3 gambar (`repeat(3, 1fr)`), dan area kontak
- **Gambar bulat**: `border-radius: 50%` dan `object-fit: cover` pada logo profil
- **Smooth scroll**: `scroll-behavior: smooth`
- **Media query**: `@media (max-width: 767px)` untuk penyesuaian tampilan mobile

## Struktur Berkas

```
Latihan4/
├── Latihan4.html   # Halaman utama landing page
├── style.css       # Stylesheet
├── logo.jpg        # Logo Arunika Studio
├── gambar1.jpg     # Gambar kartu Web Design
├── gambar2.jpg
├── gambar3.jpg
├── foto1.jpg       # Gambar kartu Web Development
├── foto2.jpg
├── foto3.jpg
└── README.md       # Dokumentasi proyek
```

> **Catatan:** Semua berkas gambar di atas harus berada satu folder dengan `Latihan4.html` agar tampil dengan benar.

## Cara Menjalankan

1. Clone atau unduh repositori ini.
2. Pastikan `Latihan4.html`, `style.css`, dan semua gambar berada dalam satu folder.
3. Buka `Latihan4.html` di browser (klik dua kali, atau gunakan ekstensi *Live Server* di VS Code).

## Teknologi

- HTML5
- CSS3
- Visual Studio Code

---

&copy; 2026 **Arsanti Nur Indriani** (4525210128) — Fakultas Teknik, Universitas Pancasila.