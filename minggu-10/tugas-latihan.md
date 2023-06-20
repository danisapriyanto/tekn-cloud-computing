
# Praktikum Teknologi Cloud Computing - Minggu ke 10 - Docker Networking

## 205611034 Danis Apriyanto

## Latihan dan Tugas

1. Pada bagian yang pertama kita akan menjalankan perintah utama untuk mengkonfigurasi dan mengelola jaringan kontainer, Seperti gambar berikut: `docker network`

    ![](img/img1.jpg)

2. Selanjutnya menjalankan perintah untuk melihat jaringan kontainer yang ada pada _host Docker_ saat ini, Seperti gambar berikut: `docker network ls`

    ![](img/img2.jpg)

3. Kemudian menggunakan perintah untuk melihat detail konfigurasi dari kontainer jaringan pada _docker host_ , Seperti gambar berikut: `docker network inspect bridge`

    ![](img/img3.jpg)

4. Menjalankan perintah untuk melihat daftar plugin jaringan, Seperti gambar berikut: `docker info`. 

    ![](img/img4.jpg)

5. Melihat jaringan penghubung pada daftar _docker host_ kita saat ini, seperti gambar berikut: `docker network ls`

    ![](img/img5.jpg)

6. Melakukan instalasi _brctl_ yang nantinya digunakan untuk mendaftar _bridges Linux_ di _host Docker_. Langkah-langkah seperti gambar berikut: `apk update` dan `apk add bridge`

    ![](img/img6.jpg)

    ![](img/img7.jpg)

    setelah itu menjalankan perintah untuk menampilakan _brctl_ apakah sudah terdapat _bridges_ yang berjalan pada _dcoker host_ seperti gambar berikut: `brctl show`

    ![](img/img8.jpg)

7. Menjalankan perintah untuk melihat detail _bridges docker_ yang sedang berjalan ketika ditampilkan pada perintah sebelumnya seperti gambar berikut: `ip a`

    ![](img/img9.jpg)

8. Membuat _container_ baru, Pembuatan _container_ baru ini berguna untuk dapat terhubung ke jaringan _bridges_ yang ada. seperti pada gambar berikut: `docker run -dt ubuntu sleep infinity`

    ![](img/img10.jpg)

9. Melihat _container_ baru yang dibuat tadi, _container_ baru ini bernama `ubuntu:lates`. Yang merupakan _image_ yang berkondisi _sleep_ tetapi sedang berjalan, seperti pada gambar  berikut: `docker ps`

    ![](img/img11.jpg)

10. Karena tidak ada jaringan yang ditentukan pada perintah _docker run_, kontainer secara otomatis akan ditambahkan ke jaringan _bridge_. Maka perlu melihat lagi _brctl_  seperti pada gambar berikut: `brctl show`

    ![](img/img12.jpg)

    hasil diatas _bridges docker0_ sudah terhubung. Bagian ini menghubungkan _bridges docker0_ ke _container_ yang baru saja dibuat.

11. Memeriksa ulang jaringan _bridges_ dengan perintah baru, seperti pada gambar berikut: `docker network inspect bridge`

    ![](img/img13.jpg)

    ![](img/img14.jpg)

12. Dari hasil sebelumnya dimana ip address yang didapatkan pada _bridges_ yaitu 172.17.0.2.Selanjutnya akan mencoba ping ke ip address tersebut untuk memastikan apakah sedang berjalan atau tidak, seperti pada gambar berikut: `ping -c5 172.17.0.2`

    ![](img/img15.jpg)

13. Selanjutnya melihat _ID bridges_ untuk nantinya dapat menghubungkan dengan URL lainnya, seperti pada gambar berikut: `docker ps`

    ![](img/gambar-16.jpg)
    
    ID adalah 079ed538c950, id ini nantinya akan digunakan untuk menjalankan shell pada container ubuntu seperti pada gambar berikut:
    
    ![](img/gambar-17.jpg)

    Dari gambar diatas sekaligus melakukan penginstalan program ping. Apabila sudah melakukan instalasi program ping maka selanjutnya kita mencoba ping ke url www.github.com. Untuk perintah dan hasilnya seperti pada gambar berikut:

    ![](img/gambar-18.jpg)

    ![](img/gambar-19.jpg)

    Selanjutnya keluar dari _running container_ tersebut, dengan menggunakan perintah seperti pada gambar berikut:

    ![](img/gambar-20.jpg)

    Hasil pada gambar diatas lansung melakukan pemberhentian untuk kontainer yang sedang berjalan dengan ID kita, untuk perintahnya seperti gambar diatas tersebut.

14. Memulai kontainer baru dan sekaligus menjalankannya dimana kontainer ini bernama official NGINX. Dimana _image_ ini berjalan pada web server pada port 80. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker run --name web1 -d -p 8080:80 nginx`

    ![](img/gambar-21.jpg)

15. Kemudian melakukan cek status container dan _port_ yang sedang berjalan, dari hasil _start_ sebelumnya. Untuk perintah dan hasilnya seperti gambar berikut: `docker ps`

    ![](img/gambar-22.jpg)

16. Menghubungkan _host docker_ dengan port 80, apabila tidak dapat membukanya pada web browser. Untuk perintah dan hasilnya seperti pada gambar berikut: `curl 127.0.0.1:8080`

    ![](img/gambar-23.jpg)

    ![](img/gambar-24.jpg)

17. Selanjutnya inisialisasi swarm baru. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker swarm init --advertise-addr $(hostname -i)`

    ![](img/gambar-25.jpg)

18. Menjalankan perintah untuk melihat node swarm yang sedang berjalan, seperti pada gambar berikut: `docker node ls`

    ![](img/gambar-26.jpg)

19. Membuat overlay jaringan dengan nama overnet. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker network create -d overlay pvernet`

    ![](img/gambar-27.jpg)

20. Menjalankan perintah untuk memastikan bahwa jaringan berhasil dibuat. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker network ls`

    ![](img/gambar-28.jpg)

    Gambar diatas menunjukan overnet jaringan berhasil dibuat.

21. Melihat kembali daftar jaringan pada docker host. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker network ls`

    ![](img/gambar-29.jpg)

22. Melihat detail informasi dari jaringan overnet. Untuk perintah dan hasilnya seperti gambar berikut: `docker network inspect overnet`

    ![](img/gambar-30.jpg)

23. Membuat layanan baru dengan nama myservice pada jaringan overnet dengan dua bagian. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker service create --name myservice \`

    ![](img/gambar-31.jpg)

24. Memastikan bahwa layanan yang dibuat dengan dua bagian sudah aktif. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker service ls`

    ![](img/gambar-32.jpg)

25. Memastikan bahwa dua node sedang berjalan. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker service ps myservice`

    ![](img/gambar-33.jpg)

26. Melakukan verifikasi jaringan dua bagian node yang sedang berjalan pada jaringan overnet. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker network ls`

    ![](img/gambar-34.jpg)

27. Detail jaringan overnet dan mendapatkan alamat ip dari running dua node yang ada. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker network inspect overnet`

    ![](img/gambar-35.jpg)

    ![](img/gambar-36.jpg)

28. Konfigurasi jaringan _myservice_. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker service inspect my service`

    ![](img/gambar-37.jpg)

29. Melakukan remove layanan myservice. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker service rm myservice`

    ![](img/gambar-38.jpg)

30. Melihat kembali _list_ jaringan container yang ada. Untuk perintah dan hasilnya seperti pada gambar berikut: `docker ps`

    ![](img/gambar-39.jpg)

31. Untuk menghapus node 1 dan 2 yang berjalan pada swarm. Untuk perintah dan hasilnya seperti pada gambar berikut:

    ![](img/gambar-40.jpg)

Terima kasih