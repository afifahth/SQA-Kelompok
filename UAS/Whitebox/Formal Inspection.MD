# FORMAL INSPECTION

## Definisi

Formal Inspection merupakan metode White Box Testing yang dilakukan secara sistematis untuk memeriksa kelengkapan, ketepatan, dan konsistensi data yang digunakan oleh sistem. Pengujian ini berfokus pada validasi data masukan dan keluaran agar sesuai dengan aturan yang telah ditentukan.

Pada Inventory Management System, Formal Inspection dilakukan untuk memastikan data yang diinput pengguna memenuhi ketentuan sistem sehingga dapat mengurangi kesalahan dan menjaga kualitas data.

## Tujuan Pengujian

Pengujian ini bertujuan untuk memastikan bahwa seluruh data yang diproses oleh sistem memiliki format yang benar, lengkap, dan sesuai dengan kebutuhan aplikasi. Selain itu, pengujian dilakukan untuk mencegah terjadinya kesalahan input yang dapat memengaruhi proses bisnis pada sistem inventori.

### Login

#### Deskripsi Pengujian
Pemeriksaan dilakukan terhadap kelengkapan data login yang dimasukkan pengguna.

| No | Pemeriksaan | Hasil |
|----|------------|--------|
| 1 | Username wajib diisi | Passed |
| 2 | Password wajib diisi | Passed |
| 3 | Format data sesuai | Passed |

### Data Bahan

#### Deskripsi Pengujian
Pemeriksaan dilakukan terhadap data bahan yang dimasukkan ke dalam sistem.

| No | Pemeriksaan | Hasil |
|----|------------|--------|
| 1 | Nama bahan wajib diisi | Passed |
| 2 | Stok berupa angka | Passed |
| 3 | Data tersimpan dengan benar | Passed |

### Transaksi

#### Deskripsi Pengujian
Pemeriksaan dilakukan terhadap data transaksi yang memengaruhi stok inventori.

| No | Pemeriksaan | Hasil |
|----|------------|--------|
| 1 | Jumlah transaksi wajib diisi | Passed |
| 2 | Data transaksi valid | Passed |
| 3 | Data tersimpan pada database | Passed |

## Kesimpulan

Berdasarkan hasil Formal Inspection, seluruh data yang digunakan dalam modul Login, Data Bahan, dan Transaksi telah memenuhi aturan validasi yang ditetapkan. Sistem mampu menangani data dengan baik sehingga risiko kesalahan input dapat diminimalkan.
