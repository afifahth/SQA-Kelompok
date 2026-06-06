# Control Flow Testing

## Definisi
Control Flow Testing berfokus pada pemeriksaan control logic untuk memastikan seluruh jalur eksekusi berjalan dengan benar.

## Pengujian Control Flow

| Kondisi | Hasil Yang Diharapkan | Hasil | Status |
|---------|---------|---------|---------|
| Login berhasil | Redirect ke Dashboard | Redirect ke Dashboard | Passed |
| Login gagal | Pesan error login | Pesan error login | Passed |
| Produksi dengan stok cukup | Produksi berhasil | Produksi berhasil | Passed |
| Produksi dengan stok tidak cukup | Produksi ditolak | Produksi ditolak | Passed |
| Pembelian bahan | Stok bertambah | Stok bertambah | Passed |
