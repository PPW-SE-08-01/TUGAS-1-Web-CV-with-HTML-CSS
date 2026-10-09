# TUGAS PENDAHULUAN / TUGAS UNGUIDED
# PEMROGRAMAN PERANGKAT BERGERAK

<br>

<div align="center">

# MODUL 01
## HTML CV WITH CSS

<br>

<img src="https://bit-jkt.telkomuniversity.ac.id/wp-content/uploads/2023/02/cropped-logo_telkom_university.png" alt="Telkom University Logo">

**Disusun Oleh :**

**Davis Arvaputra Dwiansyah**  
**NIM: 103122400034**  
**Kelas: SE-08-01**

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

### a. `index.html`

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CV - Davis Arvaputra Dwiansyah</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>

    <!-- HEADER / PROFIL SINGKAT -->
    <header>
        <img src="images/images.jpg"
             alt="Gambar saya"
             width="100"
             height="100"
             class="gambar-saya">

        <h1 class="nama-saya">Davis Arvaputra Dwiansyah</h1>
        <p>Cyber Security Analyst | Full Stack Developer</p>
        <p>Nomor Telepon: 085117703324</p>
        <p>Email: davizganteng@protonmail.com</p>
    </header>

    <!-- RINGKASAN PROFESIONAL -->
    <section>
        <section>
            <h2>Ringkasan Profesional</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </section>

        <!-- PENGALAMAN KERJA -->
        <section>
            <h2>Pengalaman Kerja</h2>

            <article>
                <h3>Cyber Security Analyst</h3>
                <p>SMT Program Indonesia - KISIA - Korea Information Security Industry Association</p>
                <p>June 2025 - September 2025</p>
                <ul>
                    <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                </ul>
            </article>

            <article>
                <h3>Project Manager</h3>
                <p>Codingcamp 2026 Powered by DBS Foundation</p>
                <p>February 2026 - August 2026</p>
                <ul>
                    <li>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                        Nunc viverra in elit id pulvinar. Curabitur sit amet ante
                        aliquet dolor congue faucibus ut sit amet urna.
                    </li>
                    <li>
                        Nulla facilisi. Sed vitae justo tincidunt, convallis diam sed,
                        porttitor elit. Aliquam ornare volutpat leo, eget sollicitudin urna.
                    </li>
                </ul>
            </article>
        </section>

        <!-- PENDIDIKAN -->
        <section>
            <h2>Pendidikan</h2>

            <article>
                <h3>Telkom University Purwokerto</h3>
                <p>Sept 2024 - Sept 2028</p>
                <p>IPK: 3.8</p>
            </article>
        </section>

        <!-- KEAHLIAN -->
        <section>
            <h2>Keahlian Teknis</h2>
            <ul>
                <li>Frontend: HTML5, CSS3, JavaScript, React, Vue.js</li>
                <li>Backend: Node.js, Express.js, Python, Django</li>
                <li>Database: MySQL, MongoDB, PostgreSQL</li>
                <li>Tools: Git, Docker, GitHub, VS Code</li>
                <li>Soft Skills: Problem Solving, Team Work, Communication</li>
            </ul>
        </section>

        <!-- SERTIFIKASI -->
        <section>
            <h2>Sertifikasi</h2>
            <ul>
                <li>Google Associate Cloud Engineer - 2024</li>
                <li>AWS Certified Solutions Architect - 2024</li>
                <li>JavaScript Advanced Course - Dicoding 2026</li>
            </ul>
        </section>

        <!-- BAHASA -->
        <section>
            <h2>Bahasa</h2>
            <ul>
                <li>Bahasa Indonesia - Native</li>
                <li>Bahasa Inggris - Profesional</li>
            </ul>
        </section>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>Portfolio: davisarvaputra.id | GitHub: github.com/davizofficial</p>
    </footer>

</body>
</html>
```

### b. `styles.css`

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    background-color: #f5f5f5;
}

body {
    width: calc(100% - 40px);
    max-width: 850px;
    margin: 32px auto;
    font-family: 'Segoe UI', Arial, sans-serif;
    font-size: 15px;
    line-height: 1.7;
    color: #333;
    overflow-wrap: anywhere;
}

header {
    display: grid;
    grid-template-columns: 110px minmax(0, 1fr);
    column-gap: 28px;
    align-items: start;
    padding: 32px;
    margin-bottom: 24px;
    background-color: #fff;
    border: 1px solid #e2e2e2;
    border-radius: 4px;
}

header img {
    grid-column: 1;
    grid-row: 1 / span 5;
    width: 110px;
    height: 110px;
    max-width: 100%;
    object-fit: cover;
    border-radius: 4px;
}

header h1,
header p {
    grid-column: 2;
    min-width: 0;
}

header h1 {
    font-size: 28px;
    font-weight: 600;
    line-height: 1.3;
    margin-bottom: 8px;
    color: #222;
}

header p {
    font-size: 14px;
    color: #555;
    margin-bottom: 4px;
}

header p:first-of-type {
    font-size: 15px;
    color: #333;
    margin-bottom: 12px;
}

body > section {
    padding: 32px;
    background-color: #fff;
    border: 1px solid #e2e2e2;
    border-radius: 4px;
}

section > section + section {
    margin-top: 28px;
}

h2 {
    font-size: 19px;
    font-weight: 600;
    line-height: 1.4;
    color: #222;
    padding-bottom: 10px;
    margin-bottom: 16px;
    border-bottom: 1px solid #e2e2e2;
}

article + article {
    margin-top: 22px;
    padding-top: 20px;
    border-top: 1px solid #eee;
}

h3 {
    font-size: 16px;
    font-weight: 600;
    line-height: 1.5;
    color: #222;
    margin-bottom: 4px;
}

article p {
    font-size: 14px;
    color: #555;
    margin-bottom: 4px;
}

ul {
    padding-left: 20px;
    margin-top: 10px;
}

li {
    padding-left: 3px;
    margin-bottom: 8px;
}

li:last-child {
    margin-bottom: 0;
}

footer {
    padding: 20px 12px 0;
    text-align: center;
    font-size: 13px;
    color: #555;
}

@media (max-width: 768px) {
    body {
        width: calc(100% - 32px);
        margin: 24px auto;
    }

    header,
    body > section {
        padding: 24px;
    }

    header {
        grid-template-columns: 90px minmax(0, 1fr);
        column-gap: 20px;
    }

    header img {
        width: 90px;
        height: 90px;
    }

    header h1 {
        font-size: 24px;
    }
}

@media (max-width: 480px) {
    body {
        width: calc(100% - 24px);
        margin: 16px auto;
    }

    header,
    body > section {
        padding: 20px;
    }

    header {
        grid-template-columns: minmax(0, 1fr);
        margin-bottom: 16px;
    }

    header img {
        grid-column: 1;
        grid-row: auto;
        width: 80px;
        height: 80px;
        margin-bottom: 16px;
    }

    header h1,
    header p {
        grid-column: 1;
    }

    header h1 {
        font-size: 22px;
    }

    h2 {
        font-size: 18px;
    }

    section > section + section {
        margin-top: 24px;
    }
}
```

## 2. Screenshot Output

> **Lampirkan screenshot hasil/output program di bagian ini.**

Contoh struktur file:

```text
screenshots/
└── output-cv.png
```

Kemudian tampilkan screenshot pada README:

```markdown
![Screenshot Output CV](screenshots/output-cv.png)
```

## 3. Deskripsi Program

Program yang dibuat merupakan halaman Curriculum Vitae (CV) menggunakan HTML dan CSS. HTML digunakan untuk membangun struktur halaman yang terdiri dari informasi profil, pengalaman kerja, pendidikan, keahlian teknis, sertifikasi, bahasa, dan informasi portfolio. CSS digunakan untuk mengatur tata letak, ukuran teks, warna, jarak, border, serta tampilan halaman agar lebih terstruktur dan mudah dibaca. Pada bagian header digunakan CSS Grid untuk menempatkan foto profil dan informasi identitas secara berdampingan. Program juga menggunakan media query agar tampilan CV dapat menyesuaikan ukuran layar pada perangkat tablet maupun smartphone. Hasil akhirnya adalah halaman CV yang memiliki struktur informasi yang rapi dan dapat ditampilkan melalui web browser.

---

## Struktur Folder Project

```text
TUGAS-1-Web-CV-with-HTML-CSS/
└── Davis-Arvaputra-Dwiansyah-103122400016/
    ├── README.md
    ├── index.html
    ├── styles.css
    └── screenshots/
        └── output-cv.png
```
