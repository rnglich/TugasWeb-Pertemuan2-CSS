# 🎨 Tugas Rutin 2 — CSS Layouting Portofolio


Repositori ini memuat implementasi **Tugas Rutin 2: CSS Layouting Portofolio** pada mata kuliah **Pemrograman Web**[cite: 1, 2]. Proyek ini mengembangkan landing page portofolio pribadi dari Tugas 1 menggunakan kombinasi arsitektur **CSS Grid** untuk tata letak halaman utama dan **Flexbox** untuk komponen internal, lengkap dengan sistem variabel CSS serta dukungan mode gelap (*dark mode*)[cite: 2].

---

## 🔗 Live Demo

- **Demo Halaman (GitHub Pages):** 
 https://rnglich.github.io/TugasWeb-Pertemuan2-CSS/

- **Repository:** 
https://github.com/rnglich/TugasWeb-Pertemuan2-CSS

---

## 🛠️ Implementasi Spesifikasi Tugas

Proyek ini dibangun dengan memenuhi seluruh daftar persyaratan (*requirements*) teknis yang diinstruksikan[cite: 2]:

### 1. Struktur Utama Berbasis CSS Grid
- Menggunakan CSS Grid pada container utama (`.layout-container` / `body`) untuk membagi tata letak induk secara terstruktur[cite: 2].
- Pemanfaatan `grid-template-areas` / `grid-template-columns` untuk memosisikan area `<header>`, `<nav>`, `<aside>`, `<main>`, dan `<footer>` secara presisi[cite: 2].

### 2. Flexbox pada Komponen Internal
- **Komponen 1 (Navigasi):** Elemen menu `<nav>` ditata menggunakan `display: flex` dengan pengaturan `justify-content: space-between` dan `align-items: center` untuk perataan tautan navigasi[cite: 2].
- **Komponen 2 (Kartu Portofolio / Skills):** Daftar kartu proyek dan badge keahlian diatur menggunakan `display: flex` beserta `flex-wrap: wrap` dan `gap` untuk tata letak yang fleksibel dan dinamis[cite: 2].

### 3. Elemen Semantik HTML5
- Mempertahankan dan mengoptimalkan kerangka semantik dari Tugas 1 yang mencakup tag `<header>`, `<aside>`, `<main>`, dan `<nav>` untuk hierarki dokumen yang terstandarisasi dan ramah aksesibilitas[cite: 2].

### 4. CSS Custom Properties (`:root` Variables)
Mengimplementasikan lebih dari 5 variabel global di `:root` untuk kemudahan pemeliharaan tema[cite: 2]:
- `--bg-primary`: Warna latar belakang utama[cite: 2].
- `--text-primary`: Warna teks utama[cite: 2].
- `--accent-color`: Warna aksen/sorotan tombol dan tautan[cite: 2].
- `--font-main`: Jenis tipografi utama dokumen.
- `--spacing-base`: Satuan dasar jarak antarelemen (*gap/margin/padding*).
- `--card-bg`: Warna latar kartu komponen.

### 5. Aturan Global Box-Sizing
- Mendeklarasikan aturan universal reset `*, *::before, *::after { box-sizing: border-box; }` untuk memastikan perhitungan ukuran elemen mencakup batas *padding* dan *border* secara konsisten di semua peramban[cite: 2].

### 6. Standar Penulisan Kode (BEM / Kebab-Case)
- Struktur penamaan kelas CSS disusun secara rapi dan modular menggunakan metodologi **BEM** (*Block-Element-Modifier*) dan penamaan berbasis **kebab-case** (misalnya `.card-profile`, `.navbar__link--active`)[cite: 2].

### 7. Fitur Bonus: Mode Gelap Otomatis
- Menyertakan media query `@media (prefers-color-scheme: dark)` untuk mendeteksi preferensi tema sistem pengguna dan menyesuaikan nilai variabel CSS warna secara otomatis tanpa JavaScript tambahan[cite: 2].

---

## 📋 Checklist Persyaratan

| No | Kriteria / Syarat | Status | Deskripsi Implementasi |
|:--:|:---|:------:|:-----------------------|
| 1 | HTML5 Semantik (`header`, `aside`, `main`, `nav`)[cite: 2] | ✅ Terpenuhi | Struktur halaman tersusun atas tag semantik standar[cite: 2] |
| 2 | Minimal 5 CSS Variables di `:root`[cite: 2] | ✅ Terpenuhi | 6+ variabel warna, jarak, dan tipografi diatur di `:root`[cite: 2] |
| 3 | `box-sizing: border-box` global[cite: 2] | ✅ Terpenuhi | Reset universal diterapkan pada `*`, `::before`, `::after`[cite: 2] |
| 4 | CSS Grid untuk struktur utama[cite: 2] | ✅ Terpenuhi | Grid template layout induk membagi seksi utama[cite: 2] |
| 5 | Flexbox untuk minimal 2 komponen[cite: 2] | ✅ Terpenuhi | Digunakan pada navbar dan kartu portofolio/galeri[cite: 2] |
| 6 | Kode rapi (BEM / kebab-case)[cite: 2] | ✅ Terpenuhi | Penamaan konsisten tanpa selector gaya sembarangan[cite: 2] |
| ⭐ | **Bonus:** Dark Mode `@media (prefers-color-scheme: dark)`[cite: 2] | ✅ Terpenuhi | Penyesuaian tema otomatis berbasis preferensi perangkat[cite: 2] |

---
