# CODE WALKTHROUGH

## Definisi

Code Walkthrough merupakan metode White Box Testing yang dilakukan dengan cara meninjau dan mendiskusikan source code secara bersama-sama untuk memahami alur logika program. Pengujian ini bertujuan untuk menemukan potensi kesalahan logika, meningkatkan kualitas kode, serta memastikan bahwa setiap fungsi telah dikembangkan sesuai dengan kebutuhan sistem.

Pada Inventory Management System, Code Walkthrough dilakukan terhadap modul Login, Data Bahan, dan Transaksi karena ketiga modul tersebut merupakan fungsi utama yang mendukung operasional sistem.

## Tujuan Pengujian

Pengujian ini bertujuan untuk memastikan bahwa struktur program mudah dipahami, logika yang digunakan sesuai dengan kebutuhan sistem, dan setiap fungsi yang dibuat dapat berjalan dengan baik. Selain itu, Code Walkthrough juga bertujuan untuk mengidentifikasi kemungkinan kesalahan sejak tahap pengembangan sehingga dapat diperbaiki sebelum sistem digunakan.

### Login

#### Deskripsi Pengujian
Peninjauan dilakukan terhadap proses validasi username dan password yang digunakan untuk memberikan hak akses kepada pengguna.

| Bagian Kode | Hasil Pemeriksaan |
|------------|------------------|
| Validasi Username | Berjalan dengan baik |
| Validasi Password | Berjalan dengan baik |
| Redirect Dashboard | Berjalan dengan baik |

### Data Bahan

#### Deskripsi Pengujian
Peninjauan dilakukan terhadap proses pengelolaan data bahan mulai dari tambah, ubah, dan hapus data.

| Bagian Kode | Hasil Pemeriksaan |
|------------|------------------|
| Tambah Data | Berjalan dengan baik |
| Edit Data | Berjalan dengan baik |
| Hapus Data | Berjalan dengan baik |

### Transaksi

#### Deskripsi Pengujian
Peninjauan dilakukan terhadap proses transaksi yang memengaruhi perubahan stok dalam sistem.

| Bagian Kode | Hasil Pemeriksaan |
|------------|------------------|
| Penyimpanan Data Transaksi | Berjalan dengan baik |
| Penambahan Stok Pembelian | Berjalan dengan baik |
| Pengurangan Stok Produksi | Berjalan dengan baik |

## Kesimpulan

Berdasarkan hasil Code Walkthrough yang telah dilakukan, struktur program pada modul Login, Data Bahan, dan Transaksi dapat dipahami dengan baik serta telah sesuai dengan kebutuhan sistem. Tidak ditemukan kesalahan logika yang dapat menghambat fungsi utama aplikasi.
