# Website Desa Bandungan

Website profil Desa Bandungan, Kecamatan Saradan, Kabupaten Madiun, Jawa Timur yang dibuat sebagai bagian dari Program BBK 7 Universitas Airlangga periode Januari 2026.

![Desa Bandungan](https://img.shields.io/badge/Desa-Bandungan-5a6b3c?style=for-the-badge)
![BBK 7 Unair](https://img.shields.io/badge/BBK-7-Unair_2026-a67c52?style=for-the-badge)

## 📋 Tentang Website

Website ini dirancang dengan desain editorial magazine-style yang modern dan elegan, menampilkan informasi lengkap tentang Desa Bandungan serta program-program BBK 7 yang dilaksanakan.

### Fitur Utama

- **Hero Section dengan Video** - Tampilan pembuka yang menarik dengan video landscape desa
- **Profil Desa** - Informasi lengkap tentang visi, misi, dan potensi desa
- **Statistik & Demografi** - Data penduduk dan wilayah yang informatif
- **Program BBK 7** - Detail program "Pasar Bersih Bernilai" dan program pendukung lainnya
- **Galeri Foto** - Dokumentasi kegiatan BBK 7 dalam format scrollable gallery
- **Tim BBK 7** - Profil lengkap anggota tim BBK 7
- **Form Kontak** - Integrasi WhatsApp untuk komunikasi langsung
- **Responsive Design** - Optimal di semua perangkat (desktop, tablet, mobile)

## 🎨 Design System

### Color Palette

```css
--earth-dark: #2d3319   /* Hijau tua untuk header dan footer */
--earth-mid: #5a6b3c    /* Hijau sedang untuk aksen */
--earth-light: #8a9a6d  /* Hijau muda untuk gradients */
--sand: #d4c5aa         /* Pasir untuk highlights */
--cream: #f5f1e8        /* Krem untuk background */
--rust: #a67c52         /* Coklat karat untuk CTAs */
```

### Typography

- **Heading**: Playfair Display (Serif)
- **Body**: Source Sans 3 (Sans-serif)

## 📁 Struktur Folder

```
desa-bandungan/
├── index.html
├── README.md
└── assets/
    ├── logo.png
    ├── video/
    │   └── desa.mp4
    ├── template/
    │   ├── sawah.png
    │   └── pasar.png
    ├── dokum/
    │   ├── foto1.png
    │   ├── foto2.png
    │   ├── foto3.png
    │   ├── foto4.png
    │   ├── foto5.png
    │   └── foto6.png
    ├── anggota/
    │   ├── nada.png
    │   ├── elga.png
    │   ├── sasa.png
    │   ├── hasan.png
    │   ├── roofi.png
    │   ├── viva.png
    │   ├── hasna.png
    │   └── ari.png
    └── foto2.jpeg - foto7.jpeg
```

## 🚀 Cara Menggunakan

### 1. Setup Awal

```bash
# Clone atau download repository
git clone [repository-url]
cd desa-bandungan
```

### 2. Persiapan Assets

Siapkan file-file berikut dan letakkan di folder yang sesuai:

#### Logo & Video
- `assets/logo.png` - Logo Desa Bandungan (format PNG, ukuran 512x512px)
- `assets/video/desa.mp4` - Video hero landscape desa (max 5MB, 1920x1080, durasi 10-30 detik)

#### Template Images
- `assets/template/sawah.png` - Foto sawah produktif
- `assets/template/pasar.png` - Foto pasar tradisional

#### Dokumentasi BBK 7
- `assets/dokum/foto1.png` - Foto kelompok BBK 7
- `assets/dokum/foto2.png` - Foto kegiatan pasar
- `assets/dokum/foto3.png` - `foto6.png` - Foto kegiatan lainnya

#### Foto Anggota
- `assets/anggota/[nama].png` - Foto profil setiap anggota (format persegi, min 400x400px)

#### Program Pendukung
- `assets/foto2.jpeg` - `foto7.jpeg` - Foto program pendukung BBK 7

### 3. Konfigurasi

Edit file `index.html` untuk menyesuaikan:

#### Informasi Kontak
```html
<!-- Line ~950 -->
<div>0351-123456</div> <!-- Ganti dengan nomor telepon -->
<div>desabandungan@madiunkab.go.id</div> <!-- Ganti dengan email -->
<a href="https://wa.me/6281234567890">+62 812-3456-7890</a> <!-- Ganti nomor WA -->
```

#### WhatsApp Integration
```javascript
// Line ~1050
const message = `...`;
window.open(`https://wa.me/6281234567890?text=${message}`, '_blank');
// Ganti 6281234567890 dengan nomor WA desa
```

### 4. Deploy

Website ini adalah **static HTML** dan dapat di-deploy ke berbagai platform:

#### GitHub Pages (Gratis)
```bash
git add .
git commit -m "Initial commit"
git push origin main
# Aktifkan GitHub Pages di Settings > Pages
```

#### Netlify (Gratis)
1. Drag & drop folder ke [Netlify Drop](https://app.netlify.com/drop)
2. Website langsung online!

#### Vercel (Gratis)
```bash
npm i -g vercel
vercel
```

#### Hosting Tradisional
Upload semua file via FTP/cPanel ke:
- `/public_html/` atau
- `/www/` atau
- Folder yang ditentukan hosting

## 📱 Responsiveness

Website ini fully responsive dengan breakpoints:

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## 🔧 Kustomisasi

### Mengubah Warna

Edit variabel CSS di bagian `<style>`:

```css
:root {
    --earth-dark: #2d3319;  /* Ubah sesuai keinginan */
    --earth-mid: #5a6b3c;
    /* dst... */
}
```

### Mengubah Font

Ganti Google Fonts import di `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=[Font-Pilihan]&display=swap" rel="stylesheet">
```

### Menambah Section Baru

Ikuti pola yang ada:

```html
<section id="section-baru" class="py-20">
    <div class="section-offset fade-in">
        <div class="text-sm uppercase tracking-widest mb-12" 
             style="color: var(--earth-mid); font-weight: 600;">
            Label Section
        </div>
        <h2 class="display-2 mb-8">Judul Section</h2>
        <!-- Konten -->
    </div>
</section>
```

## 🎯 Program BBK 7

### Program Utama: Pasar Bersih Bernilai

Program fokus pada pengelolaan sampah pasar melalui pemilahan dan komposting.

**Tahapan:**
1. Observasi & Pendekatan Pedagang
2. Sosialisasi Pemilahan Sampah
3. Implementasi Pemilahan & Komposter
4. Monitoring & Evaluasi
5. Penyusunan SOP & Serah Terima

### Program Pendukung

- Hari Pasar Bersih
- Dapur Gizi Pasar
- Pojok Gizi & Kesehatan
- Kelas Masa Depan Remaja
- Literasi Digital Remaja
- Aktivasi Media & Arsip Desa

## 👥 Tim BBK 7 Universitas Airlangga

| Nama | Posisi |
|------|--------|
| Nada | Ketua |
| Elga | Sekretaris |
| Sasa | Bendahara |
| Hasan | Acara |
| Roofi' | Acara |
| Viva | Humas |
| Hasna | PDD |
| Ari | PDD |

**Dosen Pembimbing:** Samidi

## 📊 Data Desa Bandungan

- **Penduduk:** 4.523 jiwa
- **Kepala Keluarga:** 1.289 KK
- **Luas Wilayah:** 312 hektar
- **Jumlah Dusun:** 3 dusun

### Potensi

- Sawah produktif: 180 Ha
- Kebun campuran: 45 Ha
- Pasar tradisional aktif
- UMKM kuliner: 23 unit
- Toko kelontong: 15 unit

## 🛠️ Teknologi yang Digunakan

- **HTML5** - Struktur website
- **CSS3** - Styling dan animasi
- **JavaScript (Vanilla)** - Interaktivitas
- **Tailwind CSS (CDN)** - Utility classes
- **Google Fonts** - Typography

**Tidak ada dependencies** yang perlu diinstall!

## ⚡ Performance Tips

### Optimasi Video
```bash
# Compress video menggunakan FFmpeg
ffmpeg -i input.mp4 -vcodec libx264 -crf 28 -preset slow output.mp4
```

### Optimasi Gambar
```bash
# Resize dan compress menggunakan ImageMagick
convert input.jpg -resize 1920x1080^ -quality 85 output.jpg
```

### Lazy Loading (Optional)

Tambahkan `loading="lazy"` pada image tags:

```html
<img src="assets/foto.jpg" loading="lazy" alt="Deskripsi">
```

## 📖 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ⚠️ IE11 (partial support)

## 🐛 Troubleshooting

### Video tidak autoplay di mobile
- Pastikan attribute `muted` dan `playsinline` ada
- Video harus ukuran < 5MB untuk performa optimal

### Gambar tidak muncul
- Cek path file sudah benar
- Cek ekstensi file (.png, .jpg, .jpeg)
- Pastikan folder `assets/` ada di root directory

### Form WhatsApp tidak berfungsi
- Cek nomor WhatsApp sudah format internasional (62xxx)
- Pastikan tidak ada karakter spesial di URL

## 📝 License

Website ini dibuat untuk kepentingan program BBK 7 Universitas Airlangga di Desa Bandungan, Madiun.

© 2026 BBK 7 Universitas Airlangga - Desa Bandungan

## 📞 Kontak

**Desa Bandungan**
- Alamat: Jl. Raya Bandungan, Kec. Saradan, Kab. Madiun, Jawa Timur
- Telepon: -
- Email: -
- WhatsApp: -

**Tim BBK 7**
- Instagram: [@bbk7unair_bandungan](https://www.instagram.com/bbk7unair_bandungan/)

---

**Dibuat dengan ❤️ oleh Tim BBK Universitas Airlangga - Bandungan**

*"Bandungan josjis - Menuju Desa yang Maju, Sejahtera, dan Berkelanjutan"*