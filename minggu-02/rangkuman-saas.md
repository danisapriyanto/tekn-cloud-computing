## Apa perbedaan utama antara IaaS, PaaS, dan SaaS?

Saya akan mencoba menjawab ini dari analogi, misalkan Anda ingin berselancar di internet,

Jadi anggaplah IaaS saat Anda membeli laptop untuk diri Anda sendiri, Anda bertanggung jawab atas segala sesuatu seperti menginstal sistem operasi, mengelola keamanan, menginstal perangkat lunak, dll, kemudian menginstal browser Anda dan kemudian melakukan penjelajahan. Jika sesuatu berjalan seperti kegagalan. Anda harus memperbaiki sendiri.

PaaS, Anda memiliki laptop pra-instal dengan sistem operasi dan persyaratan dasar, sekarang Anda hanya bertanggung jawab dari browser Anda.

Google App Engine, CloudFoundry, Heroku, AWS(Beanstalk) adalah beberapa contoh PaaS.

SaaS , seperti Anda telah menginstal semuanya bahkan browser pilihan Anda . Anda hanya bertanggung jawab untuk menggunakannya. Jika Anda merusak sesuatu, tanggung jawab penyedia untuk memulihkan semuanya.

GMAIL adalah contoh terbaik dari SaaS

Untuk Geeks:

Infrastruktur sebagai Layanan (IaaS): Ini hanya menyediakan infrastruktur dasar (Mesin virtual, Jaringan Definisi Perangkat Lunak, Penyimpanan terpasang). Pengguna akhir harus mengonfigurasi dan mengelola platform dan lingkungan, menerapkan aplikasi di dalamnya.

![Gambar teks editor VS Code](https://qph.cf2.quoracdn.net/main-qimg-d1772f25d7e8f52bbe60af735da1de59-pjlq)

Platform as a Service (PaaS): Ini menyediakan platform yang memungkinkan pengguna akhir untuk mengembangkan, menjalankan, dan mengelola aplikasi tanpa kerumitan membangun dan memelihara infrastruktur.

Perangkat Lunak sebagai Layanan (SaaS ): Kadang-kadang disebut sebagai "perangkat lunak berdasarkan permintaan". Biasanya diakses oleh pengguna menggunakan thin client melalui web browser. Di SaaS semuanya dapat dikelola oleh vendor: aplikasi, runtime, data, middleware, OS, virtualisasi, server, penyimpanan, dan jaringan, Pengguna akhir harus menggunakannya.

## Arsitektur SAAS:

Dengan model ini, satu versi aplikasi, dengan satu konfigurasi digunakan untuk semua pelanggan. Aplikasi diinstal pada beberapa mesin untuk mendukung skalabilitas (disebut penskalaan horizontal). Dalam beberapa kasus, versi kedua dari aplikasi disiapkan untuk menawarkan sekelompok pelanggan terpilih dengan akses ke versi pra-rilis aplikasi untuk tujuan pengujian. Dalam model tradisional ini, setiap versi aplikasi didasarkan pada kode yang unik. Meskipun pengecualian , beberapa solusi SaaS tidak menggunakan multitenancy, untuk mengelola sejumlah besar pelanggan secara hemat biaya. Apakah multitenancy merupakan komponen yang diperlukan untuk software-as-a-service adalah topik kontroversi.

Ada dua varietas utama SaaS:

SaaS Vertikal
Perangkat Lunak yang menjawab kebutuhan industri tertentu (misalnya, perangkat lunak untuk kesehatan, pertanian, real estat, industri keuangan)
SaaS Horisontal
Produk yang berfokus pada kategori perangkat lunak (pemasaran, penjualan, alat pengembang, SDM) tetapi agnostik industri.

Manfaat SAAS:

Ini menawarkan peluang besar bagi organisasi dari semua ukuran untuk mengalihkan risiko akuisisi perangkat lunak, dan untuk memindahkan TI dari pusat biaya reaktif menjadi bagian perusahaan yang proaktif dan menghasilkan nilai. Secara tradisional, menerapkan sistem perangkat lunak skala besar telah menjadi pekerjaan besar. Menyebarkan sistem ini di perusahaan besar membutuhkan biaya lebih banyak. Persyaratan waktu, staf, dan anggaran untuk penyebaran sebesar ini merupakan risiko yang signifikan bagi organisasi dengan ukuran apa pun, dan seringkali menempatkan perangkat lunak semacam itu di luar jangkauan organisasi yang lebih kecil yang jika tidak dapat memperoleh banyak manfaat darinya. kegunaan. Model pengiriman sesuai permintaan mengubah beberapa hal ini. Aplikasi SaaS tidak memerlukan penyebaran infrastruktur besar di lokasi klien.

Integrasi dapat direncanakan dan dilaksanakan dengan upaya minimal, menciptakan salah satu interval waktu tersingkat yang memungkinkan untuk investasi TI yang besar. Ini juga memungkinkan sejumlah vendor SaaS untuk menawarkan "test drive" perangkat lunak mereka yang bebas risiko (dan seringkali gratis ) untuk jangka waktu terbatas, seperti 30 hari. Memberi pelanggan kesempatan untuk mencoba perangkat lunak sebelum mereka membelinya membantu menghilangkan banyak risiko seputar pembelian perangkat lunak.

Bagaimana SaaS Mempengaruhi TI?

Setelah Anda membuat keputusan untuk mengejar SaaS, selanjutnya adalah mempersiapkan transisi dengan menilai bagaimana penerapan akan memengaruhi aset TI yang ada. Melakukan uji tuntas adalah bagian rutin dari setiap proyek penyebaran infrastruktur TI yang sukses. Beberapa area yang perlu diperhatikan dalam daftar periksa uji tuntas meliputi, Standar keamanan data : Memindahkan data bisnis penting “ke luar tembok” menimbulkan risiko kehilangan data atau pemaparan informasi sensitif secara tidak sengaja. Nilai kebutuhan keamanan data Anda, dan pastikan penyedia memiliki tindakan untuk memenuhi standar yang Anda tetapkan. Layanan pelaporan : Karena SaaS melibatkan penyerahan kontrol langsung atas beberapa data Anda, pelaporan yang akurat dan bermanfaat sangatlah penting. Tentukan layanan pelaporan apa yang ditawarkan penyedia, dan apakah layanan tersebut kompatibel dengan persyaratan intelijen bisnis Anda.

Dampak pada Peran dan Tanggung Jawab TI

Penambahan SaaS dapat menyebabkan perubahan mendasar pada peran departemen TI sebagai penyedia layanan informasi. Di masa lalu, sifat penyebaran perangkat lunak telah menempatkan kepala petugas informasi sebagai penjaga gerbang. Mereka dapat menggunakan hak veto dengan menyatakan bahwa mereka tidak akan menyimpannya di pusat data. Dengan SaaS , kendali pusat data tidak harus sama dengan kendali atas seluruh lingkungan komputasi perusahaan. Hal ini dapat menyebabkan penjaga gerbang takut kehilangan kendali.

Kesimpulan

Perusahaan sebaiknya mempertimbangkan fleksibilitas dan implikasi manajemen risiko dari penambahan SaaS ke portofolio layanan TI mereka. Integrasi dan komposisi adalah komponen penting dalam strategi arsitektur Anda untuk menggabungkan SaaS dengan sukses sebagai anggota yang berpartisipasi penuh dari infrastruktur TI Anda yang berpusat pada layanan. Kami percaya bahwa masa depan komputasi perusahaan tidak akan murni di tempat. Sebaliknya, mereka akan ada dalam harmoni simbiosis.

Referensi :
1. https://en.wikipedia.org/wiki/Software_as_a_service
2. https://msdn.microsoft.com/en-us/library/aa905332.aspx

## Apa itu Perangkat Lunak sebagai Arsitektur Layanan SaaS

![Gambar teks editor VS Code](https://www.devteam.space/wp-content/uploads/2018/06/image001.png)

Sebelum kita menyelami beberapa poin yang lebih terlibat, ada baiknya menyebutkan apa itu platform arsitektur SaaS.

SaaS adalah cara untuk mengirimkan perangkat lunak, penyedia perangkat lunak secara terpusat menghosting satu atau lebih aplikasi dan membuatnya tersedia untuk pelanggan melalui internet. Arsitektur SaaS juga merupakan salah satu pilar utama cloud computing. 

Ledakan komputasi Cloud, didorong oleh penyedia layanan cloud seperti Microsoft dengan Azure, Amazon Web Services (AWS), Oracle, dan IBM, telah melihat pertumbuhan produk dan layanan lain yang disampaikan melalui internet. Ini termasuk model SaaS berikut:

Infrastruktur sebagai Layanan
Platform sebagai Layanan
Pembelajaran Mesin sebagai Layanan
…dan banyak lagi!
Pembaruan atau tambalan apa pun ke aplikasi arsitektur SaaS semuanya ditangani oleh penyedia. Pelanggan tidak perlu mengunduh pemutakhiran atau menginstal ulang versi baru suatu produk karena perangkat lunak dikirimkan melalui internet.

Ini beroperasi sebagai arsitektur SaaS multi-penyewa di mana semua database dan templat yang relevan dengan pengguna berlisensi dapat diakses di mana pun lokasinya. 

Dengan penjelasan tentang metodologi SaaS dan perusahaan SaaS, mari kita lihat mengapa Anda mungkin ingin menggunakan produk perangkat lunak yang dirancang seperti ini.

## Bagaimana cara memulai aplikasi SaaS Anda?

Python adalah bahasa pemrograman yang banyak digunakan, dirancang untuk menekankan pada keterbacaan kodenya.

Python dapat melakukan banyak hal. Apa pun aplikasi web yang ingin Anda buat, kemungkinan ada kerangka kerja untuk itu dengan Python.

Kami di Usersnap memiliki cukup banyak pengalaman dengan Python sebelum menggunakannya untuk aplikasi web kami. Seperti yang disebutkan, fleksibilitasnya untuk berbagai kasus penggunaan adalah alasan lain bagi kami untuk menggunakan Python.

Python hebat dan pengembang kami menyukainya. Pengetikan dinamis, pemrograman meta, pembuatan prototipe cepat. Segalanya mungkin dengan Python.

Python adalah taruhan yang aman.

## DIAGRAM CLOUD
1. CREATELY (https://creately.com/id/lp/er-diagram-alat-online/) (https://creately.com/images/press-resources/creately-logo-dark-background.png)

Creately memiliki banyak kelebihan, kamu tidak perlu melakukan save secara manual, karena setiap perubahan yang kamu lakukan akan tersimpan secara otomatis di Google Drive. Selain itu, kamu juga bisa share diagram dan membuatnya bersama-sama secara langsung dengan rekanmu.

Template yang dimiliki Creately sangat beragam dan kamu dapat mencoba semuanya secara online sebelum kamu memutuskan untuk memilih paket berbayar. Versi cloud memiliki paket gratis yang sangat terbatas hingga 5 dokumen.

2. CACOO https://cacoo.com/ https://cacoo.com/assets/site/img/cacoo_ogp_en.png cacoo merupakan aplikasi pilihan lain yang lengkap. Cacoo menampilkan antarmuka pengguna yang sederhana dan beragam template. Aplikasi ini tidak mempunyai bentuk flowchart standar tapi ada template yang dapat kamu gunakan sebagai permulaan.Selain itu, aplikasi ini juga mempunyai fungsi bagan sederhana, yang memungkinkan pengguna untuk memasukkan atau menempelkan data dengan cepat untuk membuat grafik sederhana, diagram pie, dan trend.

## NON CLOUD
1. yED Graph Editor (https://static.macupdate.com/products/36897/l/yed-logo.png?v=1616135379)
aplikasi ini untuk membuat diagram-diagram yang biasa digunakan dalam perancangan sistem informasi seperti Flowchart,ER-D,DFD dan sebagainya Aplikasi ini tersedia untuk Windows,Linux dan juga MacOS.Selain itu aplikasi ini sangat mudah untuk pemula. Selain itu aplikasi ini juga menyediakan banyak sekali grafis serta kita dimudahkan untuk mewarnai pada setiap shape-shapenya.Diagram yang telah kita buat dapat diekspor ke format SWF,SVG,PDF,HTML,PNG dan sebagainya. (https://www.yworks.com/)

2. Pencil (https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQcP_3lr5CcYsBiuJoVpFQDZOJ8P8zjUOrRmw&usqp=CAU)
Aplikasi ini memiliki banyak bentuk bawaan untuk menggambar berbagai jenis antarmuka pengguna mulai dari desktop ke platform seluler di antaranya fitur shape, elemen flowchart, bentuk desktop/web UI, bentuk Android dan iOS GUI. Pencil juga mendukung pembuatan diagram, mengekspor ke berbagai format output termasuk Inkscape SVG dan Adobe PDF, dokumen teks OpenOffice/LibreOffice, dan penautan antar halaman. Tak hanya itu, Pencil juga terintegrasi dengan OpenClipart.org agar memudahkan mencari Cliparts di Internet.

(https://pencil.evolus.vn/)