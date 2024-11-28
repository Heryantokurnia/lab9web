# Lab9Web
Nama : Heryanto Kurnia Putra

Nim  : 312310268
## Persiapan Lingkungan Praktikum:
- Install XAMPP sebagai server lokal untuk menjalankan PHP dan Apache. Unduh dari situs XAMPP dan ekstrak di lokasi yang Anda pilih (misalnya, d:\xampp).
- Jalankan XAMPP melalui XAMPP Control Panel, pastikan Apache dan MySQL aktif.
- Uji server dengan membuka `http://localhost` di browser. Jika halaman XAMPP tampil, server telah berfungsi dengan baik.

## Buat Direktori Project:
- Buat folder baru bernama `lab9_php_modular` di dalam folder `htdocs` (misalnya, `d:\xampp\htdocs\lab9_php_modular`).
- Akses folder tersebut di browser dengan URL: `http://localhost/labab9_php_modular/`.

## Langkah - langkah praktikum
- buat file dengan nama `header.php` di dalam folder `lab9_php_modular`
``` php
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Contoh Modularisasi</title>
        <link href="style.css" rel="stylesheet" type="text/stylesheet" media="screen" />
    </head>
    <body>
        <div class="container">
                <header>
                    <h1>Modularisasi Menggunakan Require</h1>
                </header>
            <nav>
                <a href="home.php">Home</a>
                <a href="about.php">Tentang</a>
                <a href="kontak.php">Kontak</a>
            </nav>
```
- buat file `footer.php` di dalam folder `lab9_php_modular`
``` php
                <footer>
                    <p>&copy; 2021, Informatika, Universitas Pelita Bangsa</p>
                </footer>
        </div>
    </body>
</html>
```
- buat file baru dengan nama `home.php` di dalam folder `lab9_php_modular`
```php
<?php require('header.php'); ?>

<div class="content">
    <h2>Ini Halaman Home</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>

<?php require('footer.php'); ?>
```
- buat file baru dengan nama `about.php` di dalam folder `lab9_php_modular`
```php
<?php require('header.php'); ?>

<div class="content">
    <h2>Ini Halaman About</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>

<?php require('footer.php'); ?>
```
- Akses hasilnya di http://localhost/lab9_php_modular/
  
