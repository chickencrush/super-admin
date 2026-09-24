CHICKEN CRUSH V7.1.1 — SMART IMPORT 3-IN-1

PERBAIKAN UTAMA
1. Smart Import menjadi satu panel untuk:
   - Menu Performance
   - Penjualan per Waktu
   - Kategori Penjualan: Dine In, Take Away, ShopeeFood, GrabFood, GoFood, ESB Order

2. Pembacaan file diperkuat:
   - XLSX dibaca langsung dari struktur ZIP/XML tanpa konversi Google Drive.
   - Multi-sheet otomatis memilih sheet terbaik.
   - XLS lama mencoba HTML/Text lalu fallback konversi Drive.
   - Header lebih fleksibel.

3. Sinkronisasi dashboard:
   - Setiap import sukses menghapus cache live backend.
   - Owner Dashboard menerima sinyal refresh otomatis.
   - Kategori Penjualan masuk ke sheet baru 'Kategori Penjualan DB'.
   - Media Penjualan dashboard membaca DB baru dan fallback ke sheet lama untuk outlet yang belum diimport.

4. Penjualan per Waktu:
   - Interval 00:00 - 01:00 sekarang disimpan sebagai jam awal 00:00.

INSTALASI
- Ganti Code.gs dengan V7.1.1.
- Save.
- Deploy > Manage deployments > Edit > New version > Deploy.
- Replace repository Owner dengan paket V7.1.1.
- Tidak perlu setup sheet manual; 'Kategori Penjualan DB' dibuat otomatis saat import pertama.
- Team V7.1.0 tetap kompatibel dan tidak wajib diupdate.
