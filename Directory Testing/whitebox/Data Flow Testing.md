# Data Flow Testing

## Definisi
Data Flow Testing adalah teknik pengujian yang berfokus pada aliran data dalam sistem untuk memastikan data diproses dengan benar dari input hingga output.

## Pengujian Data Flow

| Komponen | Input | Proses | Output | Status |
|---------|---------|---------|---------|---------|
| Login | Username dan Password | Validasi akun | Dashboard | Passed |
| Data Bahan | Data bahan | Simpan database | Data tampil pada tabel | Passed |
| Pembelian | Jumlah pembelian | Update stok | Stok bertambah | Passed |
| Produksi | Jumlah produksi | Kurangi stok | Stok berkurang | Passed |
| Laporan | Data transaksi | Generate laporan | Laporan tampil | Passed |
