# Data Flow Testing

## Interface yang Diuji

Data Bahan Baku → Produksi

## Definisi

Data Flow Testing merupakan teknik White Box Testing yang digunakan untuk memeriksa aliran data dalam sistem, mulai dari proses input, penyimpanan, pengolahan, hingga menghasilkan output. Pengujian ini bertujuan untuk memastikan bahwa data yang digunakan pada setiap proses mengalir dengan benar dan menghasilkan informasi yang sesuai.

Pada Sistem Inventory Management, Data Flow Testing dilakukan pada proses Data Bahan Baku dan Produksi karena kedua fitur tersebut saling berhubungan secara langsung dalam pengelolaan persediaan dan proses produksi.

## Tujuan

1. Memastikan data bahan baku tersimpan dengan benar ke dalam database.
2. Memastikan data bahan baku dapat digunakan pada proses produksi.
3. Memastikan data stok bahan baku digunakan sebagai dasar validasi produksi.
4. Memastikan data produksi tersimpan dengan benar setelah proses produksi berhasil dilakukan.
5. Memastikan pembaruan stok bahan baku berjalan sesuai jumlah bahan yang digunakan.

## Diagram Aliran Data

```text
Admin
  ↓
Input Data Bahan Baku
  ↓
Database Bahan Baku
  ↓
Proses Produksi
  ↓
Validasi Stok
  ↓
Update Stok Bahan
  ↓
Data Produksi
  ↓
Laporan Produksi
```

## Tabel Pengujian

| Komponen Data   | Sumber Data         | Proses                      | Output                  |
| --------------- | ------------------- | --------------------------- | ----------------------- |
| Nama Bahan      | Form Tambah Bahan   | Disimpan ke database        | Data bahan tersimpan    |
| Stok Bahan      | Database Bahan Baku | Validasi produksi           | Status stok tersedia    |
| Harga Satuan    | Database Bahan Baku | Perhitungan HPP             | Total biaya produksi    |
| Jumlah Produksi | Form Produksi       | Perhitungan kebutuhan bahan | Jumlah bahan digunakan  |
| Data Produksi   | Proses Produksi     | Penyimpanan transaksi       | Data produksi tersimpan |
| Stok Bahan      | Database Bahan Baku | Pengurangan stok            | Stok bahan diperbarui   |

## Analisis

Berdasarkan hasil pengujian, data yang berasal dari fitur Data Bahan Baku dapat digunakan dengan baik pada proses Produksi. Sistem mampu mengambil data stok dan harga bahan baku dari database, melakukan perhitungan kebutuhan bahan, menghitung biaya produksi, serta memperbarui data stok setelah produksi berhasil dilakukan.

Aliran data yang terjadi pada sistem berjalan secara berurutan mulai dari input data bahan baku hingga menghasilkan data produksi dan pembaruan stok yang sesuai.

## Kesimpulan

Berdasarkan hasil Data Flow Testing yang telah dilakukan, aliran data pada Sistem Inventory Management berjalan dengan baik. Data yang dimasukkan pada fitur Data Bahan Baku dapat digunakan secara langsung pada proses Produksi, menghasilkan transaksi produksi yang valid, serta memperbarui stok bahan baku sesuai kebutuhan produksi. Hal ini menunjukkan bahwa integrasi data antar fitur telah berjalan sesuai dengan kebutuhan sistem.
