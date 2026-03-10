Pemrograman Perangkat Bergerak 
Nama : Alif Nurrohman
Tugas 3 : Mereview Widget yang digunakan dalam main.dart 

Lihat Kode main.dart : [main.dart](https://github.com/alifnurrohmans/tugas3_ppb/blob/main/main.dart)

Alur Singkat Widget : 

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
