# Desk Checking

## Definisi
Desk Checking adalah pengujian bagi para pembuat software yang telah mempelajari bahasa pemrograman dengan sangat baik. Pemeriksaan berfokus pada logika dan nilai variabel pada input dan output yang diperlukan oleh aplikasi.

## Pengujian Desk Checking

| Modul | Kondisi Awal | Input | Output yang Diharapkan | Status |
|---------|---------|---------|---------|---------|
| Login | User belum login | Username dan password benar | Masuk ke Dashboard | Passed |
| Login | User belum login | Username atau password salah | Pesan gagal login | Passed |
| Data Bahan | Data bahan kosong | Tambah data bahan | Data tersimpan | Passed |
| Produksi | Stok tersedia | Input produksi | Stok berkurang sesuai produksi | Passed |
| Pembelian | Stok tersedia | Input pembelian | Stok bertambah sesuai pembelian | Passed |
