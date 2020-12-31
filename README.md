
## Importer Data Prakiraan Cuaca BMKG

<img src="https://data.bmkg.go.id/include/assets/img/cuaca.svg" width="500" height="500">

Script PHP untuk import data prakiraan cuaca dari BMKG, dan ditambahkan ke database MYSQL, sehingga untuk kebutuhan ambil data cuaca bisa langsung query tanpa harus rekues lagi ke server BMKG

Apa yang saya lakukan dengan data ini?

Aplikasi saya bisa mencari wilayah terdekat dari table **t_wilayah**, sehingga cuaca yang ditampilkan sesuai wilayahnya terdekat, di Android saya buat versi SQLITE dan saya query wilayah terdekat dari situ, lalu ambil data cuacanya ke server.

Script ini bisa dijalankan di Browser ataupun di command line, tapi bagusnya di commandline dan gunakan [crontab](https://crontab.guru/#0_3_*_*_*) agar dieksekusi tiap waktu yang ditentukan

Dan ingat, bahwa anda harus memberitahukan jika datanya dari BMKG.

## Menjalankan Aplikasi
siapkan url endpoint https://abdazzamajhari.github.io/bmkg-iot/

dari aplikasi, unduh file wilayah.json https://abdazzamajhari.github.io/bmkg-iot/cuaca/wilayah.json

Dari json tersebut, kalkulasi lokasi user dengan wilayah terdekat, atau user pilih sendiri.

lalu download cuaca di wilayah yang dipilih berdasarkan kodenya https://abdazzamajhari.github.io/bmkg-iot/cuaca/idWilayah.json

contoh: https://abdazzamajhari.github.io/bmkg-iot/cuaca/501233.json

sesuaikan kode cuaca dengan icon di folder icon https://abdazzamajhari.github.io/bmkg-iot/icon/5.png

#### Sumber
-  [BMKG](http://data.bmkg.go.id/prakiraan-cuaca/)
-  [ICON](http://www.iconarchive.com/tag/weather)
-  [Medoo](http://www.iconarchive.com/tag/weather)
