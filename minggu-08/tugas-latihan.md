
## Penjelasan Praktikum Teknologi Cloud Computing Minggu ke 08

1. Terlebih dulu membuat direktori baru untuk project dan kemudian masuk pada direktori tersebut, seperti pada gambar dibawah ini :


![](img/img1.jpg)

![](img/img2.jpg)

![](img/img3.jpg)

Perintah yang digunakan yakni :
* `mkdir composetest`
* `cd composetest`

2. Selanjutnya membuat file baru pada project dengan nama `app.py` file python ini akan menghubungkan ke jaringan redis yang nantinya dapat diakses. Dengan menambahkan script seperti pada gambar dibawah ini:

![](img/img4.jpg)

3. Kemudian membuat file `txt` dengan nama _requirements_ dan mengisihkan _script_ pada file tersebut, seperti dibawah ini:

![](img/img5.jpg)

4. Kemudian membuat file baru dengan nama `DockerFile` dan kemudian mengisihkan _script_ seperti dibawah ini:

![](img/img6.jpg)

    Pada script diatas akan berguna untuk mengeksekusi beberapa perintah yang berada pada beberapa file sebelumnya.

5. Dan kemudian untuk selanjutnya membuat file `yml`, dengan nama `docker-compose`. File ini akan berguna sebagai wadah untuk merujuk pada port 5000 yang nantinya dapat diakses. Seperti pada gambar dibawah ini:

![](img/img7.jpg)

    Script diatas merupakan _script_ yang akan menjadi layanan dengan menggunakan port default untuk server web Flask 5000.

6. Selanjutnya melakukan _running_ untuk project/direktori yang dibuat tadi dengan menggunakan `docker compose`, yang perintahnya yaitu `docker-compose up`, seperti pada gambar dibawah ini:

![](img/img8.jpg)

![](img/img9.jpg)

    Ketika perintah docker-compose up dijalankan maka otomatis sever akan runnig, dimana setiap proses running dilakukan maka akan otomatis merujuk pada image docker dan kemudian merequest ke server redis.

Sehingga hasilnya, apabila di open pada browser dengan mengakses _server host_ yakni 192.168.99.100:5000. Host ini fungsinya sama seperti penggunaan pada _docker dekstop_ yakni localhost:5000, karena disini saya menggunakan docker tollbox, maka host yang digunakan seperti berikut.

![](img/img10.jpg)

7. Kemudian apabila melakukan refresh pada browser maka secara otomatis akan di _count_ dimana setiap kali _request_ dilakukan maka nilainya akan bertambah, artinya akan menghitung jumlah _request time_ dari _client_. Seperti pada gambar berikut:

![](img/img11.jpg)

8. Selanjutnya mengeksekusi perintah untuk melihat daftar _image_ yang ada, dengan meggunakan perintah `docker image ls`, seperti gambar berikut:

![](img/img12.jpg)

    Dimana dari gambar diatas repo/image yang digunakan sekarang yaitu python dan redis.

9. Kemudian melakukan perubahan pada `file .yml` dengan menambahkan _script_ didalamnya seperti pada gambar berikut:

![](img/img13.jpg)

    Dimana perubahan dengan menambahkan dua variabel yaitu volumes dan environtment. 

10. Selanjutnya melakukan _running_ ulang dengan perintah `docker-compose up`, dan disitu terlihat perubahan, seperti gambar berikut:

![](img/img14.jpg)

    Dimana hasil update pada file yml akan ditampilkan ketika proses runnig ulang ke host seperti pada gambar diatas tersebut. 

11. Kemudian melakukan _update_ pada file `app.py` dengan merubah pesan seperti pada gambar berikut:

![](img/img15.jpg)

12. Dan melakukan eksperimen pada beberapa perintah `docker` yang ada. Dimana beberapa perintah ini akan melihat _container_ yang sedang _running_ pada _background_, melakukan _stop running container_, melihat _running_ pada _server web_ dan _volume container_, seperti gambar berikut:

![](img/img16.jpg)

Dokumen _Script_

### File app.py

[File app.py](https://github.com/danisapriyanto/tekn-cloud-computing/blob/master/minggu-08/app.py)

### Dockefile

[Dockefile](https://github.com/danisapriyanto/tekn-cloud-computing/blob/master/minggu-08/Dockerfile.txt)

