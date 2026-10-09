<!-- Watermark: NIM: 103122400027 | Nama: Ryvanda -->

# Curriculum Vitae — Ryvanda (103122400027)

Website CV pribadi sederhana buat tugas Praktikum Web. Fokusnya lebih ke penampilan struktur halaman yang rapi, semantik, dan responsif banget, bukan malah dibuat keruntuhan sama fancy animasi.

## Poin Utama

- Pake **HTML5 semantik**, jadi strukturnya jalanin `<header>`, `<nav>`, `<main>`, `<aside>`, `<article>`, `<section>`, `<footer>` secara benar;
- CSS-nya **native eksternal**, tidak pakai framework, tidak ada inline style yang disebar-disebar di HTML (semoga);
- Layout utamanya pakai **CSS Grid**, termasuk bagian proyek yang pake `auto-fit / minmax()` biar card-nya otomatis turun naik sesuai lebar layar;
- Sidebar navigasi tetap kelihatan di atas-samping, tapi kalau buka di HP bakal jadi satu kolom utuh;
- Setting warna dipisah di variable CSS (`:root`), jadi kalau mau ganti tema biru ke coklat atau ngubah nuansa, tinggal ubah di satu tempat.

## Struktur File

```
.
├── index.html   # satu-satunya halaman utama
└── style.css    # stylesheet eksternal yang dipakai index.html
```

Yang ada cuma dua file, jadi kalau ada yang mau ditambahin halaman atau component, pelajari dulu di sini sebelum malah bikin banyak file.

## Cara Pakai

Buka file `index.html` langsung lewat browser, atau kalau mau lihat perubahan CSS sambil mengedit, jalankan server lokal.

### Contoh jalanin lokal pakai Python (kalau tersedia):

```bash
python3 -m http.server 8000
```

Lalu buka `http://localhost:8000`.

Kalau mau pakai server lain, terserah. Yang penting HTML dan CSS-nya bisa dibaca browser, dan relative path-nya tetep benar.

## Struktur Halaman

- Header utama di paling atas;
- Sidebar kiri buat identitas singkat dan menu navigasi;
- Konten utama di tengah kanan isi:
  - Profil & kontak;
  - Tentang saya;
  - Pendidikan;
  - Keahlian (hard skill & soft skill);
  - Proyek / portofolio;
  - Pengalaman organisasi;
- Footer di paling bawah.

Konten ditulis dalam Bahasa Indonesia, sesuai konteks mahasiswa Software Engineering yang lagi latihan bikin halaman web sendiri.

## Desain

### Warna

Warna dasarnya biru, diatur pakai CSS custom properties di `:root`. Kalau mau ganti tema, tinggal edit variabel-variabel itu, jangan malah nyari warna satu-satu di selector.

### Layout

- Pengaturan utama pake **CSS Grid** dengan dua kolom: sidebar + konten utama;
- Bagian proyek pakai `grid-template-columns: repeat(auto-fit, minmax(...))`, jadi card proyek bisa mengikuti ruang available tanpa perlu banyak media query tersendiri;
- Untuk layar kecil, grid dibalik jadi satu kolom lebar.

### Typography & readability

- Font umum pakai sans-serif standar;
- Spacing, border, dan radius disesuaikan biar konten tidak tampak kasar, tapi jangan terlalu berlebihan.

## 🛠 Teknologi

| Kategori | Yang dipakai |
|----------|--------------|
| Markup | HTML5 |
| Style | CSS3 native (eksternal) |
| Layout | CSS Grid + media query |
| OS / environment | Local browser / http server |

Tidak pakai framework CSS, tidak pakai build tool, tidak pakai JavaScript. Gapapa kalau nanti perlu JS buat halaman lain, tapi untuk skope CV ini tetep disederhanakan.

## Validasi Pokok (yang biasanya dilihat di praktikum)

- Semua elemen konten dibungkus elemen semantik yang tepat;
- Tautan kontak pakai `mailto:` dan `https://wa.me/...` sesuai bentuk yang baku;
- Sidebar dan footer tidak hilang saat resize;
- Elemen yang sifatnya hanya untuk screen reader jika ada bisa diberi class `.sr-only`.

## Pengembangan Selanjutnya

Kalau tugas atau urusan berikutnya butuh:

- Halaman tambahan;
- Dark mode;
- Preferensi warna yang lebih dinamis;
- Animasi interaksi yang lebih halus;

Bisa dikerjakan bertahap, jangan langsung meledak-ledak. Biar tetap enak dibaca dan dibongkar pas ada revisi.

## Penjelasan Singkat Per Elemen

- `<header>`: Judul halaman dan subjudul praktikum.
- `<nav>`: Menu navigasi samping, disimpan di sidebar.
- `<main>`: Konten inti CV.
- `<section>`: Pengelompokan per topik (tentang, pendidikan, keahlian, proyek, organisasi).
- `<article>`: Unit konten di dalam section, misalnya tiap pengalaman atau tiap proyek.
- `<footer>`: Copyright ringan di bawah.
- `.kartu-profil`: Identitas singkat di sidebar.
- `.sr-only`: Elemen yang hanya dibaca oleh screen reader.

Kombinasi elemen ini bikin struktur lebih enak dibaca oleh manusia dan lebih enak juga dibaca oleh browser / screen reader.

## Referensi

Implementasi ini mengacu pada pola umum dokumentasi web MDN, terutama:

- Struktur dokumen dengan elemen semantik, contohnya penggunaan `<header>`, `<nav>`, `<main>`, `<article>`, `<aside>`, `<footer>`
  - Sumber Context7: `/mdn/content` — contoh penataan konten semantik dan landmark page
- Layout grid responsif dengan `repeat(auto-fit, minmax(...))`
  - Sumber Context7: `/mdn/content` — pola grid auto-fill / auto-fit dan relasi `minmax()` dengan track yang fleksibel

Gunakan referensi tersebut kalau nanti perlu mengecek ulang cara pakai elemen semantik atau cara kerja CSS Grid yang lebih detail.
 
