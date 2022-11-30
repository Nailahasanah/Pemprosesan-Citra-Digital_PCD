<h1 align="center"><b>TUGAS 7</b></h2>

<h1 align="center"><b>Pemrosesan Citra Digital</b></h2>

### __KELOMPOK 10 :__
- Khoyrur Roykhan
- Delphia Aryana
- Naila Hasanah
<hr>
<br>

### __LOW-PASS FILTERING & HIGH-PASS FILTERING__

<br>

### __1. Low-Pass Filtering__

<p align="justify">&ensp;&ensp;&ensp;&ensp;Low-pass filtering adalah proses filter yang melewatkan komponen citra dengan nilai intensitas yang rendah dan meredam komponen citra dengan nilai intensitas yang tinggi. Low pass filter akan menyebabkan citra menjadi lebih halus dan lebih blur.</p>

__Aturan kernel untuk low-pass filter adalah:__
1. Semua koefisien kernel harus positif
2. Jumlah semua koefisien kernel harus sama dengan 1

Contoh kernel  yang dapat digunakan pada low-pass filtering adalah

<p align="center"><img width="700" src="img/kernel low pass.jpg"></p>

Low-pass filtering menggunakan kernel (iii) disebut juga neighborhood averaging. 

### - __Low Pass Filtering Menggunakan Octave__

<p align="center"><img width="700" src="img/kode.png"></p>

Hasil :

- Citra Asli
<p align="center"><img width="500" src="img/figure1.png"></p>

- Citra Menggunakan Kernel 1
<p align="center"><img width="500" src="img/figure2.png"></p>

- Citra Menggunakan Kernel 2
<p align="center"><img width="500" src="img/figure3.png"></p>

- Citra Menggunakan Kernel 3
<p align="center"><img width="500" src="img/figure4.png"></p>

### __2. High-Pass Filtering__

<p align="justify">&ensp;&ensp;&ensp;&ensp; <i>High Pass Filter</i> (HPF) adalah proses filter yang mengambil citra dengan gradiasi intensitas yang tinggi dan perbedaan intensitas yang rendah akan dikurangi atau dibuang. <i>High Pass Filtering</i> adalah salah satu dari metode penajaman <i>(sharpening).</i> 

<p align="justify">&ensp;&ensp;&ensp;&ensp; Tujuan utama dari proses penajaman ini adalah untuk menyoroti detail-detail halus dalam gambar atau untuk meningkatkan detail yang telah dikaburkan baik dalam kesalahan atau efek alami dari proses akuisisi citra tertentu.

### __Kegunaan__

- __High-Pass Filter__ sering disebut juga sebagai filter penajaman tepi __(edge sharpening)__ karena HPF digunakan dalam proses penajaman citra. 
- Operasi penajaman citra bertujuan untuk memperjelas tepi pada objek di dalam citra atau menghilangkan bagian citra yang lembut.
- Karena penajaman citra lebih berpengaruh pada tepi __(edge)__ objek, maka penajaman citra sering disebut juga penajaman tepi __(edge sharpening)__ atau peningkatan kualitas tepi __(edge enhancement)__.

### __Aturan-Aturan Dalam High-Pass Filter__

1. Koefisien penapis boleh negatif, nol, ataupun bernillai positif.
2. Total keseluruhan koefisiennya ialah bernilai 0 ataupun 1.
3. Apabila jumlah koefisiennya berjumlah = 0, maka setiap elemen yang rendah frekuensinya nilainya akan menurun. 
4. Namun, apabila total dari koefisien adalah = 1, maka elemen yang memiliki frekuensi rendah nilainya tetap sama dengan nilai semula.

### - __High Pass Filtering Menggunakan Octave__

<p align="center"><img width="500" src="img/kode_highpass.png"></p>

Output :

<p align="center"><img width="500" src="img/output_highpass.png"></p>