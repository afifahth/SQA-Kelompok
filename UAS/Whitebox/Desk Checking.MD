# DESK CHECKING

## Definisi

Desk Checking merupakan salah satu metode White Box Testing yang dilakukan dengan memeriksa logika program secara manual tanpa menjalankan aplikasi secara langsung. Pengujian ini berfokus pada pemeriksaan alur program, penggunaan variabel, proses input, proses pengolahan data, serta output yang dihasilkan oleh sistem. Tujuan dari Desk Checking adalah untuk menemukan kesalahan logika sejak tahap awal pengembangan sehingga dapat mengurangi kemungkinan terjadinya kesalahan saat sistem dijalankan.

Pada Inventory Management System, Desk Checking digunakan untuk memeriksa logika program pada modul Login, Data Bahan, dan Transaksi yang merupakan fitur utama dalam sistem.

## Tujuan Pengujian

Pengujian Desk Checking dilakukan untuk memastikan bahwa setiap proses utama pada Inventory Management System telah dirancang dengan logika yang benar. Pemeriksaan difokuskan pada proses autentikasi pengguna, pengelolaan data bahan, serta transaksi yang memengaruhi jumlah stok dalam sistem.

Selain itu, pengujian ini bertujuan untuk memastikan bahwa data yang dimasukkan oleh pengguna dapat diproses dengan benar, menghasilkan output yang sesuai, serta tidak menimbulkan kesalahan yang dapat mengganggu operasional sistem.

---

## Modul Login

### Deskripsi Pengujian

Pengujian dilakukan untuk memastikan bahwa sistem dapat memvalidasi username dan password yang dimasukkan oleh pengguna sebelum memberikan akses ke dalam aplikasi.

| No | Skenario Pengujian | Hasil yang Diharapkan | Status |
|----|-------------------|----------------------|--------|
| 1 | Username dan password benar | Sistem menampilkan Dashboard | Passed |
| 2 | Username benar dan password salah | Sistem menampilkan pesan gagal login | Passed |
| 3 | Username dan password kosong | Sistem menolak proses login | Passed |

---

## Modul Data Bahan

### Deskripsi Pengujian

Pengujian dilakukan untuk memastikan bahwa proses pengelolaan data bahan dapat berjalan dengan baik mulai dari penambahan, perubahan, hingga penghapusan data.

| No | Skenario Pengujian | Hasil yang Diharapkan | Status |
|----|-------------------|----------------------|--------|
| 1 | Menambahkan data bahan baru | Data berhasil tersimpan | Passed |
| 2 | Mengubah data bahan | Data berhasil diperbarui | Passed |
| 3 | Menghapus data bahan | Data berhasil dihapus | Passed |

---

## Modul Transaksi

### Deskripsi Pengujian

Pengujian dilakukan untuk memastikan bahwa transaksi yang dilakukan pengguna dapat memengaruhi jumlah stok sesuai dengan aturan yang berlaku pada sistem.

| No | Skenario Pengujian | Hasil yang Diharapkan | Status |
|----|-------------------|----------------------|--------|
| 1 | Transaksi pembelian bahan | Stok bahan bertambah | Passed |
| 2 | Transaksi produksi | Stok bahan berkurang | Passed |
| 3 | Penyimpanan data transaksi | Data tersimpan pada database | Passed |

---

## Kesimpulan

Berdasarkan hasil Desk Checking yang telah dilakukan, seluruh logika program pada modul Login, Data Bahan, dan Transaksi telah berjalan sesuai dengan kebutuhan sistem. Setiap proses input, pengolahan data, dan output yang dihasilkan menunjukkan hasil yang sesuai dengan rancangan aplikasi.

Pengujian ini menunjukkan bahwa sistem mampu menangani proses autentikasi pengguna, pengelolaan data bahan, serta transaksi yang memengaruhi stok inventori dengan baik. Oleh karena itu, dapat disimpulkan bahwa logika dasar pada Inventory Management System telah memenuhi kebutuhan fungsional aplikasi dan siap untuk dilakukan pengujian pada tahap berikutnya.
