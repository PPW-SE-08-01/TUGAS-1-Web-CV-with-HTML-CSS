<!-- NIM: 103122400026 | Nama: Geusan Edurais Aria Daffa -->

# CV Web — Geusan Edurais Aria Daffa

> Tugas Praktikum Perancangan dan Pemrograman Web — Pertemuan 1

Halaman CV pribadi yang dibuat pakai HTML5 dan CSS3 doang, tanpa framework apapun. Bisa langsung dibuka di browser atau dicetak.

---

## Tentang Proyek

Dibuat buat tugas praktikum supaya lebih paham cara kerja HTML dan CSS dari dasarnya. Isi CV-nya sendiri berdasarkan profil nyata sebagai Frontend Engineer.

---

## Cara Pakai

1. Download atau clone folder ini
2. Buka `index.html` di browser
3. *(Opsional)* Pakai ekstensi **Live Server** di VS Code biar auto-reload waktu ngedit

---

## Isi Halaman

| # | Bagian | Isi |
|---|--------|-----|
| 1 | **Header** | Nama, jabatan, kontak, link profil |
| 2 | **Professional Summary** | Ringkasan singkat profil |
| 3 | **Skills** | Daftar skill teknis |
| 4 | **Experience** | Pengalaman kerja & magang |
| 5 | **Projects** | Proyek yang pernah dikerjain |
| 6 | **Education** | Pendidikan |
| 7 | **Certifications** | Sertifikasi |
| 8 | **Contact Me** | Form input |

---

## Teknis

### HTML

Elemen yang dipakai dipilih sesuai fungsinya:

- `<header>` — bagian atas berisi nama dan kontak
- `<section>` — tiap bagian CV punya section sendiri
- `<dl>` / `<dt>` / `<dd>` — daftar skill pakai definition list
- `<ul>` — poin-poin pencapaian di bagian pengalaman
- `<form>`, `<fieldset>`, `<legend>` — form di bagian bawah

### CSS

Semua ditulis manual di `style.css`, tanpa framework:

- **CSS Custom Properties** — warna dan ukuran disimpan di `:root` biar gampang diubah
- **Flexbox** — untuk susunan header dan tiap item (judul kiri, tanggal kanan)
- **CSS Grid** — untuk form dua kolom dan daftar skill
- **`@media (max-width: 640px)`** — supaya rapi di layar kecil
- **`@media print`** — tampilan khusus waktu dicetak, form disembunyikan

### Warna

```
Background  : #f1f2f4
Surface     : #ffffff
Teks utama  : #1f2330
Teks muted  : #5c6377
Aksen       : #2f4b8f  (navy)
```

---

## Struktur File

```
pertemuan1/
├── index.html       ← konten dan struktur CV
├── style.css        ← styling
└── assets/
    └── img/         ← folder gambar
```