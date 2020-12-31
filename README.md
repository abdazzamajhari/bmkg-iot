
## Importer Data Prakiraan Cuaca BMKG

<img src="https://data.bmkg.go.id/include/assets/img/cuaca.svg" width="100" height="100">

Script PHP untuk import data prakiraan cuaca dari BMKG, dan ditambahkan ke database MYSQL, sehingga untuk kebutuhan ambil data cuaca bisa langsung query tanpa harus rekues lagi ke server BMKG

Apa yang saya lakukan dengan data ini?

Aplikasi saya bisa mencari wilayah terdekat dari table **t_wilayah**, sehingga cuaca yang ditampilkan sesuai wilayahnya terdekat, di Android saya buat versi SQLITE dan saya query wilayah terdekat dari situ, lalu ambil data cuacanya ke server.

Script ini bisa dijalankan di Browser ataupun di command line, tapi bagusnya di commandline dan gunakan [crontab](https://crontab.guru/#0_3_*_*_*) agar dieksekusi tiap waktu yang ditentukan

Dan ingat, bahwa anda harus memberitahukan jika datanya dari BMKG.

## Instalasi

Copy **config.example.php** menjadi **config.php**
ganti isinya dengan konfigurasi database anda
impor **bmkg.sql** ke database anda
pada file **bmkg.php** di paling bawah, **hapus** bagian **git**
kecuali anda mau host datanya di Github juga

#### Sumber
-  [BMKG](http://data.bmkg.go.id/prakiraan-cuaca/)
-  [ICON](http://www.iconarchive.com/tag/weather)
-  [Medoo](http://www.iconarchive.com/tag/weather)
