
## Praktikum Teknologi Cloud Computing - Minggu 11 (Application Containerization & Microservice Orchestration)

## 205611034 Danis Apriyanto

1. Melakukan _clonning_ repo dari git dan mengakses direktori, serta memeriksa _branch_ dari repo tersebut.

    ![](img/gambar-01.jpg)

2. Kemudian memeriksa `branch step0` untuk melihat file didalamnya. Dan kemudian melihat isi dari file `python linkextractor`.

    ![](img/gambar-02.jpg)

3. Menjalankan file `linkextractor.py.`

    ![](img/gambar-03.jpg)

4. Memeriksa _branch step1_ untuk melihat file didalamnya.

    ![](img/gambar-04.jpg)

5. Kemudian melihat isi dari file `Dockerfile`

    ![](img/gambar-05.jpg)

6. Membangun _docker image_ kita, dengan menjalankan perintah seperti gambar berikut dan sekaligus manghasilkan outputnya.

    ![](img/gambar-06.jpg)

    ![](img/gambar-07.jpg)

7. Selanjutnya membuat _docker image_ bernama _linkextractor: step1_ selanjutnya kroscek dengan melihat daftar/list dari _image docker_ yang sudah ada. Dan melakukan ekstrak docker image kita dengan mendapat URL

    ![](img/gambar-08.jpg)

    Gambar berikut merupakan _output_ apabila kita mengakses alamat URL tersebut.

    ![](img/gambar-09.jpg)

8. Kemudian melakukan percobaan pada halaman web untuk melihat lebih banyak tautan.

    ![](img/gambar-10.jpg)

9. Dan memeriksa _branch_ step 2 dan daftar file yang ada di dalamnya.

    ![](img/gambar-11.jpg)

10. Secara otomatis file `linkextractor.py` akan diupdate, berikut merupakan hasil _update_ dari file tersebut.

    ![](img/gambar-12.jpg)

11. Selanjutnya membuat _image_ baru

    ![](img/gambar-13.jpg)

12. Hasilnya _image docker_ yang baru dibuat dengan nama `linkextractor:step02` kita cek pada pada _list image docker_ yang sudah ada.

    ![](img/gambar-14.jpg)

13. Menjalankan _image docker_ tersebut dan menghasilkan _out put_ seperti gambar berikut:

    ![](img/gambar-15.jpg)

14. Kemudian menjalankan `image docker step1` yang sebelumnya dan menghasilkan keluaran yang masih sama seperti gambar berikut:

    ![](img/gambar-16.jpg)

15. Memeriksa `branch step3` dan isi file didalamnya.

    ![](img/gambar-17.jpg)

16. Kroscek `Dockerfile` untuk melihat perubahannya.

    ![](img/gambar-18.jpg)

17. Kemudian melihat isi dari file `main.py` yang baru ditambahkan tersebut.

    ![](img/gambar-19.jpg)

18. Kemudian _update_ `image docker step3` ini dengan beberapa langkah perubahan, seperti gambar berikut.

    ![](img/gambar-20.jpg)

    ![](img/gambar-21.jpg)

19. Menjalankan _container_ dalam mode (-d flag) sehingga terminal dapat tersedia untuk perintah yang lain saat _container_ masih berjalan. 

    Perhatikan juga bahwa disitu terdapat port 5000 dari _container_ dengan host 5000 (menggunakan perintah -p 5000: 5000) agar dapat diakses dari host. Dan juga memberikan nama (--name = linkextractor) ke _container_ untuk lebih mudah melihat log atau menghapus _container_. Serta melihat list _image container_ yang baru dibuat tersebut.

    ![](img/gambar-22.jpg)    

20. Membuat permintaan HTTP dalam bentuk `/api/url` untuk mengakses server ini dan mengambil respons berisi link yang diekstrak.

    ![](img/gambar-23.jpg)

21. Karena container berjalan dalam mode terpisah, jadi tidak dapat melihat proses yang terjadi di dalam. Tetapi dapat melihat _log_ menggunakan `linkextractor` yang di tetapkan untuk _container_. Serta menghapus _image container_ ini.

    ![](img/gambar-24.jpg)

22. Selanjutnya memeriksa `branch step4` dan isi file didalamnya.

    ![](img/gambar-25.jpg)

23. Melihat isi dari file `docker-compose.yml` dan `www/index.php`.

    ![](img/gambar-26.jpg)

24. Membuat mode terpisah untuk _container_.

    ![](img/gambar-27.jpg)

    ![](img/gambar-28.jpg)

25. Memeriksa daftar _container_ yang sedang berjalan serta memastikan bahwa kedua _container_ tersebut dapat berjalan dan mengkases layanan API.

    ![](img/gambar-29.jpg)

    Sehingga ketika megkasesnya pada URL, maka hasilnya seperti pada gambar berikut:

    ![](img/gambar-30.jpg)

26. Kemudian modifikasi file www/index.php mengganti semua kemunculan Link _Extractor_ dengan Super Link _Extractor_. Kemudian mengembalikan perubahan, dan menonaktifkan _container_ berikut.

    ![](img/gambar-31.jpg)

27. Kemudian memeriksa _branch step5_ dan melihat isi file didalamnya.

    ![](img/gambar-32.jpg)

28. Memeriksa file Dockerfile yang baru di dalam direktori `cat www/Dockerfile`

    ![](img/gambar-33.jpg)

29. Selanjutnya, melihat isi file `api/main.py` dengan menggunakan server redis.

    ![](img/gambar-34.jpg)

30. Melihat hasil perubahan pada file `docker-compose.yml.`

    ![](img/gambar-35.jpg)

31. Selanjutnya melakukan eksekusi container ini, untuk bisa di buka pada browser.

    ![](img/gambar-36.jpg)

    ![](img/gambar-37.jpg)

    Sehingga hasilnya ketika ditampilkan pada browser, seperti pada gambar berikut:

    ![](img/gambar-38.jpg)

32. Selanjutnya memeriksa apakah layanan redis dipakai atau tidak.

    ![](img/gambar-39.jpg)

33. Memeriksa ketika folder _www_ tidak tersedia pada _container_ yang sedang berjalan. kemudian melakukan verifikasi bahwa perubahan yang dibuat secara lokal tidak berada dalam layanan yang berjalan dengan memuat ulang halaman web dan kemudian mengembalikan perubahan. Dan menonaktifkan cointainer berikut.

    ![](img/gambar-40.jpg)    

34. Selanjutnya memeriksa _branch step6_ dan melihat isi file didalamnya.

    ![](img/gambar-41.jpg)

35. Selanjutnya melihat isi file `linkextractor.rb` ini merupakan file _ruby_ untuk mengelola _dependency_. Kemudian juga melihat isi file `Dockerfile`.

    ![](img/gambar-42.jpg)

    ![](img/gambar-43.jpg)

36. Kemudian mengecek perubahan pada file `docker-compose.yml.`

    ![](img/gambar-44.jpg)

37. Kemudian selanjutnya mengeksekusi container ini.

    ![](img/gambar-45.jpg)

    ![](img/gambar-46.jpg)

    Selanjutnya harus dapat mengakses API (menggunakan nomor port yang diperbarui):

    ![](img/gambar-47.jpg)

    Hasil yang ditampilkan pada halaman browser seperti gambar berikut:

    ![](img/gambar-48.jpg)

38. Kemudian _shut down container_ ini tetapi _log_ akan tetap ada, walaupun _container_ akan hilang.

    ![](img/gambar-49.jpg)


Terima kasih


