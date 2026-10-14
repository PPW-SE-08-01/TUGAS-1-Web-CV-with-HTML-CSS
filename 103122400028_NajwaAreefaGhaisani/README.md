<!-- NIM: [NIM KAMU] | Nama: Najwa Areefa Ghaisani -->

# CV Web — Najwa Areefa Ghaisani

> Tugas Praktikum Perancangan dan Pemrograman Web — Pertemuan 1

Halaman CV pribadi yang dibuat menggunakan HTML5 dan CSS3 tanpa framework. CV ini menampilkan profil singkat, pengalaman kerja lapangan, pendidikan, pengalaman organisasi, serta keterampilan yang dimiliki. Halaman dapat langsung dibuka melalui browser atau dicetak.

---

## Tentang Proyek

Proyek ini dibuat untuk memenuhi tugas praktikum Perancangan dan Pemrograman Web sekaligus mempelajari dasar-dasar HTML dan CSS dalam membangun halaman web.

CV berisi informasi profil pribadi sebagai mahasiswa S1 Rekayasa Perangkat Lunak di Telkom University Purwokerto, termasuk pengalaman kerja lapangan, pendidikan, pengalaman organisasi dan kepanitiaan, serta keterampilan dan pencapaian.

---

## Cara Pakai

1. Download atau clone repository ini.
2. Buka folder proyek `resume-najwa`.
3. Buka file `index.html` menggunakan browser.
4. *(Opsional)* Gunakan ekstensi **Live Server** di VS Code agar perubahan kode dapat langsung terlihat saat mengedit.

---

## Isi Halaman

| # | Bagian | Isi |
|---|--------|-----|
| 1 | **Header** | Nama, nomor telepon, email, tautan LinkedIn, dan lokasi |
| 2 | **Professional Summary** | Ringkasan profil dan minat di bidang pengembangan website |
| 3 | **Pengalaman Kerja Lapangan** | Pengalaman sebagai Staff Lab dan Student Internship |
| 4 | **Pendidikan** | Riwayat pendidikan SMK dan perguruan tinggi |
| 5 | **Pengalaman Organisasi & Kepanitiaan** | Pengalaman dalam organisasi dan kepanitiaan |
| 6 | **Skills, Achievements & Other Experience** | Keterampilan, pencapaian, dan pengalaman lainnya |

---

## Teknis

### HTML

Elemen HTML digunakan untuk menyusun konten CV sesuai fungsinya:

- `<header>` — bagian atas yang berisi nama dan informasi kontak.
- `<h1>` dan `<h2>` — judul utama dan judul setiap bagian CV.
- `<p>` — menampilkan ringkasan profil dan informasi kontak.
- `<div>` — mengelompokkan konten, seperti pengalaman, jabatan, dan tanggal.
- `<span>` — menampilkan informasi tambahan dalam satu baris teks.
- `<ul>` dan `<li>` — menampilkan daftar tugas dan pencapaian.
- `<a>` — membuat tautan email dan profil LinkedIn.

### CSS

Semua styling ditulis secara manual di file `style.css`, tanpa menggunakan framework CSS:

- **CSS Reset** — mengatur margin, padding, dan `box-sizing` agar tampilan lebih konsisten.
- **Flexbox** — mengatur posisi informasi header serta judul dan tanggal pengalaman.
- **Typography** — mengatur jenis font, ukuran teks, ketebalan, dan jarak antarbaris.
- **Spacing** — mengatur margin dan padding agar setiap bagian CV terlihat rapi.
- **`@media (max-width: 600px)`** — menyesuaikan tata letak agar lebih nyaman dilihat pada layar kecil.
- **`@media print`** — mengatur tampilan saat CV dicetak dengan menghilangkan latar belakang abu-abu dan bayangan halaman.

### Warna

```css
Background  : #eeeeee
Surface     : #ffffff
Teks utama  : #111111
Teks muted  : #888888
```

---

## Struktur File

```text
resume-najwa/
├── index.html    ← konten dan struktur CV
├── style.css     ← styling halaman CV
└── img/          ← folder untuk aset gambar
```

---