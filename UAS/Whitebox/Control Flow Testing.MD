# Control Flow Testing

## Interface yang Diuji

Produksi

## Definisi

Control Flow Testing merupakan teknik White Box Testing yang digunakan untuk menguji jalur eksekusi program berdasarkan percabangan dan pengambilan keputusan yang terdapat pada source code. Pengujian ini bertujuan untuk memastikan bahwa setiap kondisi menghasilkan alur proses yang sesuai dengan logika program yang telah dirancang.

Pada Sistem Inventory Management, Control Flow Testing dilakukan pada fitur Produksi karena fitur ini memiliki beberapa percabangan penting seperti pengecekan ketersediaan komposisi produk, validasi stok bahan baku, penyimpanan data produksi, serta pembaruan stok setelah proses produksi berhasil dilakukan.

## Tujuan

1. Memastikan seluruh jalur keputusan pada proses produksi berjalan sesuai logika program.
2. Memastikan sistem dapat mendeteksi kondisi ketika komposisi produk belum tersedia.
3. Memastikan sistem dapat mendeteksi kondisi stok bahan baku yang tidak mencukupi.
4. Memastikan sistem dapat melanjutkan proses produksi apabila seluruh persyaratan terpenuhi.
5. Memastikan sistem menghasilkan output yang sesuai pada setiap kondisi yang diuji.

## Diagram Alur

```text
Mulai
  ↓
Pilih Produk
  ↓
Input Jumlah Produksi
  ↓
Ambil Data Komposisi Produk
  ↓
Apakah Komposisi Produk Tersedia?
├── Tidak
│   ↓
│ Tampilkan Pesan:
│ "Komposisi produk belum diatur"
│   ↓
│ Selesai
│
└── Ya
    ↓
    Hitung Kebutuhan Bahan
    ↓
    Cek Stok Bahan
    ↓
    Apakah Stok Mencukupi?
    ├── Tidak
    │   ↓
    │ Redirect ke:
    │ form.php?error=stok_kurang
    │   ↓
    │ Selesai
    │
    └── Ya
        ↓
        Hitung Total HPP
        ↓
        Simpan Data Produksi
        ↓
        Simpan Detail Produksi
        ↓
        Update Stok Produk
        ↓
        Kurangi Stok Bahan
        ↓
        Redirect ke:
        │ ../dashboard.php?success=produksi
        ↓
        Selesai
```

## Tabel Pengujian

| Jalur | Kondisi                                            | Hasil yang Diharapkan                                                                                                                  | Status |
| ----- | -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| P1    | Komposisi produk tersedia dan stok bahan mencukupi | Sistem menghitung kebutuhan bahan, menyimpan data produksi, memperbarui stok, kemudian redirect ke `../dashboard.php?success=produksi` | Sesuai |
| P2    | Komposisi produk tidak tersedia                    | Sistem menampilkan pesan "Komposisi produk belum diatur" dan proses produksi dihentikan                                                | Sesuai |
| P3    | Stok bahan tidak mencukupi                         | Sistem redirect ke `form.php?error=stok_kurang` dan proses produksi dibatalkan                                                         | Sesuai |
| P4    | Data produksi berhasil disimpan                    | Sistem menyimpan detail produksi serta memperbarui stok produk dan bahan baku                                                          | Sesuai |

## Analisis

Berdasarkan hasil pengujian, seluruh jalur keputusan pada fitur Produksi telah berjalan sesuai dengan logika program yang dirancang. Sistem mampu membedakan kondisi ketika komposisi produk belum tersedia, stok bahan baku tidak mencukupi, maupun ketika seluruh persyaratan produksi terpenuhi. Setiap kondisi menghasilkan respons yang berbeda sesuai kebutuhan sistem sehingga proses produksi dapat berjalan dengan lebih aman dan terkontrol.

## Kesimpulan

Berdasarkan hasil Control Flow Testing yang telah dilakukan, seluruh percabangan dan jalur keputusan pada fitur Produksi telah berfungsi dengan baik. Sistem mampu melakukan validasi terhadap komposisi produk dan stok bahan baku sebelum produksi dilakukan, serta mampu menyimpan data produksi dan memperbarui stok secara otomatis ketika proses produksi berhasil dijalankan. Dengan demikian, alur kontrol pada fitur Produksi telah berjalan sesuai dengan kebutuhan Sistem Inventory Management.
