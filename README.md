# Fun English English Training Centre - Website

Folder siap deploy (HTML statis + Tailwind CDN, tanpa backend).

Struktur:
- index.html : seluruh halaman (logo sudah tertanam, tidak bergantung folder assets)
- assets/brosur-fun-english.jpg : brosur yang tampil di hero
- assets/logo-fun-english-160.jpg : logo (cadangan)

PENTING: upload SELURUH isi folder (index.html + folder assets), bukan hanya index.html.

Cara deploy:
1. Netlify: buka app.netlify.com/drop lalu drag seluruh folder. Untuk update, drag ulang ke site yang sama.
2. Vercel: drag folder ke vercel.com/new, atau jalankan `npx vercel --prod` di dalam folder.
3. Hosting biasa: upload seluruh isi folder ke public_html.

Sebelum publish, cek:
- Nama, foto, dan sertifikasi pengajar di bagian Tim Pengajar (saat ini masih "Nama Pengajar").
- Pin peta: Google Maps memakai pencarian alamat, pastikan pin jatuh di lokasi yang benar.
- Nomor WA Cabang Kranji: brosur 0856-0715-2724, prompt 0857-0715-2724. Saat ini memakai 0856.
- Harga per paket: saat ini hanya "mulai Rp100.000" (biaya awal). Ganti jika ada rincian resmi.
- Jadwal kelas: tabel memakai jam 12.00-19.00 Senin-Sabtu dari brosur. Sesuaikan jika per level berbeda.

Fitur:
- Navbar: Home | Programs | Trainers | Schedule | Placement Test | Contact Us
- Placement test 5 soal di halaman, hasil langsung mengarah ke WhatsApp
- Form pendaftaran: pilih paket dan cabang, lalu pesan terkirim ke WA cabang
- Peta Google Maps untuk kedua cabang
- Tombol WhatsApp mengambang dan tautan Instagram/Facebook
- Tidak ada Student Portal dan pembayaran online (QRIS/transfer) otomatis; perlu backend dan payment gateway terpisah jika dibutuhkan
