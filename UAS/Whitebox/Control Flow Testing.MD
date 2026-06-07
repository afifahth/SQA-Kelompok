# DATA FLOW TESTING

## Definisi

Data Flow Testing merupakan metode White Box Testing yang berfokus pada pemeriksaan aliran data dalam sistem, mulai dari proses input, pengolahan, penyimpanan, hingga menghasilkan output. Pengujian ini dilakukan untuk memastikan bahwa data diproses dengan benar dan tidak terjadi kehilangan atau kesalahan data selama proses berlangsung.

Pada Inventory Management System, Data Flow Testing dilakukan pada modul Login, Data Bahan, dan Transaksi karena ketiga modul tersebut memiliki aliran data yang penting dalam operasional sistem.

## Tujuan Pengujian

Pengujian ini bertujuan untuk memastikan bahwa data yang dimasukkan pengguna dapat diproses dengan benar oleh sistem, tersimpan pada database, dan menghasilkan output yang sesuai dengan kebutuhan aplikasi.

### Login

#### Deskripsi Pengujian
Pengujian dilakukan untuk memastikan data login dapat diproses dengan benar hingga menghasilkan akses ke sistem.

| Input | Proses | Output | Status |
|---------|---------|---------|---------|
| Username dan Password | Validasi akun | Dashboard tampil | Passed |

### Data Bahan

#### Deskripsi Pengujian
Pengujian dilakukan untuk memastikan data bahan dapat tersimpan dan ditampilkan kembali dengan benar.

| Input | Proses | Output | Status |
|---------|---------|---------|---------|
| Data bahan | Simpan ke database | Data tampil pada tabel | Passed |
| Perubahan data bahan | Update database | Data diperbarui | Passed |

### Transaksi

#### Deskripsi Pengujian
Pengujian dilakukan terhadap aliran data transaksi yang memengaruhi stok inventori.

| Input | Proses | Output | Status |
|---------|---------|---------|---------|
| Pembelian bahan | Update stok | Stok bertambah | Passed |
| Produksi | Kurangi stok | Stok berkurang | Passed |
| Data transaksi | Simpan database | Riwayat transaksi tersimpan | Passed |

## Kesimpulan

Berdasarkan hasil Data Flow Testing, seluruh aliran data pada modul Login, Data Bahan, dan Transaksi berjalan dengan baik. Data berhasil diproses mulai dari tahap input, pengolahan, penyimpanan, hingga menghasilkan output yang sesuai dengan kebutuhan sistem.
