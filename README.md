# Analisis Penggunaan Bahan Bakar - Mohammad Rafdi
## Domain Proyek
Behan Bakar merupakan sebuah komponen utama dalam menggunaan kendaraan maka dari itu dalam projek ini penulis melakukan pemodelan ML dengan memprediksi beberapa variabel yang mempengaruhi jarak tempuh dan berapa banyak bahan bakar yang dibutuhkan untuk menempuh perjalanan

## Data Understanding
Dataset yang digunakan adalah [Bahan Bakar](http://buku.dioskurn.com/buku1/ch4/)

Dataset memiliki 7 kolom dan 65 baris
| Liter | Penumpang | Bagasi | Kecepatan | RPM  | Suhu | Kilometer |
|-------|-----------|--------|-----------|------|------|-----------|
| 20    | 1         | 0      | 42        | 3000 | 29   | 142       |
| 25    | 2         | 15     | 50        | 4000 | 36   | 177       |
| 20    | 4         | 10     | 50        | 3000 | 24   | 144       |
| 30    | 5         | 25     | 50        | 3000 | 18   | 203       |

Korelasi antara variabel dalam dataset

![maxx](https://user-images.githubusercontent.com/118952537/209936541-5ca0f240-d358-4419-b7ef-10326c8d6b70.png)

Niali dari gambar tersebut dapat dijelaskan bahwa semakin tua warna biru nya maka tidak saling berhubungan dan semakin tua warna merahnya maka semakin berhubungan

kemudian visualisasikan variabel dengan korelasi paling tinggi yaitu liter dan kilometer dan mendrop data yang tidak digunakan dan memiliki nilai korelasi negatif (-)
sehingga fitur yang digunakan adalah Liter,Kecepatan,Suhu sedangkan targenya merupakan Kilometer

![zzzaa](https://user-images.githubusercontent.com/118952537/209936880-81e174bd-49ad-4605-a525-e3e0df3f7c14.png)

## Modeling & Evaluasi
Pada tahap ini model yang digunakan adalah model Linear Regression dikarenakan pattern yang di dapat pada gambar diatas.
Score yang didapat menggunakan Linear Regression adalah 75%

## Kesimpulan
Banyaknya fitur akan mempengaruhi nilai akurasi dalam pemodelan Linear Regression ini semakin banyak fitur maka akurasi bisa berkurang semakin sedikit fitur akan membuat akurasi semakin akurat.
