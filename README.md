# Praktikum 8 -- PHP dan Database MySQL

-   Nama: Siti Azka Ikrima
-   NIM: 312510315
-   Kelas: I251C
-   Mata kuliah: Pemrograman Web

## Tujuan Praktikum

1.  Memahami konsep dasar database.
2.  Memahami konsep dasar CRUD menggunakan PHP.
3.  Membuat program CRUD sederhana menggunakan PHP.

## Perangkat

-   XAMPP (Apache dan MySQL/MariaDB)
-   phpMyAdmin
-   Visual Studio Code
-   Browser

## Database

-   Nama database: `latihan1`
-   Nama tabel: `data_barang`

Kolom tabel: `id_barang`, `kategori`, `nama`, `gambar`, `harga_beli`,
`harga_jual`, `stok`.

## Data Awal

Tabel `data_barang` diisi dengan tiga data awal: 1. HP Samsung Android
2. HP Xiaomi Android 3. HP OPPO Android

Ketiganya menggunakan kategori `Elektronik`.

## Langkah Praktikum

### 1. Persiapan server

Jalankan Apache dan MySQL melalui XAMPP. Buka phpMyAdmin melalui
`http://localhost/phpmyadmin/`.

### 2. Membuat database dan tabel

Buat database `latihan1`, kemudian buat tabel `data_barang` dengan kolom
sesuai struktur di atas. Kolom `id_barang` menjadi primary key dan
menggunakan auto increment.

### 3. Memasukkan data awal

Masukkan tiga data barang elektronik: HP Samsung Android, HP Xiaomi
Android, dan HP OPPO Android.

### 4. Membuat koneksi (`koneksi.php`)

File ini menggunakan `mysqli_connect()` untuk menghubungkan PHP dengan
database `latihan1`.

### 5. Menampilkan data -- Read (`index.php`)

Query `SELECT` mengambil seluruh data dari tabel `data_barang`. Hasilnya
ditampilkan dalam tabel HTML menggunakan perulangan.

### 6. Menambah data -- Create (`tambah.php`)

Formulir menerima data barang melalui metode POST. Data disimpan
menggunakan query `INSERT`. File gambar diterima melalui `$_FILES` dan
dipindahkan ke folder `gambar`.

### 7. Mengubah data -- Update (`ubah.php`)

Data barang dipilih berdasarkan `id_barang`. Formulir menampilkan data
lama dan perubahan disimpan menggunakan query `UPDATE`.

### 8. Menghapus data -- Delete (`hapus.php`)

Data dihapus berdasarkan `id_barang` menggunakan query `DELETE`.

## Struktur Folder

``` text
lab8_php_database/
├── koneksi.php
├── index.php
├── tambah.php
├── ubah.php
├── hapus.php
├── style.css
```

## Dokumentasi

Database latihan1:
![database](<ss/Screenshot 2026-11-16 110753.png>)

Tabel data_barang:
![tablemysql](<ss/Screenshot 2026-11-16 110809.png>)
![tablesheet](<ss/Screenshot 2026-11-16 110826.png>)

Tabel:
![tabelweb](<ss/Screenshot 2026-11-16 111030.png>)

Tambah Barang:
![tambah](<ss/Screenshot 2026-11-16 111209.png>)

Ubah Barang:
![ubah](<ss/Screenshot 2026-11-16 111233.png>)


## Kesimpulan
Praktikum ini menerapkan PHP dan MySQL untuk membuat aplikasi
pengelolaan data barang dengan operasi CRUD, yaitu Create, Read, Update,
dan Delete.