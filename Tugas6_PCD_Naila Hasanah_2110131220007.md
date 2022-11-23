# Nama : Naila Hasanah
# NIM  : 2110131220007
## Tugas 6 PCD : Image Enhancement Domain Spasial Dan Domain Frekuensi.

<br>
<br>



# Image Enhancement 

<p align = "justify">
Image enhancement adalah metode yang umum digunakan dalam meningkatkan kualitas citra. Perbaikan citra (image enhancement) bertujuan untuk mendapatkan tampilan citra dengan bentuk visualisasi yang lebih baik, dengan cara memaksimalkan kandungan informasi di dalam citra masukan.</p>

<p align = "justify">
Ruang lingkup dalam Peningkatan Citra atau Image Enhancement ada dua, yaitu: Spasial dan Frekuensi. Spasial mencakup semua teknik memanipulasi citra dalam domain spasial bidang citra. Sedangkan frekuensi memanipulasi citra dalam domain frekuensi dengan teknik transformasi Fourier.</p>

<p align="center">
    <img src="foto2/foto1_foto_5.png" >
</p>


# Spatial  Domain
<p align = "justify">
 Dalam metode domain frekuensi didasarkan pada Transformasi Fourier dari suatu gambar. Secara kasar, istilah frekuensi dalam sebuah gambar menceritakan tentang laju perubahan nilai piksel.</p>

<p align = "justify">
 Suatu citra dapat direpresentasikan dalam bentuk matriks 2D dimana setiap elemen matriks merepresentasikan intensitas piksel. Keadaan matriks 2D yang menggambarkan distribusi intensitas suatu gambar disebut Domain Spasial.</p>

<p align="center">
    <img src="foto2/3_foto_5.png" >
</p>

<p align = "justify">
Setiap intensitas piksel direpresentasikan sebagai f(x,y) di mana x,y adalah koordinat piksel dalam matriks 2D. Operasi yang berbeda dilakukan dalam nilai ini. Misalnya- operasi T(katakanlah, penambahan 5 ke semua piksel) dilakukan dalam f(x,y) yang berarti bahwa setiap nilai piksel bertambah 5. Ini dapat ditulis sebagai berikut :</p>

<p align="center">
    <img src="foto2/1_foto_5.png" >
</p>


g(x,y) = T[f(x,y)]

Keterangan :

f(x, y) = Citra original/citra input<br>
g(x, y) = Citra baru yang dimodifikasi/citra output<br>
T = Sebuah transformasi yang diterapkan untuk mendapatkan citra baru (g(x,y))<br>

<p align = "justify">
di mana, g(x,y) adalah intensitas baru setelah menambahkan 5 ke f(x,y).
Peningkatan Gambar Menggunakan Pemfilteran Domain Spasial
Istilah spasial, merujuk pada piksel yang merupakan elemen terkecil dari suatu citra. Semua perubahan langsung mengeksekusi nilai-nilai ini. Domain spasial dapat ditulis dalam notasi ini:</p>

<p align = "justify">
Dalam domain spasial, bentuk paling sederhana dari T berukuran 1×1. Dalam hal ini, g(x,y) hanya bergantung pada nilai f(x,y), dan T menjadi tingkat keabuan. Lingkungan yang lebih besar juga bisa ada. Mereka dikenal sebagai mask yang mungkin berbeda dalam implementasinya seperti filter, kernel, template atau windows .</p>

<p align = "justify">
Seperti yang dijelaskan, gambar skala abu-abu digunakan sebagai input ke algoritma. Gambar RGB (Merah Hijau Biru) diperoleh dalam tugas akuisisi. Gambar-gambar ini perlu diubah menjadi gambar skala abu-abu. Konversi citra input ke grayscale bertujuan untuk meminimalkan varians antar citra yang disebabkan oleh warna subjek yang berbeda. Jika algoritma dioptimalkan untuk warna tertentu, akan sangat sulit untuk bekerja dengan warna lain. Oleh karena itu dengan mengubah gambar RGB menjadi gambar grayscale, dimungkinkan untuk memiliki satu input format standar.</p>


# Domain Frekuensi
<p align = "justify">
Dalam metode domain frekuensi didasarkan pada Transformasi Fourier dari suatu gambar. Secara kasar, istilah frekuensi dalam sebuah gambar menceritakan tentang laju perubahan nilai piksel.</p>

<p align="center">
    <img src="foto2/4_foto_5.png" >
</p>

<p align = "justify">
Metode-metode image enhancement dalam ranah frekuensi dilakukan dengan mengubah citra terlebih dahulu dari ranah spasial ke ranah frekuensi, baru kemudian memanipulasi nilai-nilai frekuensi tersebut.</p>

Metode diantaranya ialah:

- Transformasi fourier
<p align = "justify">
Tranformasi fourier adalah suatu model transformasi yang memindahkan domain spasial atau domain waktu menjadi domain frekuensi. Dengan menggunakan transformasi fourier, sinyal atau citra dapat dilihat sebagai suatu objek dalam domain frekuensi. Analisis dalam domain frekuensi banyak digunakan seperti filtering.</p>


# Perbedaan antara domain spasial dan domain frekuensi

- Dalam domain spasial, berurusan dengan gambar apa adanya. Nilai piksel gambar berubah sehubungan dengan pemandangan.
- Sedangkan dalam domain frekuensi, berurusan dengan laju perubahan nilai piksel dalam domain spasial.

**Domain Spasial: Input -> Pemrosesan Gambar -> Output**

**Domain Frekuensi: Frekuensi + Distribusi -> Pemrosesan Gambar -> Transformasi Invers -> Keluaran**
