# portfolio-content

Repository ini adalah sumber data JSON bersama untuk Public Portfolio dan Portfolio-Admin. File yang dibaca publik adalah `data/portfolio.json`.

## Aturan repository

- Gunakan branch utama `main` (atau sesuaikan kedua `config.js` bila menggunakan branch lain).
- Repository perlu **Public** agar visitor website dapat membaca JSON melalui Raw GitHub tanpa token.
- Isi file dianggap publik. Jangan menyimpan password, token GitHub, data sensitif, atau draft rahasia.
- Admin memperbarui file lewat GitHub REST API Contents endpoint. Setiap operasi simpan yang berhasil menghasilkan commit.
- Gunakan `schemaVersion: 1`. Koleksi yang wajib ada: `skills`, `experiences`, `education`, `organizations`, `achievements`, `projects`, dan `socialLinks`. `profile` dan `siteSettings` berupa objek.
- Record di dalam koleksi menggunakan `id`, `createdAt`, dan `updatedAt`. Pertahankan ID yang sudah ada saat mengedit.

## Cek data

Buka `data/portfolio.json` di editor yang memvalidasi JSON. Pastikan tidak ada koma tambahan, string tidak tertutup, atau tipe field yang salah. URL raw setelah repository dibuat:

`https://raw.githubusercontent.com/triagantaraga24/portfolio-content/main/data/portfolio.json`

Jika owner atau repo berbeda, sesuaikan URL tersebut serta konfigurasi pada website.
