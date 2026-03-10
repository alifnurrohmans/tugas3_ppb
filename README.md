## Pemrograman Perangkat Bergerak 
## Nama : Alif Nurrohman
## Tugas 3 : Mereview Widget yang digunakan dalam main.dart 

Lihat Kode main.dart : [main.dart](https://github.com/alifnurrohmans/tugas3_ppb/blob/main/main.dart)

## 1. Alur Singkat Widget : 

```
MyApp (Stateless)
└── MaterialApp (Theme & Home)
    └── RowColumnPage (Stateless)
        └── Scaffold
            ├── AppBar (Title: "My First App", Color: Orange)
            └── Column (Body Utama - MainAxisAlignment.center)
                ├── [1] Container (Wrapper Gambar - Light Blue)
                │       └── AspectRatio (1.0)
                │           └── Center ── Image.network (Picsum)
                ├── [2] Container (Label Box - Pink)
                │       └── Text ("What image is that")
                ├── [3] Container (Category Box - Yellow)
                │       └── Row (MainAxisAlignment.spaceEvenly)
                │           ├── Column (Food) ── [Icon, Text]
                │           ├── Column (Scenery) ── [Icon, Text]
                │           └── Column (People) ── [Icon, Text]
                └── [4] CounterCard (StatefulWidget - Cyan)
                        └── Row (MainAxisAlignment.spaceBetween)
                            ├── Text ("Counter here: $_counter")
                            └── IconButton (Action: _incrementCounter)
```

## 2. Detail Komponen Widget

Berikut adalah rincian peran dan properti kunci dari setiap widget yang digunakan dalam aplikasi:

* **MaterialApp (Top-level)**: Mengatur tema global (`useMaterial3: true`), skema warna dari *seed color*, dan menentukan halaman utama.
* **Scaffold (Layout)**: Menyediakan struktur dasar halaman dengan slot khusus untuk `appBar` dan `body`.
* **Column (Multi-child)**: Menyusun widget secara **vertikal**. Menggunakan `mainAxisAlignment: center` untuk memposisikan konten di tengah layar secara vertikal.
* **Row (Multi-child)**: Menyusun widget secara **horizontal**. Digunakan pada baris ikon kategori dan baris interaksi counter.
* **Container (Styling)**: Widget dekoratif untuk mengatur **Margin**, **Padding**, dan **Warna** latar belakang (seperti warna pink, kuning, dan biru).
* **AspectRatio (Sizing)**: Memaksa widget anaknya (gambar) tetap memiliki rasio dimensi yang konsisten (Rasio 1:1 untuk bentuk persegi).
* **MediaQuery (Utility)**: Mengambil data fisik layar (`width` & `height`) secara dinamis agar tampilan bersifat *responsive* di berbagai ukuran HP.
* **StatefulWidget (Logic)**: Digunakan pada `CounterCard` sebagai satu-satunya komponen yang memiliki data dinamis (`_counter`) yang bisa berubah-ubah saat aplikasi berjalan.
