# 1.1. BACKGROUND CONTEXT

Sebuah supermarket melihat adanya peluang untuk meningkatkan pendapatan dari bisnis mereka dalam era digitalisasi. Dengan memanfaatkan data pelanggan yang telah dikumpulkan selama 2 tahun terakhir, supermarket mencoba untuk menganalisa pola perilaku pelanggan dengan harapan dapat menemukan cara untuk meningkatkan pendapatan mereka di tahun-tahun berikutnya.

## 1.2. STAKEHOLDER

Analisa yang dilakukan ditujukan kepada seluruh pihak yang terlibat dalam aktivitas bisnis supermarket, di mana setiap pihak diharapkan dapat mengambil informasi dan manfaat dari hasil analisa ini. Adapun secara spesifik analisa ini dikhususkan untuk tim **Business Development** dari supermarket.

## 1.3. PROBLEM STATEMENT

**Pertanyaan bisnis utama:** <br>

`1. Bagaimana Supermarket meningkatkan pendapatannya berdasarkan pola perilaku pelanggan selama 2 tahun terkahir?`

**Pertanyaan riset berdasarkan data:**<br>

`1. Bagaimana karakteristik pelanggan potensial Supermarket?`<br>
    1.1 Bagaimana segmentasi pelanggan potensial untuk dijadikan target dalam meningkatkan penjualan?<br>
    1.2 Bagaimana profil pelanggan potensial untuk dijadikan target dalam meningkatkan penjualan?<br>

`2. Bagaimana Supermarket mengoptimalkan penjualan pada segmen pelanggan potensial?`<br>
    2.1 Apa produk yang tepat untuk diatawarkan pada segmen pelanggan potensial?<br>
    2.2 Apa media yang cocok untuk melayani segmen pelanggan potensial?<br>
    2.3 Bagaimana strategi marketing yang tepat untuk segmen pelanggan potensial?<br>

    ## 1.4. GOALS

Tujuan utama dari analisa ini yaitu untuk meningkatkan pendapatan Supermarket berdasarkan pola perilaku pelanggan selama 2 tahun terakhir dengan memahami karakteristik dari pelanggan potensial guna menaikkan tingkat konversi segmen pelanggan potensial

## 1.5. DATA UNDERSTANDING

`Sumber Data`

Dataset yang digunakan berjudul "Supermarket Customer" dengan format .csv (Comma-Seperated Values). Diberikan oleh Tim Akademik Purwadhika Data Science Class yang dapat diakses melalui link:

https://drive.google.com/drive/folders/1WodnBbuYTvsF0-6HTuQABQ0KCS31lqbK

Dataset berisikan profil pelanggan termasuk demografi, riwayat pembelian, dan riwayat pemasaran. Terdiri dari 29 kolom yang dibagi ke dalam 4 kategori dengan detail sebagai berikut:


| Kolom               | Deskripsi                                             |
|---------------------|-------------------------------------------------------|
| ID                  | Nomor ID unik pelanggan                           |
| Year_Birth          | Tahun kelahiran pelanggan                             |
| Education           | Tingkat pendidikan pelanggan                          |
| Marital_Status      | Status pernikahan pelanggan                           |
| Income              | Pendapatan tahunan rumah tangga pelanggan            |
| Kidhome             | Jumlah anak di rumah tangga pelanggan                |
| Teenhome            | Jumlah remaja di rumah tangga pelanggan              |
| Dt_Customer         | Tanggal pendaftaran pelanggan dengan perusahaan       |
| Recency             | Jumlah hari sejak pembelian terakhir pelanggan       |
| Complain            | Status aktivitas komplain pelanggan dalam 2 tahun terakhir (Y/N) |
| MntWines            | Jumlah pembelian anggur pelanggan dalam 2 tahun terakhir |
| MntFruits           | Jumlah pembelian buah pelanggan dalam 2 tahun terakhir |
| MntMeatProducts     | Jumlah pembelian daging pelanggan dalam 2 tahun terakhir |
| MntFishProducts     | Jumlah pembelian ikan pelanggan dalam 2 tahun terakhir |
| MntSweetProducts    | Jumlah pembelian permen pelanggan dalam 2 tahun terakhir |
| MntGoldProds        | Jumlah pembelian emas pelanggan dalam 2 tahun terakhir |
| NumDealsPurchases   | Jumlah pembelian dengan diskon                       |
| AcceptedCmp1        | 1 jika pelanggan menerima tawaran dalam kampanye pertama, 0 sebaliknya |
| AcceptedCmp2        | 1 jika pelanggan menerima tawaran dalam kampanye kedua, 0 sebaliknya |
| AcceptedCmp3        | 1 jika pelanggan menerima tawaran dalam kampanye ketiga, 0 sebaliknya |
| AcceptedCmp4        | 1 jika pelanggan menerima tawaran dalam kampanye keempat, 0 sebaliknya |
| AcceptedCmp5        | 1 jika pelanggan menerima tawaran dalam kampanye kelima, 0 sebaliknya |
| Response            | 1 jika pelanggan menerima tawaran dalam kampanye terakhir, 0 sebaliknya |
| NumWebPurchases     | Jumlah pembelian melalui situs web perusahaan        |
| NumCatalogPurchases | Jumlah pembelian menggunakan katalog                 |
| NumStorePurchases   | Jumlah pembelian langsung di toko                   |
| NumWebVisitsMonth   | Jumlah kunjungan ke website perusahaan dalam bulan terakhir |

## KARAKTERISTIK PELANGGAN POTENSIAL

**SEGMENTASI PELANGGAN POTENSIAL UNTUK DIJADIKAN TARGET DALAM MENINGKATKAN PENJUALAN** <br>

   Berdasarkan analisis segmentasi pelanggan dengan metode RFM di supermarket, terdapat tiga segmen pelanggan, diantaranya:

1. `Segmen 1` <br>
Terdiri dari pelanggan dengan nilai monetary yang tinggi, menunjukkan kecenderungan mereka untuk melakukan transaksi dengan nominal besar. <br>

2. `Segmen 2` <br>
Teridiri dari pelanggan dengan nilai frequency dan/atau recency yang tinggi, yaitu pelanggan yang sering melakukan transaksi dan/atau baru saja melakukan transaksi.<br>

3. `Segmen 3` <br>
Teridiri dari pelanggan dengan nilai recency, frequency, dan monetary yang rendah, menunjukkan bahwa mereka jarang bertransaksi, sudah lama tidak melakukan transaksi, dan nilai transaksinya kecil. <br>

Dengan demikian, dapat ditentukan bahwa `Segmen 1 merupakan segmen pelanggan potensial`. Direkomendasikan bahwa segmen ini dijadikan prioritas utama atau target untuk meningkatkan penjualan. (diperpanjang)

**PROFIL PELANGGAN POTENSIAL UNTUK DIJADIKAN TARGET DALAM MENINGKATKAN PENJUALAN**

Terdapat 4 profil demografi yang tepat untuk dihighlight dalam melihat profil dari segmen pelanggan potensial, yaitu usia, tingkat pendidikan, jumlah anak, dan jumlah pendapatan. Profil demografi tersebut memiliki tren atau kecenderungannya masing-masing dalam mencirikan setiap segmen, terutama segmen pelanggan potensial, sehingga dapat dibedakan dengan jelas, profil demografi dari segmen pelanggan potensial. 

Berdasarkan analisis profil demografi pelanggan, didapat kesimpulan sebagai berikut:

| Profil Demografi       |           Segmen 1                                                                                                  |           Segmen 2                                                                                          |           Segmen 3                                                                                       |
|:-------------------:|:----------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------:|
| Kelompok Usia       | Berumur lebih tua (Proporsi pelanggan berusia 50-65 tahun relatif tinggi)                                                                  | Berumur lebih muda (Proporsi pelanggan berusia 50-65 tahun relatif rendah)                                                                             | Berumur lebih muda (Proporsi pelanggan berusia 50-65 tahun relatif rendah)                                                                          |
| Tingkat Pendidikan  | Proporsi tingkat pendidikan doktoral menyerupai pendidikan magister, dan hampir tidak ada yang tamatan SMA | Proporsi tingkat pendidikan doktoral rendah dan masih terdapat sebagian kecil yang tamatan SMA     | Proporsi tingkat pendidikan doktoral rendah dan masih terdapat sebagian kecil yang tamatan SMA |
| Jumlah Anak         | 50% pelanggan tidak memiliki anak                                                                    | 50% pelanggan memiliki seorang anak                                                           | 50% pelanggan memiliki seorang anak                                                       |
| Pendapatan          | Dominasi kelas menengah, dan terdapat proporsi yang cukup signifikan dari pelanggan kelas menengah atas   | Dominasi kelas menengah ke bawah, hampir tidak ada kelas menengah ke atas                         | Dominasi kelas menengah ke bawah, tidak ada dari kelas menengah ke atas                        |



Dilihat dari profil demografinya, pelanggan Segmen 1 memiliki profil yang mendukung sebagai segmen pelanggan yang disebut potensial. Pelanggan pada segmen ini terdiri dari individu dengan rata-rata usia yang relatif lebih lebih tua, tingkat pendidikan yang lebih tinggi, tidak memiliki tanggungan anak, dan mayoritas pendapatan berada di kelas menengah hingga menengah ke atas.


