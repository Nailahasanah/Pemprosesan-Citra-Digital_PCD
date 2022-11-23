# Nama : Naila Hasanah
# NIM  : 2110131220007
##  Tugas 4 PCD : Algoritma Patterning,Dithering, Bit Plane Slicing, Dan Histogram Equalization

<br>
<br>

# 1). Patterning

Patterning adalah sebuah metode halftoning yang memanfaatkan pola-pola tertentu
untuk menyusun sebuah citra.

## Algoritma :

pola 0 = [0 0 0;0 0 0;0 0 0];

pola 1 = [0 0 0;0 0 0;0 0 1];

pola 2 = [1 0 0;0 0 0;0 0 1];

pola 3 = [1 0 1;0 0 0;0 0 1];

pola 4 = [1 0 1;0 0 0;1 0 1];

pola 5 = [1 0 1;0 0 0;1 1 1];

pola 6 = [1 0 1;1 0 0;1 1 1];

pola 7  = [1 1 1;1 0 0;1 1 1];

pola 8 = [1 1 1;1 0 1;1 1 1];

pola 9 = [1 1 1;1 1 1;1 1 1];

gambar = [ ]

## Pseudocode :

for x (x = 1; x < gambar.length; x++){

            for (y = 1; y < gambar.length; y++){

                    if (gambar [x, y] >= 0 and gambar [x, y] <= 25):

                            gambar[x, y] = pola0

                    elif (gambar [x, y] >= 26 and gambar [x,y] <= 51):

                            gambar [x, y] = pola1

                    elif (gambar [x, y] >= 52 and gambar [x, y] <= 77):

                            gambar[x, y] = pola2

                    elif (gambar [x, y] >= 78 and gambar [x, y] <= 103):

                            gambar [x, y] = pola3

                    elif (gambar [x, y] >= 104 and gambar [x, y] <= 129):

                            gambar [x, y] = pola4

                    elif (gambar [x, y] >= 130 and gambar [x, y] <= 155):

                            gambar [x, y] = pola5

                    elif (gambar [x, y] >= 156 and gambar [x, y] <= 181):

                            gambar[x,y] = pola6

                    elif (gambar [x, y] >= 182 and gambar [x, y] <= 207):

                            gambar [x, y] = pola7

                    elif (gambar [x, y] >= 208 and gambar [x, y] <= 233):

                            gambar [x, y] = pola8

                    elif (gambar [x, y] >= 234 and gambar [x, y] <= 259):

                            gambar [x, y] = pola9

           }

    }

<br>


# 2). Dithering
- Dithering merupakan salah satu metode dalam halftoning yang memanfaatkan sebuah
matriks dithering yang dijadikan sebagai sebuah threshold.
- Matriks citra dibandingkan dengan matriks dither, proses ini disebut sebagai
thresholding.

## Algoritma Dithering :

d1 = [
	0 128;
	192 64
];

M = [
	0 128 32 160;
	192 64 224 96;
	48 176 16 144;
	240 112 208 80
];

##  Berikut Cara menentukan Pola Dithering :
- Menentukan matriks dan treshold.
- Membandingkan nilai setiap elemen matriks dengan nilai setiap elemen treshold.
- Jika nilai elemen matriks lebih besar dari nilai elemen treshold maka piksel berwarna hitam atau bernilai 0.
- Sebaliknya jika nilai elemen matriks lebih kecil dari nilai elemen treshold maka piksel berwarna putih atau bernilai 1.

# 3). Bit Plane Slicing

<p align = "justify">
Bit-plane slicing merupakan metode yang digunakan untuk melihat
konstribusi atau pengaruh tiap bit penyusun citra.
Untuk citra 8 bit, pada dasarnya tiap intensitas yang nilainya dalam format
decimal, bisa dipecah menjadi bit-bit dalam format biner. Misalnya, sebuah
pixel dengan intensitas 245 (decimal) bila dijadikan biner adalah 11110101.</p>

# Algoritma :
- Mengubah nilai setiap elemen matriks menjadi biner.
- Simpan nilai biner dari nilai setiap elemen matriks.
- Setiap 1 angka pada matriks disimpan lagi kedalam matriks baru sehingga menjadi 8 buah matriks baru dari bilangan biner tersebut.
- Bilangan biner yang berada disisi paling kanan adalah last significant bit.
- Sedangkan bilangan biner yang berada disisi paling kiri adalah most significant bit.

# 4). Histogram equalization

<p align = "justify">
- Histogram equalization merupakan suatu operasi Image
Enhancement (peningkatan kualitas citra) yang bertujuan untuk
memperoleh histogram yang intensitasnya terdistribusi secara
seragam pada citra.</p>
<p align = "justify">
-  Efeknya dapat digunakan untuk meningkatkan kontras secara
menyeluruh. Dengan demikian, citra yang memiliki histogram yang tidak merata
akan menjadi citra yang lebih jelas karena derajat keabuannya
tidak dominan gelap atau dominan terang.</p>

## Algoritma Histogram Equalization :

- Ambil nilai maksimal intensitas piksel pada citra yang ingin
diterapkan histogram equalization.
- Hitung frekuensi untuk tiap nilai intensitas piksel pada citra.
- Hitung frekuensi kumulatif berdasarkan frekuensi tiap nilai
intensitas piksel pada citra.
- Normalisasi nilai intensitas piksel dengan membagi nilai frekuensi
kumulatifnya dengan total semua nilai intensitas piksel pada citra.
- Nilai piksel yang baru didapatkan dengan mengalikan hasil
normalisasi dengan nilai maksimal intensitas piksel pada citra.
- Untuk setiap nilai awal pada citra, ubah dengan nilai baru.
