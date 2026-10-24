LINK PENDEK VIA GITHUB PAGES
============================
Isi folder ini:
  index.html       -> link publik   (https://NAMA.github.io/)
  bps/index.html   -> link admin    (https://NAMA.github.io/bps/)

1. Buka config.js (cukup satu file), ganti GANTI_DENGAN_LINK_EXEC_ANDA dengan link /exec
   (Apps Script > Deploy > Manage deployments > Web app URL). Contoh:
   https://script.google.com/macros/s/AKfy.../exec
2. Di GitHub, buat repository baru bernama NAMA.github.io (NAMA = username GitHub Anda)
   supaya alamatnya paling pendek. Repository lain juga bisa, tapi alamatnya jadi NAMA.github.io/NAMA-REPO/.
3. Unggah isi folder ini (index.html, config.js, dan folder bps) ke repository.
4. Settings > Pages > Source: "Deploy from a branch" > Branch: main, folder: / (root) > Save.
5. Tunggu 1-2 menit, lalu buka https://NAMA.github.io/.
6. Opsional: di Code.gs isi SHORT_PUBLIC_URL = 'https://NAMA.github.io/' supaya tombol Bagikan,
   QR code, dan Lihat Publik memakai link pendek. Lalu Deploy > New version.

Catatan: repository GitHub Pages gratis bersifat publik, jadi link /exec (termasuk ?page=admin) bisa
dilihat orang yang membuka kodenya. Halaman admin tetap dilindungi password. Jika tidak ingin link
admin tampil, hapus folder bps dan gunakan link /exec?page=admin secara langsung.
Jika link /exec berubah (mis. membuat "New deployment"), ubah EXEC_URL di config.js.
