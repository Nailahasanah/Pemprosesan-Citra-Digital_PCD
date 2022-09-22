# Nama : Naila Hasanah
# NIM  : 2110131220007

# Tugas 2 Pemprosesan Citra Digital

<br>

# Eksplorasi Octave dengan Package Image
<br>

Langkah pertama adalah dengan membuat package image terlebih dahulu.Ketik **pkg load image** pada command windows.Jika ingin mengecek pack image apakah sudah ada atau belum bisa dengan mengetik **pkg list**.


### Berikut contoh Eksplorasi Octave dengan Package Image :

## 1.Gambar Asli dan Histogram
<p align="center">
    <img src="foto/gambar_asli.png" >
</p>

<p align="center">
    <img src="foto/histogram_ori.png" >
</p>

## 2.Gambar Read dan Histogram
<p align="center">
    <img src="foto/merah.png" >
</p>

<p align="center">
    <img src="foto/histogram_merah.png" >
</p>

## 3.Gambar Green dan Histogram

<p align="center">
    <img src="foto/hijau.png" >
</p>

<p align="center">
    <img src="foto/histogram_hijau.png" >
</p>

## 4.Gambar Blue dan Histogram
<p align="center">
    <img src="foto/biru.png" >
</p>

<p align="center">
    <img src="foto/histogram_biru.png" >
</p>

<br>

### Dari hasil tersebut dapat disimpulkan bahwa Gambar terbagi menjadi 3 layer yaitu *merah(read)*,*hijau(green)* dan *biru(blue)*.

<br>

# Kode Editor untuk membuat  Package Image

<p align="center">
    <img src="foto/kode_tugas2_pcd.png" >
</p>



<br>

## Fungsi Kode

- Imread (images read) digunakan untuk membaca citra menjadi sebuah data matriks.
- Imshow (images show) digunakan untuk menampilkan data matriks menjadi sebuah gamba
- Imhist Adalah suatu perintah yang berfungsi untuk menampilkan suatu histogram dari sebuah citra.Histogram adalah tampilan grafis dari tabulasi frekuensi yang digambarkan dengan grafis batangan manifestasi data benning.