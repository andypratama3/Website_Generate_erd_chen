<div align="center">

# 🗂️ ERD Generator - Notasi Chen

[![Release](https://img.shields.io/badge/release-v2.0-blue.svg)](https://github.com/andypratama3/Website_Generate_erd_chen/releases)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Live Demo](https://img.shields.io/badge/demo-live-success.svg)](https://website-generate-erd-chen.vercel.app)
[![Vercel](https://img.shields.io/badge/deployed%20on-Vercel-black.svg)](https://vercel.com)

**Tool berbasis web untuk menghasilkan Entity Relationship Diagram (ERD) dengan Notasi Chen secara otomatis dari struktur database Anda.**

[🚀 Live Demo](https://website-generate-erd-chen.vercel.app) • [📖 Dokumentasi](#dokumentasi) • [🐛 Laporkan Bug](https://github.com/andypratama3/Website_Generate_erd_chen/issues) • [✨ Request Fitur](https://github.com/andypratama3/Website_Generate_erd_chen/issues)

</div>

---

## 📋 Daftar Isi

- [Tentang Project](#tentang-project)
- [⚠️ Peringatan Penting](#️-peringatan-penting)
- [Fitur Utama](#fitur-utama)
- [Cara Menggunakan](#cara-menggunakan)
- [Persyaratan](#persyaratan)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)
- [Pembuat](#pembuat)
- [Dukungan](#dukungan)

---

## 🎯 Tentang Project

**ERD Generator - Notasi Chen** adalah tool berbasis web yang saya buat untuk mempermudah proses pembuatan Entity Relationship Diagram dari struktur database. Tool ini secara otomatis mengkonversi skema database Anda menjadi diagram ERD visual menggunakan gaya Notasi Chen, membuat desain dan dokumentasi database menjadi lebih mudah dan cepat.

### Kenapa Tool Ini?

- 🎨 **Representasi Visual**: Visualisasikan struktur database Anda secara instan
- ⚡ **Cepat & Mudah**: Tidak perlu menggambar manual
- 🎓 **Edukatif**: Sempurna untuk belajar desain database
- 💼 **Profesional**: Hasilkan diagram siap dokumentasi
- 🆓 **Gratis & Open Source**: Gunakan kapan saja, di mana saja

---

## ⚠️ Peringatan Penting

### 🚨 **PENTING: Database Harus Kosong Sebelum Di-Export**

Sebelum generate ERD, pastikan bahwa:

1. ✅ **Database Anda HANYA berisi struktur tabel (schema)**
2. ✅ **Semua tabel kosong (tidak ada data/rows)**
3. ✅ **Hanya ada statement CREATE TABLE**

### Kenapa Ini Penting:

- ❌ **Jika database berisi data**, file export akan sangat besar
- ❌ **File besar akan membuat generator gagal atau freeze**
- ❌ **Statement INSERT tidak diperlukan untuk generate ERD**
- ✅ **Hanya struktur tabel dan relasi yang dibutuhkan**

### Cara Export yang Benar:

**Untuk MySQL/MariaDB:**
```bash
# Export struktur saja (tanpa data)
mysqldump -u username -p --no-data nama_database > schema.sql
```

**Untuk PostgreSQL:**
```bash
# Export struktur saja (tanpa data)
pg_dump -U username -s nama_database > schema.sql
```

**Untuk phpMyAdmin:**
1. Pilih database Anda
2. Klik "Export"
3. Pilih metode "Custom"
4. Di bagian "Tables", pilih "Structure" saja
5. Uncheck "Data"
6. Klik "Go"

---

## ✨ Fitur Utama

- 🎨 **ERD Notasi Chen**: Generate diagram menggunakan gaya notasi Chen klasik
- 📊 **Deteksi Otomatis**: Otomatis mendeteksi tabel, kolom, dan relasi
- 🔄 **Generate Real-time**: Generate diagram instan dari file SQL
- 💾 **Export .drawio**: Download ERD Anda dalam format .drawio
- 🌐 **Berbasis Web**: Tidak perlu instalasi, buka langsung di browser
- 📱 **Responsive Design**: Berfungsi di desktop, tablet, dan mobile
- ⚡ **Proses Cepat**: Dioptimalkan untuk generate diagram dengan cepat
- 🎯 **Relasi Akurat**: Mengenali foreign key dan relasi dengan tepat
- 🔗 **Deteksi M:N**: Otomatis mendeteksi junction table untuk relasi many-to-many
- 🎨 **Smart Layout**: Algoritma layout yang menghindari collision antar elemen

---

## 🚀 Cara Menggunakan

### Tidak Perlu Instalasi!

Tool ini adalah **HTML murni** yang bisa langsung dibuka di browser. Tidak perlu `npm install` atau setup apapun!

### Cara Menjalankan Lokal:

1. **Clone repository**
   ```bash
   git clone https://github.com/andypratama3/Website_Generate_erd_chen.git
   cd Website_Generate_erd_chen
   ```

2. **Buka file HTML**
   ```bash
   # Langsung buka index.html di browser
   open index.html
   # atau double-click file index.html
   ```

3. **Atau gunakan Live Server (opsional)**
   ```bash
   # Jika ingin menggunakan live server
   python -m http.server 8000
   # Buka http://localhost:8000
   ```

---

## 📖 Panduan Penggunaan

### Langkah-langkah:

1. **Persiapkan Database Anda**
   - Pastikan database hanya berisi struktur tabel
   - Hapus semua data dari tabel (atau export struktur saja)

2. **Export Schema Database**
   ```bash
   # Contoh MySQL
   mysqldump -u root -p --no-data nama_database > schema.sql
   ```

3. **Upload ke Generator**
   - Kunjungi [https://website-generate-erd-chen.vercel.app](https://website-generate-erd-chen.vercel.app)
   - Klik "Upload SQL File" atau drag & drop file SQL Anda
   - Klik "Generate ERD"

4. **Lihat & Download**
   - Review ERD yang dihasilkan
   - Download dalam format .drawio
   - Gunakan untuk dokumentasi atau presentasi

### Format SQL yang Didukung:

- ✅ MySQL / MariaDB
- ✅ PostgreSQL
- ✅ SQLite
- ✅ Standard SQL CREATE TABLE statements

---

## 📋 Persyaratan

### Browser yang Didukung:

- Chrome (direkomendasikan) - v90+
- Firefox - v88+
- Safari - v14+
- Edge - v90+

### Persyaratan Database:

- File SQL dengan statement CREATE TABLE
- Foreign key constraints (untuk deteksi relasi)
- Syntax SQL yang valid

### Persyaratan Sistem:

- **Tidak ada!** Ini adalah HTML murni, langsung buka di browser

---

## 🛠️ Teknologi yang Digunakan

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Styling**: Custom CSS dengan Google Fonts (Plus Jakarta Sans, JetBrains Mono)
- **Analytics**: Vercel Analytics
- **Deployment**: Vercel
- **Version Control**: Git & GitHub
- **No Dependencies**: Tidak ada npm packages, murni HTML/CSS/JS

---

## 🤝 Kontribusi

Kontribusi sangat diterima! Berikut cara Anda bisa membantu:

1. Fork repository ini
2. Buat feature branch (`git checkout -b feature/FiturKeren`)
3. Commit perubahan Anda (`git commit -m 'Menambahkan fitur keren'`)
4. Push ke branch (`git push origin feature/FiturKeren`)
5. Buat Pull Request

### Panduan Kontribusi:

- Ikuti style code yang ada
- Tulis commit message yang jelas
- Test perubahan Anda dengan teliti
- Update dokumentasi jika diperlukan

---

## 📄 Lisensi

Project ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail.

```
MIT License

Copyright (c) 2024 Andy Pratama

Dengan ini diberikan izin, tanpa biaya, kepada siapa pun yang mendapatkan salinan
dari perangkat lunak ini dan file dokumentasi terkait ("Perangkat Lunak"), untuk
menggunakan Perangkat Lunak tanpa batasan, termasuk tanpa batasan hak untuk
menggunakan, menyalin, memodifikasi, menggabungkan, menerbitkan, mendistribusikan,
mensublisensikan, dan/atau menjual salinan Perangkat Lunak, dan untuk mengizinkan
orang yang menerima Perangkat Lunak untuk melakukannya, dengan ketentuan berikut:

Pemberitahuan hak cipta di atas dan pemberitahuan izin ini harus disertakan dalam
semua salinan atau bagian substansial dari Perangkat Lunak.

PERANGKAT LUNAK INI DISEDIAKAN "SEBAGAIMANA ADANYA", TANPA JAMINAN APA PUN, BAIK
TERSURAT MAUPUN TERSIRAT, TERMASUK NAMUN TIDAK TERBATAS PADA JAMINAN KELAYAKAN UNTUK
DIPERDAGANGKAN, KESESUAIAN UNTUK TUJUAN TERTENTU DAN NON-PELANGGARAN. DALAM KEADAAN
APA PUN PENULIS ATAU PEMEGANG HAK CIPTA TIDAK BERTANGGUNG JAWAB ATAS KLAIM, KERUSAKAN
ATAU KEWAJIBAN LAINNYA, BAIK DALAM TINDAKAN KONTRAK, KESALAHAN ATAU LAINNYA, YANG
TIMBUL DARI, DARI ATAU SEHUBUNGAN DENGAN PERANGKAT LUNAK ATAU PENGGUNAAN ATAU
TRANSAKSI LAIN DALAM PERANGKAT LUNAK.
```

---

## 👨‍💻 Pembuat

**Andy Pratama**

- GitHub: [@andypratama3](https://github.com/andypratama3)
- Website: [https://website-generate-erd-chen.vercel.app](https://website-generate-erd-chen.vercel.app)
- Repository: [Website_Generate_erd_chen](https://github.com/andypratama3/Website_Generate_erd_chen)

---

## ☕ Support This Project

Jika project ini membantu Anda, pertimbangkan untuk membeli saya kopi! ☕

[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Support-yellow?style=for-the-badge&logo=buy-me-a-coffee)](https://buymeacoffee.com/andypratama3)

**Dukungan Anda sangat berarti untuk pengembangan project ini!** 🙏

### Cara Lain Mendukung:

- ⭐ **Beri bintang repository** di GitHub
- 🐛 **Laporkan bug** atau sarankan fitur via [Issues](https://github.com/andypratama3/Website_Generate_erd_chen/issues)
- 🔀 **Berkontribusi** ke project
- � **Bagikan** ke teman atau kolega yang membutuhkan

---

## 📊 Statistik Project

![GitHub stars](https://img.shields.io/github/stars/andypratama3/Website_Generate_erd_chen?style=social)
![GitHub forks](https://img.shields.io/github/forks/andypratama3/Website_Generate_erd_chen?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/andypratama3/Website_Generate_erd_chen?style=social)

---

## 🔄 Changelog

### Version 2.0 (Terbaru)
- 🎉 Major release dengan peningkatan performa
- ✨ Rendering notasi Chen yang lebih baik
- 🐛 Perbaikan bug dan peningkatan stabilitas
- 📱 Responsiveness mobile yang lebih baik
- ⚡ Generate diagram lebih cepat
- 🎨 Algoritma layout yang lebih pintar dengan collision detection
- 🔗 Deteksi otomatis junction table untuk relasi M:N

[Lihat semua releases](https://github.com/andypratama3/Website_Generate_erd_chen/releases)

---

## 🙏 Ucapan Terima Kasih

- Terima kasih kepada semua kontributor yang telah membantu meningkatkan project ini
- Terinspirasi dari kebutuhan akan tool visualisasi database yang lebih baik
- Dibuat dengan ❤️ untuk komunitas developer

---

<div align="center">

**Dibuat dengan ❤️ oleh [Andy Pratama](https://github.com/andypratama3)**

⭐ **Beri bintang repo ini jika bermanfaat!** ⭐

[⬆ Kembali ke Atas](#-erd-generator---notasi-chen)

</div>
