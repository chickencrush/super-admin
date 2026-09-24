CHICKEN CRUSH V7.1.2 — SMART IMPORT SALES RECAP FIX

Diuji terhadap sample:
Sales Recapitulation Report_LDA2GODEANVIEW_17901801382835.xlsx

STRUKTUR SAMPLE YANG SEKARANG DIDUKUNG
- Header tabel berada di baris 13
- Sales Date berupa serial tanggal Excel
- Sales In Time
- Branch
- Visit Purpose
- Pax Total
- Net Sales
- Grand Total

SATU FILE SALES RECAPITULATION SEKARANG MENGISI 2 DATABASE SEKALIGUS
1. ESB Waktu DB
   - Mengelompokkan Sales In Time menjadi bucket 1 jam
   - Contoh 08:10:06 -> 08:00
   - Bill, Pax, Net Sales, Grand Total dijumlahkan per tanggal/outlet/jam

2. Kategori Penjualan DB
   - Dine In
   - Take Away
   - ShopeeFood
   - GrabFood
   - GoFood
   - ESB Order
   - ESB ORDER DELIVERY digabung ke ESB Order
   - Nilai kategori menggunakan Grand Total agar lebih dekat dengan omset transaksi

PENYESUAIAN OUTLET
Chicken Crush Godean -> Godean
Chicken Crush Signature -> CCS
Chicken Crush Tamansiswa -> Tamsis

UI INPUT CENTER
- Smart Import menjadi panel default saat Input Center dibuka
- Navigasi dibuat lebih ringkas dan sticky
- Drop area dipindahkan lebih dekat ke bagian atas
- Mobile: selector horizontal, Smart Import tetap muncul paling depan

STABILITAS IMPORT
- Timeout Smart Import dinaikkan menjadi 90 detik
- File besar tidak di-retry otomatis
- Request ID dipertahankan agar retry manual tidak menulis data dua kali
- Dashboard Owner tetap auto-refresh setelah import sukses

INSTALL
1. Ganti Code.gs dengan AppsScript_CCI_Shared_API_V7_1_2_SMART_IMPORT_SALES_RECAP.gs
2. Save
3. Deploy > Manage deployments > Edit > New version > Deploy
4. Replace repository Owner dengan paket OWNER V7.1.2
5. Team tidak perlu diganti.
