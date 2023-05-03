
## 205611034 Danis Apriyanto

# Data as a service

Dalam komputasi, data sebagai layanan, atau DaaS, adalah istilah yang digunakan untuk menggambarkan perangkat lunak berbasis cloud yang digunakan untuk bekerja dengan data, seperti mengelola data di gudang data atau menganalisis data dengan kecerdasan bisnis. Ini diaktifkan oleh perangkat lunak sebagai layanan (SaaS).[1] Seperti semua teknologi "sebagai layanan" (aaS), DaaS dibangun di atas konsep bahwa produk datanya dapat diberikan kepada pengguna sesuai permintaan, [2] terlepas dari pemisahan geografis atau organisasi antara penyedia dan konsumen. Arsitektur berorientasi layanan (SOA) dan meluasnya penggunaan API telah menjadikan platform tempat data berada sebagai tidak relevan.[3]

Data sebagai layanan sebagai model bisnis adalah konsep ketika dua atau lebih organisasi membeli, menjual, atau memperdagangkan data yang dapat dibaca mesin dengan imbalan sesuatu yang bernilai.[4]

# Sofware Yang Diperlukan

* [Download GO](https://go.dev/doc/install)

* [Download MySQL](https://dev.mysql.com/downloads/installer/)

* [Download MonggoDB](https://www.mongodb.com/try/download/community)


## Implementasi Program Go Untuk Membaca Data Pada Mysql

Golang connection to PHPMySQL

1. Buat direktori `mkdir project-pertama`

2. Masuk ke direktori `cd project-pertama`

3. Untuk membuat go.mod `go mod init project-pertama`

4. Cek file terlebih dahulu `ls`

5. Setting path variabel `dir`

![](img/img1.jpg)

Install gopath

## Koneksi mysql

![](img/img2.jpg)

Untuk kode koneksi ke mysql sebagai berikut,

![](img/img10.jpg)


1. Instalasi driver terlebih dahulu ketik `go get github.com/go-sql-driver/mysql`

![](img/img7.jpg)

2. Buat database dan tabel di MySQL

![](img/img4.jpg)

3. Buat tabel

![](img/img5.jpg)

4. isikan data

![](img/img6.jpg)

5. Untuk menjalankan golang ketikan `go run main.go`

![](img/img8.jpg)

6. Masuk ke mongodb, 

![](img/img11.jpg)

instalasi ketikan `go get go.mongodb.org/mongo-driver/mongo`

![](img/img9.jpg)

7. Membuat project

![](img/img12.jpg)