# Formal Inspection

## Interface yang Diuji

Data Bahan Baku

## Definisi

Formal Inspection merupakan teknik White Box Testing yang dilakukan dengan memeriksa struktur program, validasi data, dan kelengkapan proses secara sistematis. Pengujian ini bertujuan untuk memastikan bahwa data yang dimasukkan ke dalam sistem telah memenuhi persyaratan yang ditentukan sebelum diproses atau disimpan ke dalam database.

Pada Sistem Inventory Management, Formal Inspection dilakukan pada fitur Data Bahan Baku karena fitur ini merupakan sumber utama data yang digunakan dalam proses produksi dan pengelolaan persediaan.

## Tujuan

1. Memastikan seluruh field input bahan baku tersedia dan dapat digunakan.
2. Memastikan sistem melakukan validasi terhadap data yang wajib diisi.
3. Memastikan data bahan baku dapat disimpan dengan benar ke dalam database.
4. Memastikan data yang tersimpan dapat digunakan pada proses produksi.
5. Memastikan kualitas data yang tersimpan tetap terjaga.

## Tabel Pengujian

| Skenario           | Data Masukan              | Hasil yang Diharapkan           | Status |
| ------------------ | ------------------------- | ------------------------------- | ------ |
| Semua field terisi | Nama, Satuan, Stok, Harga | Data berhasil disimpan          | Sesuai |
| Nama bahan kosong  | Nama tidak diisi          | Sistem menolak penyimpanan data | Sesuai |
| Stok kosong        | Stok tidak diisi          | Sistem menolak penyimpanan data | Sesuai |
| Harga kosong       | Harga tidak diisi         | Sistem menolak penyimpanan data | Sesuai |


## Analisis

Berdasarkan hasil pemeriksaan, seluruh field yang diperlukan pada form bahan baku telah tersedia dan dapat menerima input pengguna dengan baik. Sistem juga menerapkan validasi pada field yang wajib diisi sehingga data yang tidak lengkap tidak dapat disimpan ke database. Dengan adanya validasi tersebut, risiko terjadinya kesalahan data dapat diminimalkan dan kualitas informasi yang tersimpan menjadi lebih baik.

## Kesimpulan

Berdasarkan hasil Formal Inspection yang telah dilakukan, fitur Data Bahan Baku telah memiliki mekanisme validasi yang memadai. Sistem mampu memastikan bahwa hanya data yang lengkap dan valid yang dapat disimpan ke dalam database sehingga mendukung kelancaran proses produksi dan pengelolaan persediaan.
