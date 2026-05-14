# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0] - 2024-01-15

### 🎉 Major Release

#### ✨ Added
- **SEO Optimization**
  - Sitemap.xml untuk search engine indexing
  - Robots.txt untuk web crawler guidance
  - Structured Data (JSON-LD) untuk rich snippets di Google
  - Open Graph tags lengkap untuk social media preview
  - Twitter Cards untuk preview di Twitter
  - Canonical URL untuk mencegah duplicate content
  - Meta keywords lengkap dalam bahasa Indonesia

- **PWA Support**
  - Manifest.json untuk Progressive Web App
  - Installable sebagai aplikasi mobile/desktop
  - Theme color dan app icons configuration
  - Offline-ready capabilities

- **Smart Layout Algorithm**
  - Collision detection untuk menghindari overlap elemen
  - Automatic layering berdasarkan dependencies
  - Balanced distribution untuk tabel yang banyak
  - Dynamic spacing dan positioning

- **Junction Table Detection**
  - Deteksi otomatis many-to-many relationships
  - Smart identification dari junction tables
  - Proper M:N relationship visualization

- **Documentation**
  - README lengkap dalam Bahasa Indonesia
  - Peringatan penting tentang database harus kosong
  - Panduan export database yang benar (MySQL, PostgreSQL, phpMyAdmin)
  - Informasi lisensi MIT lengkap
  - Buy Me a Coffee integration untuk support

#### 🔧 Changed
- Update meta tags dari English ke Indonesian
- Improve responsive design untuk mobile devices
- Enhanced color scheme dan visual design
- Better error handling dan user feedback

#### 🛠️ Technical Improvements
- Vercel.json configuration untuk deployment optimization
- .htaccess untuk Apache server optimization
- Security headers implementation
- Compression dan caching configuration
- No npm dependencies - pure HTML/CSS/JS

#### 📄 Files Added
- `sitemap.xml` - Search engine sitemap
- `robots.txt` - Web crawler instructions
- `manifest.json` - PWA manifest
- `vercel.json` - Vercel deployment config
- `.htaccess` - Apache server config
- `CHANGELOG.md` - This file

#### 🐛 Bug Fixes
- Fixed layout collision issues
- Improved attribute positioning
- Better handling of large schemas
- Enhanced relationship line routing

#### 💖 Community
- Added Buy Me a Coffee support link
- GitHub sponsors ready
- Open source dengan MIT License
- Contribution guidelines

---

## [1.0] - 2024-01-01

### Initial Release

#### Features
- Basic ERD generation dari SQL files
- Chen Notation support
- Export to .drawio format
- Basic layout algorithm
- Foreign key detection
- Primary key identification

---

## Future Plans

### [2.1] - Planned
- [ ] Multiple database dialect support
- [ ] Custom color themes
- [ ] Export to PNG/SVG
- [ ] Zoom and pan controls
- [ ] Undo/redo functionality

### [3.0] - Planned
- [ ] Real-time collaboration
- [ ] Cloud storage integration
- [ ] Version history
- [ ] Template library
- [ ] AI-powered suggestions

---

**Developed with ❤️ by [Andy Pratama](https://github.com/andypratama3)**

For more information, visit: https://website-generate-erd-chen.vercel.app
