# LAPORAN PRAKTIKUM
# PEMROGRAMAN PERANGKAT BERGERAK

<br>

<div align="center">

# MODUL 02 & 03
## HTML CV WITH CSS

<br>

**Disusun Oleh :**

**Chiara Calina Devi**  
**NIM: 103122400016**  
**Kelas: SE08-01**

<br>

**Asisten Praktikum :**  
Abu Abdirrahman Humaid Al-Atsary  
Hamka Zainul Ardhi
<br>

**Dosen Pengampu :**  
Arif Amrullah, S.Kom., M.Kom.

<br>

**PROGRAM STUDI S1 SOFTWARE ENGINEERING**  
**FAKULTAS INFORMATIKA**  
**TELKOM UNIVERSITY PURWOKERTO**  
**2026**

</div>

---

# A. SOAL

Membuat halaman Curriculum Vitae (CV) menggunakan HTML yang telah diberikan dan menerapkan CSS untuk mengatur tampilan halaman agar lebih rapi, terstruktur, dan responsif.

# B. JAWABAN

## 1. Source Code

### a. `cv.html`

```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>CV - Chiara Calina Devi</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="cv">

    <header>
      <img src="foto.jpg" alt="Foto Chiara Calina Devi">
      <div class="kontak">
        <h1>CHIARA CALINA DEVI</h1>
        <p><b>Address:</b> Puri Wiradadi 3 Blok B No. 4, Dusun Jl. RW Salak No. 3, RT.08/RW.04, Kec. Sokaraja, Kab. Banyumas, Jawa Tengah 53181</p>
        <p><b>Phone:</b> 0878-6126-6468</p>
        <p><b>Email:</b> chiaracalinaa@gmail.com</p>
      </div>
    </header>

    <section>
      <h2>SUMMARY</h2>
      <p>Adaptable, detail-oriented, and highly organized professional with 3+ years of experience spanning administration, cash handling, operational support, and customer service across F&amp;B, retail, and service environments. Proven track record in managing daily operations, financial record-keeping, client communication, and schedule coordination with accuracy and efficiency. Combines technical problem-solving capabilities as a Software Engineering undergraduate with strong interpersonal and multitasking skills. Reliable, quick to learn, and ready to deliver immediate value in administrative, personal assistance, operational, or customer-facing roles.</p>
    </section>

    <section>
      <h2>WORK EXPERIENCE</h2>

      <div class="baris"><span>Nirmala Fashion - Admin</span><span>Juni 2021 - Juli 2023</span></div>
      <ul>
        <li>Recorded and monitored daily cash inflows and outflows to ensure accurate financial tracking.</li>
        <li>Performed input of incoming goods and maintained up-to-date stock records.</li>
        <li>Carried out bookkeeping tasks to support smooth and organized store operations.</li>
        <li>Maintained accurate documentation to assist inventory control and reporting.</li>
      </ul>

      <div class="baris"><span>Es teh Desa Jatinegara - Admin &amp; Barista</span><span>Juli 2023 - Oct 2024</span></div>
      <ul>
        <li>Prepared and made customer orders while ensuring consistent product quality.</li>
        <li>Recorded daily cash transactions and maintained accurate store bookkeeping.</li>
        <li>Maintained store cleanliness and organization to support a comfortable customer experience.</li>
        <li>Handled customer interactions and inquiries, ensuring excellent service standards.</li>
      </ul>

      <div class="baris"><span>Gombong Huis - Waiters</span><span>Juni 2025 - Sept 2025</span></div>
      <ul>
        <li>Served and presented menu items to customers with attentive, friendly service.</li>
        <li>Performed café closing procedures, including final checks and end-of-day tasks.</li>
        <li>Maintained cleanliness and tidiness of the café to uphold service standards.</li>
      </ul>

      <div class="baris"><span>Business Owner Glowny Collection - Personal Asisstant</span><span>Juni 2026 - Agustus 2026</span></div>
      <ul>
        <li>Managed daily schedule, personal agenda, deadlines, and important reminders for the business owner.</li>
        <li>Accompanied the business owner on work needs, both in and out of town.</li>
        <li>Arranged travel logistics and reservations for hotels, flights, transport, and restaurants.</li>
        <li>Conducted basic research on products, services, and vendors.</li>
        <li>Handled personal errands and purchasing on the business owner's behalf.</li>
        <li>Supported various PA tasks as directed, including correspondence, task prioritization, and pet care.</li>
        <li>Applied strong adaptability, multitasking, and communication skills in a fast-paced setting.</li>
      </ul>
    </section>

    <section>
      <h2>EDUCATION</h2>
      <div class="baris"><span>Bachelor of Software Engineering</span><span>Sept 2024 - May 2028 (Expected)</span></div>
      <p><i>Telkom University Purwokerto</i></p>
      <ul>
        <li>Current GPA: 3.71 out of 4.00</li>
      </ul>
    </section>

    <section>
      <h2>ADDITIONAL INFORMATION</h2>
      <p><b>Soft Skills</b>: Problem Solving, Time Management, Detail Oriented, Multitasking, Teamwork in Collaboration, Innovative and Adaptive, Verbal &amp; Non-Verbal Communication.</p>
      <p><b>Hard Skills</b>: Microsoft Office (Excel, Word, PowerPoint), Google Workspace (Sheets, Docs, Calendar, Drive), bookkeeping, Data entry &amp; filing system, Travel &amp; schedule arrangement, Invoice tracking</p>
      <p><b>Languages</b>: Bahasa Indonesia (Fasih), English (Fluent).</p>
      <p><b>Certifications</b>: English Course Certificate - Mr Bob (26 January - 20 February 2026).</p>
    </section>

  </div>
</body>
</html>
```

### b. `style.css`

```css
body {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 14px;
  line-height: 1.5;
  color: #222;
  background: #f2f2f2;
  margin: 0;
}

.cv {
  max-width: 800px;
  margin: 20px auto;
  padding: 30px 40px;
  background: #fff;
}

header {
  display: flex;
  gap: 24px;
  margin-bottom: 20px;
}

header img {
  width: 120px;
  height: 120px;
  object-fit: cover;
  object-position: center top;
  border-radius: 61%;
}

h1 {
  margin: 0 0 8px;
  font-size: 26px;
  color: #1f3a5f;
}

.kontak p {
  margin: 2px 0;
}

h2 {
  font-size: 16px;
  color: #1f3a5f;
  border-bottom: 1px solid #1f3a5f;
  padding-bottom: 3px;
  margin: 22px 0 10px;
}

.baris {
  display: flex;
  justify-content: space-between;
  gap: 10px;
  font-weight: bold;
  margin-top: 12px;
}

.baris span:last-child {
  white-space: nowrap;
}

ul {
  margin: 4px 0 0;
  padding-left: 20px;
}

p {
  margin: 4px 0;
}

@media (max-width: 600px) {
  .cv { padding: 20px; margin: 0; }
  header { flex-direction: column; }
  .baris { flex-direction: column; gap: 0; }
}

@media print {
  body { background: #fff; }
  .cv { margin: 0; padding: 0; max-width: none; }
}
```

## 2. Screenshot Output

![Screenshot Output CV](output.png)

## 3. Deskripsi Program

Program yang dibuat merupakan halaman Curriculum Vitae (CV) menggunakan HTML dan CSS. HTML digunakan untuk membangun struktur halaman yang terdiri dari header berisi foto dan informasi kontak, ringkasan profesional (summary), pengalaman kerja, pendidikan, serta informasi tambahan berupa soft skills, hard skills, bahasa, dan sertifikasi. Elemen seperti `header`, `section`, `h1`, `h2`, `ul`, dan `li` digunakan agar struktur dokumen semantik dan mudah dibaca.

CSS digunakan untuk mengatur tampilan halaman. Seluruh isi CV dibungkus dalam class `cv` dengan lebar maksimal 800px, diposisikan di tengah, dan diberi latar putih di atas background abu-abu muda. Pada bagian header digunakan Flexbox agar foto profil dan informasi kontak tampil berdampingan, dengan foto dibuat berbentuk lingkaran menggunakan `border-radius` dan `object-fit: cover`. Judul setiap bagian (`h2`) diberi warna biru tua dan garis bawah sebagai pemisah antarbagian. Pada bagian pengalaman kerja dan pendidikan, nama posisi dan periode waktu ditampilkan sejajar dalam satu baris menggunakan class `baris` dengan Flexbox dan `justify-content: space-between`.

Program juga menggunakan media query `max-width: 600px` agar tampilan menyesuaikan layar smartphone, yaitu foto dan kontak tersusun vertikal serta padding dikurangi. Selain itu, media query `print` ditambahkan agar CV tampil bersih tanpa background dan margin ketika dicetak. Hasil akhirnya adalah halaman CV yang terstruktur, konsisten, dan dapat ditampilkan dengan baik melalui web browser.

---

## Struktur Folder Project

```text
TUGAS-1-Web-CV-with-HTML-CSS/
└── 103122400016_chiara calina devi/
    ├── README.md
    ├── cv.html
    ├── style.css
    ├── foto.jpg
    └── screenshots/
        └── output.png
```