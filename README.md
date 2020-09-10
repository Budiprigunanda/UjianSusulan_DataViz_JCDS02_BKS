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
Masih dalam Jupyter Notebook Anda, kerjakan soal-soal berikut.

1. Import semua table yang ada di database world (ada 3 tables), jadikan table-table tersebut menjadi 3 dataframe yang berbeda. **Hapus** semua data `NaN`. Kemudian, tampilkan 3 dataframe tersebut dengan ketentuan sebagai berikut:
    - Menggunakan Dataframe `country`, tampilkan 10 (sepuluh) negara dengan populasi terkecil.
    
    ![slicing1](https://github.com/ridhoaryo/Ujian_DataViz_JCDS02_BKS/blob/master/slicing1.jpg?raw=true)

    - Menggunakan Dataframe `city`, tampilkan 10 (sepuluh) countrycode dengan rata-rata populasi terbesar.

![slicing2](https://github.com/ridhoaryo/SEA_Games/blob/master/slicing2.jpg?raw=true)

    - Menggunakan Dataframe `countrylanguage`, tampilkan 10 (sepuluh) bahasa yang paling banyak digunakan di dunia.
        ![slicing3](https://github.com/ridhoaryo/SEA_Games/blob/master/slicing3.jpg?raw=true)

2. Buatlah sebuah Pie Chart yang menampilkan presentase populasi dari setiap benua. Menggunakan Pie Chart yang sudah dibuat, jawablah pertanyaan berikut:
    - Dilihat dari presentase tiap benua, benua manakah yang menjadi penyumbang populasi terbanyak?
    - Berapa presentase populasi manusia yang berada di benua Amerika Utara?

3. **(Gunakan nama benua pada pertanyaan nomer 2 poin pertama)** Pada soal nomor 3 ini, buatlah sebuah horizontal barplot, yang membagi tiap negara dalam benua tersebut. Tampilkan secara berurutan dalam barplot, 10 (sepuluh) negara yang menyumbang populasi terbanyak. Kriteria barplot:
    - Munculkan text `Total Population: ` pada tiap bar seperti contoh di bawah ini. Plot berikut hanya ilustrasi.

        ![contoh](https://github.com/ridhoaryo/SEA_Games/blob/master/contoh%20barplot.jpg?raw=true)

    Jawablah pertanyaan di bawah ini, berdasarkan horizontal bar plot yang sudah Anda buat.
    - Sebutkan negara dengan populasi terbanyak!
    - Negara apakah yang menjadi urutan ke 10 berdasarkan horizontal barplot yang sudah Anda buat?
    - Berapakah populasi negara yang berada di urutan ke-3?

4. Hitunglah:
    - IQR dari Angka Harapan Hidup (Life Expectancy) dari Benua Asia
    - Hitunglah juga, Mean, Median, Standard Deviation, Upper Boundaries serta Lower Boundaries.

    Buatlah sebuah Distribution Plot dari Angka Harapan Hidup di Benua Asia. Dan tampilkan pula di dalam Distribution Plot tersebut:
    - Garis vertikal untuk menandakan dimanakah letak Mean, Median, Upper Boundaries dan Lower Boundaries

    Menurut Distribution Plot tersebut jawablah pertanyaan ini:
    - Apakah terdapat negara yang Angka Harapan Hidup-nya berada pada outliers? Jika ada, tampilkan dalam bentuk Dataframe, data dari negara tersebut.
    - Jika tidak ada, cukup jawab dengan 'Tidak ada.'

5. Data GNP (Gross National Product) pada Dataframe `country` saat ini, masih dalam satuan "million USD". Sehingga, jika Anda menemukan negara dengan GNP 10, maka nominal GNP sesungguhnya dari negara tersebut adalah 10,000,000 USD. Mengetahui hal itu maka, selesaikan tugas berikut:
    - Ubah value dalam kolom GNP ke nominal sesungguhnya (dikali 1,000,000)
    - Buatlah sebuah function bernama `percapita()` yang berisi rumus untuk menghitung GNP per Capita. Kemudian, buatlah kolom baru bernama `GNPperCapita` di Dataframe `country`, lalu isi kolom tersebut menggunakan function yang tadi sudah dibuat.

6. Saya memiliki asumsi bahwa negara-negara dengan `LifeExpectancy` yang tinggi akan selalu memiliki `GNPperCapita` yang tinggi pula. Dan ini berarti `LifeExpectancy` dan `GNPperCapita` memiliki korelasi positif yang signifikan. Apakah Anda setuju dengan asumsi saya?
    - Jawablah pertanyaan ini menggunakan chart/plot yang sesuai (setidaknya ada 2 chart/plot), sehingga dapat melandasi jawaban Anda!
    - Jika Anda setuju jelaskan alasannya, dan jika anda tidak setuju jelaskan juga alasannya!
    - Serta tampilkan dalam bentuk `DataFrame` benua manakah yang salah satu negaranya mencetak `GNPperCapita` tertinggi, jika dibandingkan dari benua-benua lainnya!

## Catatan Penting:
Upload Text File yang berisi jawaban Query dan file ipynb ini ke dalam satu buah repository di github. Lalu kirim linknya ke email ridhoaryo1991@gmail.com dan email operasional Purwadhika.

## Happy Coding And Analyzing!