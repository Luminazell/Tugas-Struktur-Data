Pengertian ADT Array Satu Dimensi

Meskipun bahasa pemrograman Python menyediakan struktur data list, kita tetap dapat mengimplementasikan konsep Abstract Data Type (ADT) Array untuk merepresentasikan sekumpulan elemen yang tersusun secara linier dengan ukuran tetap.

ADT Array satu dimensi memiliki sejumlah operasi dasar yang digunakan untuk mengelola elemen-elemen di dalamnya. Operasi-operasi tersebut meliputi:

1. Array(size)
Membentuk sebuah array dengan jumlah elemen sesuai nilai size.
Setiap elemen dalam array diinisialisasi dengan nilai None.
Nilai size harus lebih besar dari nol agar array dapat dibuat.

2. length()
Mengembalikan jumlah total elemen yang terdapat dalam array.

3. getitem(index)
Mengambil nilai yang tersimpan pada indeks tertentu menggunakan notasi tanda kurung siku [].

4. setitem(index, value)
Mengubah atau memperbarui nilai pada indeks tertentu dengan nilai baru yang diberikan.

5. clearing(value)
Mengatur seluruh elemen dalam array menjadi nilai tertentu sesuai dengan parameter value.

6. iterator()
Menyediakan mekanisme untuk mengakses atau menelusuri setiap elemen dalam array secara berurutan.

Simulasi Game of Life Menggunakan Array

Simulasi ini menggunakan array dua dimensi untuk merepresentasikan sebuah grid yang berisi sel-sel organisme. Setiap sel memiliki dua kemungkinan kondisi, yaitu hidup atau mati.

Konsep simulasi ini berasal dari Game of Life yang diperkenalkan oleh matematikawan Inggris, John Conway.

Array berfungsi sebagai struktur penyimpanan data untuk mengelola status setiap sel dalam grid. Perubahan dari satu generasi ke generasi berikutnya ditentukan berdasarkan jumlah tetangga hidup yang mengelilingi setiap sel.

Aturan Perkembangan Sel

Setiap sel dalam grid akan menentukan statusnya pada generasi berikutnya berdasarkan delapan tetangga di sekitarnya (vertikal, horizontal, dan diagonal).

1. Kelangsungan Hidup
Sel yang hidup akan tetap hidup apabila memiliki 2 atau 3 tetangga hidup.

2. Kematian karena Isolasi
Sel yang hidup akan mati jika memiliki kurang dari 2 tetangga hidup.

3. Kematian karena Overpopulasi
Sel yang hidup akan mati apabila memiliki lebih dari 3 tetangga hidup.

4. Kelahiran
Sel yang mati akan menjadi hidup jika memiliki tepat 3 tetangga hidup.

Implementasi Simulasi
1. Pengaturan Awal
Pengguna menentukan posisi awal sel-sel yang hidup di dalam grid. Kondisi awal ini akan menjadi generasi pertama dalam simulasi.

2. Iterasi Generasi
Program menerapkan aturan perkembangan sel secara serentak pada seluruh sel untuk menghasilkan generasi baru. Proses ini dilakukan berulang kali sesuai jumlah iterasi yang ditentukan.

3. Pengamatan Pola
Dari hasil simulasi, dapat diamati beberapa kemungkinan pola, antara lain:
Semua sel menjadi mati (kepunahan total)

Pola stabil (tidak mengalami perubahan pada generasi berikutnya)

Pola osilator yang berubah secara periodik
