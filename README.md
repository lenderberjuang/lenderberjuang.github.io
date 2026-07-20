# Lender Berjuang — Starter Template

Template dasar Jekyll untuk situs Lender Berjuang, siap di-upload ke GitHub Pages.

## Cara Pakai (langkah demi langkah)

### 1. Buat repository di GitHub
- Login ke github.com
- Klik "New repository"
- Nama repo **harus** persis: `USERNAME-KAMU.github.io` (ganti USERNAME-KAMU dengan username GitHub kamu)
- Pilih "Public", jangan centang "Add README" (karena sudah ada)

### 2. Upload file-file ini ke repo
Cara termudah tanpa command line:
- Buka repo yang baru dibuat di github.com
- Klik "Add file" > "Upload files"
- Drag semua file & folder dari template ini ke situ
- Klik "Commit changes"

Atau kalau pakai GitHub Desktop:
- Clone repo kosong ke komputer
- Copy semua isi folder template ini ke folder repo tersebut
- Commit lalu Push

### 3. Aktifkan GitHub Pages
- Di repo, buka Settings > Pages
- Source pilih branch `main`, folder `/ (root)`
- Simpan. Tunggu 1-2 menit, web kamu akan aktif di `https://USERNAME-KAMU.github.io`

### 4. Edit `_config.yml`
Buka file `_config.yml`, ganti bagian `url` dengan alamat GitHub Pages kamu (hapus tanda `#` di depan baris itu).

## Struktur Folder

```
lenderberjuang-site/
├── _config.yml          <- pengaturan situs (judul, deskripsi, menu)
├── index.md             <- halaman beranda
├── about.md              <- halaman "Tentang Kami"
├── proses-hukum.md       <- halaman ringkasan proses hukum
└── _posts/                <- semua artikel update ada di sini
    └── 2026-07-20-selamat-datang.markdown   <- contoh artikel
```

## Menambah Artikel Baru

1. Buat file baru di dalam folder `_posts`
2. Format nama file **wajib**: `TAHUN-BULAN-TANGGAL-judul-singkat.markdown`
   Contoh: `2026-08-01-sidang-kedua-digelar.markdown`
3. Isi bagian atas file (di antara dua baris `---`) dengan judul, tanggal, kategori — contoh formatnya bisa dilihat di file artikel contoh
4. Tulis isi artikel di bawahnya pakai Markdown
5. Upload/push ke GitHub — artikel otomatis muncul di beranda dalam 1-2 menit

## Menambah Halaman Baru (bukan artikel, misal "FAQ" atau "Cara Bergabung")

1. Buat file baru di folder utama (sejajar dengan `about.md`), misal `faq.md`
2. Isi bagian atas dengan:
   ```
   ---
   layout: page
   title: FAQ
   permalink: /faq/
   ---
   ```
3. Tulis isinya di bawah, lalu upload

## Belajar Markdown Cepat (10 menit)

- `# Judul` = judul besar
- `## Sub judul` = judul lebih kecil
- `**tebal**` = **tebal**
- `*miring*` = *miring*
- `- item` = bullet list
- `[teks](url)` = link
- Baris kosong = paragraf baru

## Kalau Mau Preview di Komputer Sebelum Upload (opsional, agak teknis)

Ini butuh install Ruby & Jekyll — boleh dilewati dulu kalau belum siap, karena upload langsung ke GitHub juga otomatis menampilkan hasilnya di web dalam 1-2 menit tanpa perlu preview lokal.
