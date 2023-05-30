# E-Commerce Customer Churn

## Business Problem Understanding

### Context
Customer atau pelanggan merupakan hal yang sangat penting bagi kelangsungan hidup suatu perusahaan baik perusahaan barang maupun jasa. Dengan ditinggalkan pelanggan sebuah perusahaan akan mengalami kerugian yang sangat besar.

Kehilangan pelanggan (Customer Churn) juga menjadi salah satu tantangan yang harus dihadapi oleh perusahaan e-commerce, dimana konsumen pada e-commerce dengan mudah membandingkan produk dan jasa yang mereka peroleh dan dengan mudah berpindah ke komptitor lain (Pondel dkk, 2021).

Menurut Hong dalam Yulianti (2016), churn pelanggan adalah kecenderungan pelanggan untuk meninggalkan penyedia layanan, atau beralihnya pelanggan dari satu penyedia layanan ke yang lainnya. Sementara itu, menurut Lazarov et al dalam Suryana (2014) churn berasal dari kata “change” dan “turn” yang berarti tidak berlanjutnya kontrak. Hal ini telah menjadi isu penting yang merupakan salah satu tantangan utama oleh banyak perusahaan di era global ini dan harus dihadapinya. Disamping itu menurut Mathai (2020) Biaya untuk mendapatkan pelanggan baru biasanya lima sampai enam kali lebih tinggi dari pada biaya mempertahankan pelanggan yang sudah ada. Melihat begitu mahalnya untuk memperoleh pelanggan baru tentunya perusahaan akan lebih memilih mempertahankan pelanggan dibanding dengan mendapatkan pelanggan baru. Melihat hasil fakta tersebut maka banyak perusahaan sekarang lebih beralih untuk mempertahankan pelanggan yang ada dan menghindari churn pelanggan.

### Problem Statement
Pada e-commerce, konsumen dengan mudah membandingkan produk dan jasa yang mereka peroleh dan dengan mudah berpindah ke komptitor. Hal ini akan merugikan perusahaan karena akan mengurangi jumlah pelanggan dan akan berdampak pada berkuranganya pendapatan perusahaan. sehingga perusahaan harus mencari cara untuk mempertahannkan customer tersebut agar tidak churn dan berpindah ke kompetitor.

### Goals
Berdasarkan permasalahan yang dihadapi, perusahaan harus bisa memprediksi customer yang berpotensi melakukan churn dengan tepat, lalu memberikan treatment yang tepat untuk customer tersebut agar tidak churn. Sehingga perusahaan bisa mempertahankan keuntungan yang telah didapatkan.

### Analytic Approach
Pendekatan awal yang akan dilakukan adalah dengan menganalisa data untuk menemukan pola yang membedakan customer yang akan churn atau tidak.

Kemudian kita akan melakukan prediksi menggunakan machine learning dengan metode Supervised Learning (Binary Classification). kita akan mengevaluasi beberapa model klasifikasi yang memberikan prediksi paling akurat pada seorang pelanggan yang akan/ingin berhenti menggunakan produk/layanan.

### Metric Evaluation
Target:

![Untitled](https://github.com/yunisartika26/Capstone-Project-Modul-3/assets/124022134/4f180d7f-e807-4941-af7c-54d3814535e8)


0: customer tidak churn

1: customer churn

Confusion Metrix Term:

TP: customernya aktualnya churn dan diprediksi churn
TN: customernya aktualnya tidak churn dan diprediksi tidak churn
FN: customernya aktualnya churn dan diprediksi tidak churn
FP: customernya aktualnya tidak churn dan diprediksi churn
FN (False Negative):

Kekurangan

Kehilangan customer (alias churn)
Adanya cost customer acquistion untuk menggantikan customer yang telah churn
FP (False Positive):

Kekurangan

Salah target treatment untuk customer yang tidak churn (tapi diprediksi churn)
Sia-sianya biaya customer retention, waktu dan sumber daya
Jadi, model yang kita cari adalah model yang mengurangi hilangnya pelanggan loyal, tetapi tetap memperhatikan pengeluaran biaya pemasaran untuk pelanggan yang kurang tepat. Recall dan precision yang diseimbangkan akan dari kelas positif (Pelanggan churn). Metrik yang akan digunakan adalah ROC-AUC.
