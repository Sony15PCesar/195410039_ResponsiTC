195410039_ResponsiTekCloud
Petunjuk :
1. Membuat repository di Github, kemudian lakukan UP FILE pada repository yang telah dibuat
2. Membuat repository baru pada Docker Hub, kemudian kaitkan repository GitHub dengan repository Docker Hub
3. Gunakan link image php:7.4-apache :
      https://hub.docker.com/_/php
      atau gunakan
      https://katacoda.com/courses/ubuntu/playground1804
4. Git clone repository pada Github :
      https://github.com/Sony15PCesar/195410039_responsitc.git
5. Pull image yang telah dibuat pada Docker Hub :
      docker pull sonypintoko15/repotc
6. Masuk ke dalam directory (repository) pada Github :
      cd 195410039_responsitc
7. Jalankan perintah docker compose :
      docker-compose up -d
8. Setelah selesai jika anda memakai katacoda, klik Web Preview dan pilih :
      Select port to view on Host 1
      kemudian Display port 8080
   jika memakai link image php:7.4-apache, buka buka web browser anda lalu masuk ke localhost :
      localhost --> masuk ke menu web
      localhost:8080 --> masuk database
 9. Login ke dalam database yang sebelumnya telah dibuat dengan :
      user = "root";
      pass = "example";
      db_name = "";
10. Kemudian create database dengan nama : tutorialweb
11. create tabel dengan nama : mahasiswa
12. buatlah databasesql dengan ketentuan berikut :
  `nim` int(11) NOT NULL,
  `password` varchar(35) NOT NULL,
  `nama` varchar(50) NOT NULL,
  `tempat_lahir` varchar(20) NOT NULL,
  `tanggal_lahir` date NOT NULL,
  `email` varchar(50) NOT NULL,
  `jenis_kelamin` varchar(20) NOT NULL,
  `agama` varchar(20) NOT NULL,
  `jurusan` varchar(30) NOT NULL,
  `semester` varchar(2) NOT NULL,
  `tahun_masuk` varchar(5) NOT NULL,
  `alamat` varchar(100) NOT NULL,
  `foto` varchar(100) NOT NULL,
  `status` int(1) NOT NULL
 ) ENGINE=InnoDB DEFAULT CHARSET=latin1;
13. Untuk menjalankannya jika memakai katacoda klik Web Preview dan pilih :
    view HTTP port 80 on Host 1
    kemudian jalankan.
    jika memakai link image php:7.4-apache, buka lagi localhost, lalu masuk ke menu CRUD. sekarang telah bisa menjalankannya.
14. Untuk mematikan docker ketikkan pada terminal perintah :
      docker-compose stop
15. Selesai.




