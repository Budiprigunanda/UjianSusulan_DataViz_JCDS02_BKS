![purwadhika logo](https://static.wixstatic.com/media/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png/v1/fill/w_246,h_39,al_c,usm_0.66_1.00_0.01/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png)

Selamat datang di Ujian Susulan Modul 2, JCDS Bekasi.
Pada ujian kali ini, Anda akan menggunakan data dari database Distributor Diecast Hot Wheels. Database ini terbagi menjadi 8 (delapan) tables, antara lain:
1. customers
2. employees
3. offices
4. orderdetails
5. orders
6. payments
7. productlines
8. products

Ujian kali ini akan dibagi menjadi 2 (dua) bagian, yaitu:
1. Query Test
2. Data Visualization Test

## I. Query Test A (Poin 25)
Sebelum Anda mengerjakan soal ini, lakukan beberapa hal berikut:
1. Buatlah sebuah database kosong bernama hotwheels
2. Masuk ke dalam database hotwheels
3. Copy-paste dan run [query](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/hotwheels_db.sql) ini untuk membangun table-table yang dibutuhkan

Buka MySQL Workbench Anda dan selesaikan persoalan di bawah ini menggunakan database: Hot Wheels.

1. **(poin 5)** Tampilkan jumlah total customer yang Anda layani, beserta jumlah total kota & negara asal customer-customer Anda. Contoh output yang diharapkan:

    ![soal1](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql1.jpg?raw=true)


2. **(poin 5)** Tampilkan resources yang Anda miliki, mulai dari jumlah karyawan, jumlah kantor & lokasi negaranya, jumlah barang yang dijual, total stok barang & jumlah vendor yang menjadi partner Anda. Contoh output yang diharapkan:

    ![soal2](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql2.jpg?raw=true)

3. **(poin 5)** Dari soal nomor 2, Anda mengetahui anda memiliki 23 karyawan. Tampilkan jumlah karyawan yang bekerja di tiap-tiap kantor Anda yang tersebar di beberapa negara. Contoh output yang diharapkan:

    ![soal3](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql3.jpg?raw=true)

4. **(poin 5)** Dari soal nomor 2 tercatat Anda memiliki 110 model die cast dengan total stok 555,131 items. Jika dikategorikan, produk yang Anda jual terbagi menjadi 7 product line die cast, yakni model mobil klasik, mobil vintage, sepeda motor, pesawat terbang, kapal laut, kereta api serta truk & bus. Rumuskan single query yang dapat menampilkan harga produk terendah & tertinggi untuk masing-masing kategori. Contoh output yang diharapkan:

    ![soal4](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql4.jpg?raw=true)

5. **(poin 5)** Tampilkan daftar 10 customer paling royal (paling banyak mendatangkan uang bagi kita), yang total nominal transaksinya paling tinggi. Data yang ditampilkan adalah nama customer, kota & negara asal, beserta total uang yang dihabiskan di produk kita. Contoh output yang diharapkan:

    ![soal5](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql5.jpg?raw=true)

Simpan semua query ke dalam satu buah text file (boleh di Notepad).

## II. Query Test B (Poin 15)

Buka Jupyter Notebook Anda. Buatlah koneksi ke SQL Server Anda, sehingga Anda dapat menggunakan query untuk menampilkan table dalam bentuk `DataFrame`.

Kerjakan soal-soal berikut:

1. **(poin 5)** Pada 2003-06-05, terdapat pembayaran masuk sebesar US$ 14571.44. Tampilkan data seputar transaksi tersebut, mencakup nama customer yang melakukan pembayaran, nama produk yang dibeli, jumlah tiap produk yang dibeli dan harga satuannya. Pastikan total harga yang dibeli sesuai dengan data pembayaran masuk. Output yang diharapkan:

    ![soal6](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql6.jpg?raw=true)

2. **(poin 5)** Tampilkan 10 (sepuluh) orderNumber dengan nominal transaksi terbesar. Tampilkan juga nama customer yang melakukan pemesanan dengan orderNumber terkait. Berikut dengan asal kota dan negaranya. Output yang diharapkan:

    ![soal7](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql7.jpg?raw=true)

3. **(poin 5)** Tampilkan 10 (sepuluh) mainan yang paling laris (Most Wanted Items) atau yang paling sering diorder oleh customer pada tahun 2003. Output yang diharapkan:

    ![soal8](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/sql8.jpg?raw=true)


## III. Data Visualization Test (60)
Pada ujian Data Visualization, Anda akan menggunakan dataset Collision-Dataset. Dataset ini me-*record* data kecelakaan yang terjadi di Kota Seattle, Amerika Serikat. Silahkan download dataset ini di chat. Dan Anda dapat membaca penjelasan tiap kolom bisa Anda baca [di sini](https://github.com/ridhoaryo/UjianSusulan_DataViz_JCDS02_BKS/blob/master/columns_information.ipynb). Masih dalam Jupyter Notebook Anda, kerjakan soal-soal berikut.

1. **(poin 5)** Menurut dataset collision, berapa perbandingan rasio kecelakaan antara kategori Injury Collision dengan Property Damage Collision? (Jawab pertanyaan ini menggunakan plot yang sesuai dan jelaskan ratio perbandingannya dalam markdown!)

2. **(poin 10)** Menggunakan kolom `PERSONCOUNT`,  `PEDCOUNT`, `PEDCYLCOUNT`, `VEHCOUNT`. Hitunglah dan tampilkan dari tiap kolom tersebut hasil dari:
    - Data Central Tendency (Mean, Median dan Mode)
    - Data Dispersion (Persebaran data atau Standard Deviation)
    - IQR, Upper bound dan Lower Bound
    - Skewness Test

3. **(poin 10)** Menggunakan jawaban dari pertanyaan nomor 2, selesaikan persoalan berikut:
    
    - Buatlah sebuah boxplot untuk setiap kolom `PERSONCOUNT`,  `PEDCOUNT`, `PEDCYLCOUNT`, `VEHCOUNT`. Dalam tiap boxplot tampilkan garis untuk median **(biru)**, Upper bound **(jingga)** dan Lower bound **(hijau)** dari setiap kolom tersebut. Dan tampilkan dalam `dataframe` data-data yang termasuk dalam outliers?
    - Berdasarkan Skewness Test dari setiap kolom yang sudah Anda lakukan, jelaskan kolom mana yang termasuk skew, dan kolom mana yang tidak termasuk skew?

4. **(poin 10)** Menggunakan kolom `INCDATE` buatlah 2 (dua) kolom baru yang tiap kolom hanya menyimpan value **tahun** dan kolom lainnya menyimpan value **jam**. Dan tampilkan dalam sebuah `piechart` kecelakaan apa yang sering terjadi pada pukul 00:00 dini hari!

5. **(poin 15)** Saya memiliki asumsi bahwa, dari data tahun ke tahun, rasio kecelakaan yang terjadi akibat pengendara yang terpengaruh alkohol lebih sering terjadi pada pukul 20:00 malam. Apakah Anda setuju dengan asumsi saya? Jika iya, jelaskan alasannya. Jika tidak, jelaskan alasannya. Anda perlu menggunakan `stackplot` untuk menjawab pertanyaan ini.

6. **(poin 10)** Berdasarkan jumlah laporan kecelakaan dari tahun ke tahun pada dataset ini, tahun 2011 adalah tahun di mana jumlah laporan kecelakaan tercatat paling banyak. Apakah Anda setuju dengan hal ini? Gunakan plot yang sesuai untuk mendukung jawaban Anda.

## Catatan Penting:
Upload Text File yang berisi jawaban Query dan file ipynb ini ke dalam satu buah repository di github. Lalu kirim linknya ke email ridhoaryo1991@gmail.com dan email operasional Purwadhika.

## Happy Coding And Analyzing!