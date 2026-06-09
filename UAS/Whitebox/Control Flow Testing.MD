# Code Walkthrough

## Interface yang Diuji

Produksi

## Definisi

Code Walkthrough merupakan teknik White Box Testing yang dilakukan dengan meninjau source code secara langsung untuk memahami alur logika program, mengidentifikasi potensi kesalahan, serta memastikan bahwa setiap proses telah berjalan sesuai dengan kebutuhan sistem.

Pada Sistem Inventory Management, Code Walkthrough dilakukan pada fitur Produksi karena fitur ini merupakan proses utama yang menghubungkan data bahan baku, perhitungan biaya produksi, serta pembaruan stok produk dan bahan baku.

## Tujuan

1. Memastikan logika program pada proses produksi berjalan sesuai kebutuhan sistem.
2. Memastikan proses perhitungan kebutuhan bahan baku dilakukan dengan benar.
3. Memastikan validasi stok bahan baku berjalan sesuai aturan.
4. Memastikan data produksi tersimpan ke database dengan benar.
5. Memastikan pembaruan stok produk dan bahan baku dilakukan secara tepat.

## Tabel Pengujian

| No | Potongan Kode                                          | Deskripsi                                                                                                                                     |
| -- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| 1  | `$jumlah_dibutuhkan = $takaran * $jumlah_produksi;`    | Sistem menghitung jumlah bahan baku yang diperlukan berdasarkan takaran bahan dan jumlah produksi yang akan dibuat.                           |
| 2  | `if (!$b \|\| $b['stok'] < $jumlah_dibutuhkan)`        | Sistem memeriksa apakah stok bahan baku tersedia dan mencukupi kebutuhan produksi. Jika stok tidak mencukupi maka proses produksi dihentikan. |
| 3  | `$subtotal = $jumlah_dibutuhkan * $b['harga_satuan'];` | Sistem menghitung biaya bahan baku yang digunakan dalam proses produksi.                                                                      |
| 4  | `$total_hpp += $subtotal;`                             | Sistem menghitung total Harga Pokok Produksi (HPP) berdasarkan seluruh bahan baku yang digunakan.                                             |
| 5  | `INSERT INTO t_produksi`                               | Sistem menyimpan data transaksi produksi ke dalam database.                                                                                   |
| 6  | `UPDATE t_produk SET stok = stok + $jumlah_produksi`   | Sistem menambahkan stok produk jadi setelah proses produksi berhasil dilakukan.                                                               |
| 7  | `UPDATE t_bahan_baku SET stok = stok - $jumlah_bahan`  | Sistem mengurangi stok bahan baku sesuai jumlah yang telah digunakan selama proses produksi.                                                  |

## Analisis

Berdasarkan hasil peninjauan source code, proses produksi telah memiliki alur logika yang jelas mulai dari perhitungan kebutuhan bahan baku, validasi stok, perhitungan biaya produksi, penyimpanan data transaksi produksi, hingga pembaruan stok produk dan bahan baku. Setiap proses saling terhubung sehingga dapat mendukung jalannya proses produksi secara otomatis.

## Kesimpulan

Berdasarkan hasil Code Walkthrough yang telah dilakukan, logika program pada fitur Produksi telah berjalan sesuai dengan kebutuhan sistem. Sistem mampu menghitung kebutuhan bahan baku, memvalidasi stok, menyimpan data produksi, serta memperbarui stok produk dan bahan baku secara tepat sehingga proses produksi dapat berjalan dengan baik.
