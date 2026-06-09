# Desk Checking

## Interface yang Diuji

Produksi

## Definisi

Desk Checking merupakan teknik White Box Testing yang dilakukan dengan memeriksa logika program secara manual tanpa menjalankan aplikasi secara langsung. Pengujian ini bertujuan untuk memastikan bahwa setiap proses perhitungan dan pengambilan keputusan pada program telah berjalan sesuai dengan algoritma yang dirancang.

Pada Sistem Inventory Management, Desk Checking dilakukan pada fitur Produksi karena fitur ini memiliki proses perhitungan kebutuhan bahan baku, pengecekan stok, serta pembaruan stok setelah proses produksi berhasil dilakukan.

## Tujuan

1. Memastikan sistem dapat menghitung kebutuhan bahan baku dengan benar.
2. Memastikan sistem dapat memvalidasi ketersediaan stok bahan baku sebelum produksi dilakukan.
3. Memastikan stok bahan baku berkurang sesuai jumlah yang digunakan.
4. Memastikan proses produksi gagal apabila stok bahan baku tidak mencukupi.
5. Memastikan logika produksi berjalan sesuai kebutuhan sistem.

## Tabel Pengujian

| Stok Awal | Jumlah Dibutuhkan | Stok Akhir  | Kondisi       | Hasil yang Diharapkan                        | Status |
| --------- | ----------------- | ----------- | ------------- | -------------------------------------------- | ------ |
| 100       | 20                | 80          | 100 - 20 = 80 | Produksi berhasil diproses                   | Sesuai |
| 50        | 20                | 30          | 50 - 20 = 30  | Produksi berhasil diproses                   | Sesuai |
| 15        | 20                | Tidak Valid | 15 < 20       | Produksi ditolak karena stok tidak mencukupi | Sesuai |

## Analisis

Berdasarkan hasil pengujian, sistem mampu melakukan perhitungan kebutuhan bahan baku sesuai jumlah produksi yang dimasukkan pengguna. Sistem juga berhasil melakukan validasi stok sebelum proses produksi dijalankan. Ketika stok bahan baku mencukupi, proses produksi dapat dilanjutkan dan stok bahan akan dikurangi sesuai kebutuhan. Sebaliknya, apabila stok tidak mencukupi, sistem secara otomatis menolak proses produksi dan menampilkan pesan kesalahan.

## Kesimpulan

Berdasarkan hasil Desk Checking yang telah dilakukan, logika program pada fitur Produksi telah berjalan sesuai dengan kebutuhan sistem. Sistem mampu menghitung kebutuhan bahan baku, melakukan validasi stok, dan memperbarui data stok secara tepat sehingga dapat meminimalkan kesalahan dalam proses produksi.
