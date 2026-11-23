# Simulasi Pembiayaan Rumany

Simulator pembiayaan rumah Rumany (Divisi Lending, KSPPS Syirkah Kebaikan Indonesia).
Satu file `index.html`, tanpa server dan tanpa instalasi. Logo KSPPS dan Rumany sudah tertanam di dalam file.

## Isi
- Tiga program: Skema Dasar (margin 8%), Margin Normal 5%, Promo 3%
- Syarat: DP minimal 25%, margin dasar 3–8% per tahun, tenor maksimal 15 tahun
- Cicilan 24 bulan pertama dan cicilan setelahnya (pembagian margin mengikuti skema sheet MASTER)
- Bandingkan DP/tenor/margin, jadwal pembayaran, cocokkan dengan kemampuan klien
- Skema yang tidak lolos analisa Credit Risk diberi cap **DITOLAK**, dan tombol salin WhatsApp dimatikan

## Cara upload ke GitHub Pages
1. Buat repository baru di GitHub, misalnya `simulasi-rumany`.
2. Klik **Add file → Upload files**, lalu unggah `index.html` (dan `README.md` ini).
3. Klik **Commit changes**.
4. Buka **Settings → Pages**. Di bagian *Build and deployment*, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
5. Tunggu 1–2 menit. Alamatnya: `https://<username>.github.io/simulasi-rumany/`

## Versi publik dan internal
File ini adalah **versi publik** (`AKSES_PENUH = false` di bagian atas `<script>`):
panel Analisa Credit Risk dihapus dan halaman selalu dalam tampilan klien.

Catatan: hitungan berjalan di browser, jadi asumsi perhitungan (pembayaran ke pemilik rumah dan compounding)
tetap bisa dilihat lewat *View Source*. Jangan mengubah `AKSES_PENUH` menjadi `true` di repository publik.

Angka di halaman adalah simulasi. Nilai final mengikuti akad setelah analisa kelayakan oleh KSPPS Syirkah Kebaikan Indonesia.
