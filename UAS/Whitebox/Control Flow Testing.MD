# CONTROL FLOW TESTING

## Definisi

Control Flow Testing merupakan metode White Box Testing yang digunakan untuk memeriksa jalur kontrol dan percabangan yang terdapat dalam program. Pengujian ini dilakukan untuk memastikan bahwa setiap kondisi dan keputusan yang ada dalam sistem dapat dieksekusi sesuai dengan logika yang dirancang.

Pada Inventory Management System, pengujian difokuskan pada modul Login, Data Bahan, dan Transaksi karena ketiga modul tersebut memiliki percabangan logika yang penting.

## Tujuan Pengujian

Pengujian ini bertujuan untuk memastikan seluruh jalur keputusan dalam sistem dapat berjalan dengan benar dan menghasilkan output yang sesuai berdasarkan kondisi yang diberikan pengguna.

### Login

#### Deskripsi Pengujian
Pengujian dilakukan terhadap percabangan proses autentikasi pengguna.

| Kondisi | Hasil Diharapkan | Status |
|----------|------------------|---------|
| Data benar | Dashboard tampil | Passed |
| Data salah | Pesan error login | Passed |
| Data kosong | Peringatan muncul | Passed |

### Data Bahan

#### Deskripsi Pengujian
Pengujian dilakukan terhadap proses penyimpanan data bahan.

| Kondisi | Hasil Diharapkan | Status |
|----------|------------------|---------|
| Data lengkap | Data tersimpan | Passed |
| Data tidak lengkap | Penyimpanan ditolak | Passed |

### Transaksi

#### Deskripsi Pengujian
Pengujian dilakukan terhadap kondisi perubahan stok berdasarkan transaksi.

| Kondisi | Hasil Diharapkan | Status |
|----------|------------------|---------|
| Stok mencukupi | Produksi berhasil | Passed |
| Stok tidak mencukupi | Produksi ditolak | Passed |
| Pembelian bahan | Stok bertambah | Passed |

## Kesimpulan

Berdasarkan hasil Control Flow Testing, seluruh jalur kontrol dan percabangan pada sistem berhasil dieksekusi sesuai logika yang dirancang. Sistem mampu menangani berbagai kondisi input dan menghasilkan respon yang sesuai.
