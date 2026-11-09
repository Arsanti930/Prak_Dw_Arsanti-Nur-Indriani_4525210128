# Tugas Praktikum Desain Web — Pertemuan 7

## Biodata Mahasiswa

| Keterangan | Identitas |
|---|---|
| Nama | Arsanti Nur Indriani |
| NIM | 4525210128 |
| Program Studi | Teknik Informatika |
| Mata Kuliah | Praktikum Desain Web A |
| Pertemuan | 7 — HTML Form dan Validasi Input |

## Deskripsi

Membangun Form Registrasi Mahasiswa Baru menggunakan HTML5 dan CSS3 murni. Form mengumpulkan nama, NIM, email, jenis kelamin, program studi, hobi, dan foto. Tata letak dibuat responsif untuk desktop serta mobile.

## Elemen HTML yang Digunakan

| Elemen / Atribut | Fungsi |
|---|---|
| `form` | Membungkus elemen formulir. |
| `action` | Menentukan endpoint tujuan pengiriman. |
| `method="post"` | Mengirim data melalui body HTTP request. |
| `enctype="multipart/form-data"` | Diperlukan untuk mengirim file foto. |
| `input type="text"` | Memasukkan nama dan NIM. |
| `input type="email"` | Validasi dasar format email oleh browser. |
| `input type="radio"` | Memilih satu jenis kelamin. |
| `input type="checkbox"` | Memilih beberapa hobi dan persetujuan. |
| `select` dan `option` | Memilih program studi. |
| `input type="file"` dan `accept` | Memilih file foto JPG/JPEG/PNG. |
| `required`, `pattern`, `minlength` | Validasi dasar di sisi browser. |
| `fieldset` dan `legend` | Mengelompokkan pilihan yang berkaitan. |

## Perbedaan GET dan POST

- **GET** dipakai pada contoh pencarian data mahasiswa. Parameter form ditambahkan ke URL sehingga cocok untuk pencarian atau filter yang tidak mengubah data.
- **POST** dipakai pada tugas registrasi. Data dikirim melalui body request dan tidak ditambahkan sebagai query string pada URL.
- Form registrasi memakai `POST` karena mengirim data pendaftaran dan file foto. Atribut `enctype="multipart/form-data"` diperlukan untuk pengiriman file.

## Struktur Folder

```text
Pertemuan7/
├── Contoh 1/                                  # Contoh form dasar
├── Contoh 2/                                  # Contoh form lanjutan
├── Form-Pencarian-Data-Mahasiswa-Method-GET/  # Demonstrasi method GET
├── Form-Pendaftaran-Mahasiswa-Method-POST/    # Demonstrasi method POST
├── quiz/                                      # Latihan/kuis dari materi
└── Tugas/
    ├── css/
    │   └── style.css
    ├── images/
    │   ├── desktop-version.png
    │   └── mobile-version.png
    ├── dokumentasi/
    │   └── README.md
    └── mahasiswa.html
```

## Validasi yang Diterapkan

1. Nama wajib diisi dan memiliki minimal 3 karakter.
2. NIM wajib diisi, berupa angka, dan memiliki panjang 8–10 digit melalui `pattern="[0-9]{8,10}"`.
3. Email wajib diisi dan menggunakan `type="email"`.
4. Salah satu opsi jenis kelamin harus dipilih.
5. Program studi wajib dipilih dari dropdown.
6. Foto wajib dipilih dan dibatasi pada JPG, JPEG, atau PNG melalui atribut `accept`.
7. Persetujuan wajib dicentang sebelum formulir dikirim.

Validasi ini merupakan validasi sisi browser. Atribut `accept` membatasi pilihan file pada dialog pemilih file, tetapi bukan pemeriksaan keamanan file di server.

## Cara Menjalankan

1. Ekstrak folder proyek.
2. Buka `Pertemuan7/Tugas/mahasiswa.html` melalui browser.
3. Isi form dan coba kirim ketika masih ada kolom wajib yang kosong.
4. Uji NIM dengan kurang dari 8 digit, lebih dari 10 digit, atau karakter non-angka untuk melihat validasi HTML.
5. Pilih file dengan format yang diterima.

## Catatan Pengiriman

Form menggunakan `action="/submit-registration"` sebagai placeholder endpoint. Source ini adalah tugas frontend HTML/CSS, sehingga data belum disimpan ke database. Agar pengiriman POST benar-benar diproses, diperlukan backend/server yang menyediakan endpoint `/submit-registration`. Saat dibuka langsung dengan `file://`, browser tetap dapat menampilkan form dan menjalankan validasi HTML, tetapi tidak ada server yang menerima data.

## Teknologi dan Batasan

- HTML5
- CSS3 eksternal
- CSS Grid, Flexbox, media query, dan pseudo-class
- Tidak menggunakan JavaScript, framework, maupun backend
