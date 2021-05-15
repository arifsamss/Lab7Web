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
http://localhost/lab7_php_dasar/latihan2.php?nama=Agung
![6  predefine](https://user-images.githubusercontent.com/81839328/118350687-5caab780-b582-11eb-98aa-c788bca153fe.JPG)

# 6. Membuat Form Input
~~~
<h2>Form Input</h2>
    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>
    <?php 
        echo 'Selamat Datang ' . $_GET['nama'];
    ?>
~~~
![7  Membuat form Input](https://user-images.githubusercontent.com/81839328/118350861-1013ac00-b583-11eb-8077-a21c871b0988.JPG)

# 7. Operator
~~~
<h2>Operator</h2>
    <?php
        $gaji = 1000000;
        $pajak = 0.1;
        $thp = $gaji - ($gaji*$pajak);
            echo "Gaji sebelum pajak = Rp. $gaji <br>";
            echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
~~~
![8  Operator](https://user-images.githubusercontent.com/81839328/118350911-36394c00-b583-11eb-916b-a495ad74e08b.JPG)

# 8. Kondisi IF
~~~
<h2>Kondisi IF</h2>
    <?php
        $nama_hari = date("l");
            if ($nama_hari == "Sunday") {
        echo "Minggu";
            } elseif ($nama_hari == "Monday") {
        echo "Senin";
            } else {
        echo "Selasa";
        }
~~~
![9  Kondisi IF](https://user-images.githubusercontent.com/81839328/118350932-4fda9380-b583-11eb-97d5-8b44071563d4.JPG)

# 9. Kondisi Switch
~~~
<h2>Kondisi Switch</h2>
    <?php
        $nama_hari = date("l");
            switch ($nama_hari) {
            case "Sunday":
        echo "Minggu";
            break;
            case "Monday":
    echo "Senin";
            break;
            case "Tuesday":
    echo "Selasa";
            break;
            default:
    echo "Sabtu";
            }
    ?>
~~~
![10  Kondisi Switch](https://user-images.githubusercontent.com/81839328/118350951-6a147180-b583-11eb-86ed-b7dcc8fe9074.JPG)

# 10. Perulangan FOR
~~~
<h2>Perulangan For</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            for ($i=1; $i<=10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
        }
        echo "Perulangan Menurun dari 10 ke 1 <br />";
            for ($i=10; $i>=1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
        }
    ?>
~~~
![11  Perulangan FOR](https://user-images.githubusercontent.com/81839328/118350967-86b0a980-b583-11eb-8097-c72294bd745a.JPG)

# 11. Perulangan While
~~~
h2>Perulangan While</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            $i=1;
            while ($i<=10) {
        echo "Perulangan ke: " . $i . '<br />';
            $i++;
        }
    ?>
~~~
![12  Perulangan While](https://user-images.githubusercontent.com/81839328/118351037-cf686280-b583-11eb-8078-ca3ed03e78c4.JPG)

# 12. Perulangan Do While
~~~
<h2>Perulangan Dowhile</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            $i=1;
            do {
        echo "Perulangan ke: " . $i . '<br />';
            $i++;
            } while ($i<=10);
    ?>
~~~
![13  Perulangan do while](https://user-images.githubusercontent.com/81839328/118351060-e7d87d00-b583-11eb-9e7a-165790e45b70.JPG)

# Pertanyaan dan Tugas
Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan
nama, tanggal lahir dan pekerjaan. Kemudian tampilkan outputnya dengan menghitung
umur berdasarkan inputan tanggal lahir. Dan pilihan pekerjaan dengan gaji yang
berbeda-beda sesuai pilihan pekerjaan.
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
<h2>Pertanyaan dan Tugas</h2>
    <form method="post">
            <label>Nama Lengkap: </label>
            <input type="text" name="nama">
            <br>
            <label>Tempat Lahir: </label>
            <input type="text" name="tempat_lahir">
            <br>
            <label>Tanggal Lahir: </label>
            <input type="date" name="tgl_lahir">
            <br>
            <label>Alamat: </label>
            <input type="text" name="alamat">
            <br>
            <label>Pekerjaan:
            <select name='pekerjaan'>
                <option value='Guru'>Guru</option>
                <option value='Dokter'>Dokter</option>
                <option value='Polisi'>Polisi</option>
                <option value='Pegawai Swasta'>Pegawai Swasta</option>
            </select>
            </label>
            <br>
            <input type="submit" value="Kirim">
    </form>
    <h2>Output</h2>
    <?php
        echo '<br> Nama Lengkap : ' . $_POST['nama'];
        echo '<br> Tempat Lahir : ' . $_POST['tempat_lahir'];
        echo '<br> Alamat : ' . $_POST['alamat'];
            $tgl_lahir = @$_POST['tgl_lahir'];
            $lahir = new DateTime($tgl_lahir);
            $hari_ini = new DateTime();
            $diff = $hari_ini->diff($lahir);
        echo "<br> Usia : ". $diff->y ." Tahun";
        echo "<br> Pekerjaan : ". $_POST['pekerjaan'];
            $pekerjaan = @$_POST['pekerjaan'];
            if($pekerjaan == "Guru"){
                echo '<br> Gaji : Rp. 4.000.000,-';
            }
            elseif($pekerjaan == "Dokter"){
                echo '<br> Gaji : Rp. .8.000.000,-';
            }
            elseif($pekerjaan == "Polisi"){
                echo '<br> Gaji : Rp. 5.000.000,-';
            }
            elseif($pekerjaan == "Pegawai Swasta"){
                echo '<br> Gaji : Rp. 5.100.000,-';
            }
    ?>
</html>
~~~
![14  Tugas](https://user-images.githubusercontent.com/81839328/118351121-35ed8080-b584-11eb-9ff9-077274c1cfba.JPG)
