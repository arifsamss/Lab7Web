# Pemograman Web
~~~
Nama  : Arif Samsudin
NIM   : 311910255
Kelas : TI 19 C1
~~~
# 1. Menjalankan Web Server
Untuk menjalankan web server dari menu XAMPP Control.
![1  Menjalankan web server](https://user-images.githubusercontent.com/81839328/118350422-c1fda900-b580-11eb-85a5-58dacfc133b0.JPG)

• Uji coba apakah server sudah berkerja dengan baik
   
   http://127.0.0.1 atau http://localhost 
   Tampil halaman utama XAMPP jika server sudah berkerja dengan baik.

• Dokumen Website 
  
  Semua file website tempatkan di direktori: \xampp\htdocs\

• Database MySQL 
  
  Direktori: \xampp\mysql\Manajemen database: http://localhost/phpmyadmin

# 2. Memulai PHP
Buat folder lab7_php_dasar pada root directory web server (d:\xampp\htdocs)
![2  Buat folder](https://user-images.githubusercontent.com/81839328/118350548-93cc9900-b581-11eb-95ac-186fa844f9e4.JPG)

Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL:http://localhost/lab7_php_dasar/
![3  Access Web](https://user-images.githubusercontent.com/81839328/118350562-a6df6900-b581-11eb-9418-5b180dadf186.JPG)

# 3. PHP Dasar
Buat file baru dengan nama php_dasar.php pada directory tersebut. Kemudian buat kode seperti berikut.
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World";
    ?>
</body>
</html>
~~~
Kemudian untuk mengakses hasilnya melalui URL:http://localhost/lab7_php_dasar/php_dasar.php
![4  PHP Dasar](https://user-images.githubusercontent.com/81839328/118350607-de4e1580-b581-11eb-8cdc-b3c7f29c8ebf.JPG)

# 4. Variable PHP
Menambahkan variable pada program.
~~~
<?php
$nim = "0411500400";
$nama = 'Abdullah';
echo "NIM : " . $nim . "<br>";
echo "Nama : $nama";
?>
~~~
![5  Menambahkan Variable](https://user-images.githubusercontent.com/81839328/118350656-28cf9200-b582-11eb-9a07-36d9796cacb4.JPG)

# 5. Predefine Variable $_GET
~~~
<?php
echo 'Selamat Datang ' . $_GET['nama'];
?>
~~~
Untuk mengaksesnya gunakan URL:
http://localhost/lab7_php_dasar/latihan2.php?nama=Arif%Samsudin
![6  predefine](https://user-images.githubusercontent.com/81839328/118350687-5caab780-b582-11eb-98aa-c788bca153fe.JPG)


