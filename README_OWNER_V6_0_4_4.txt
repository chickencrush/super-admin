CHICKEN CRUSH V6.0.4.4 — DATA INPUT CENTER MULTI-DAY

MENU PERFORMANCE
- Tetap tersedia Isi Manual.
- Ditambah mode Input Banyak Hari.
- Pilih Outlet, Kategori, Nama Menu, lalu isi Qty dan Nilai Penjualan untuk banyak tanggal.
- Hari kosong tidak dikirim.
- Penyimpanan aman menggunakan upsert untuk data Input Center.

PENJUALAN PER WAKTU
- Tetap tersedia Isi Manual.
- Ditambah mode Input Banyak Hari.
- Pilih Outlet dan satu interval jam.
- Isi Qty, Nett Sales, dan Grand Total untuk banyak tanggal.
- Pilihan jam sekarang berupa interval 1 jam:
  00:00 - 01:00
  01:00 - 02:00
  ...
  23:00 - 00:00
- Untuk outlet non-CCS, pilihan tetap mengikuti jam operasional database mulai bucket 08:00.

BACKEND
Code.gs wajib diganti ke V6.0.4.4 dan Web App wajib Deploy New Version.
Tidak perlu menjalankan setup baru karena tidak ada sheet baru.
