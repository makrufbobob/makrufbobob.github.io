---
layout: post
title:  "Sistem Terdistribusi BAB I"
date:   2015-10-05 11:35:33
---
 
###<center>BAB I</center>

>
1. Apa itu Sistem Terdistribusi?
2. Bagaimana hubungan antara Jaringan Komputer dengan Sistem Terdistribusi?
   Apakah sama atau tidak?
3. Apakah fungsi/manfaat dari Sistem Terdistribusi?
4. Bagaimana karakter Sistem Terdistribusi?
5. Model seperti apakah yang dapat kita implementasikan kedalam Sistem Terdistribusi?
6. Kendala apakah yang akan kita hadapi dalam Sistem Terdistribusi?
7. Sebutkan contoh-contoh Sistem Terdistribusi?

>####1. Apa itu Sistem Terdistribusi?

Sistem Terdistribusi adalah sekumpulan komputer otonom yang terhubung
ke suatu jaringan, dimana bagi pengguna sistem terlihat sebagai satu komputer.

Maksud komputer otonomi adalah walaupun komputer tidak terhubung
ke jaringan, komputer tersebut tetap dapat berjalan.

Dengan menjalankan Sistem Terdistribusi, komputer dapat melakukan :

- Koordinasi Aktivitas,
- Berbagi sumber daya : hardware, software dan data.

Dengan devinisi tersebut diatas maka internet sesungguhnya bukanlah suatu Sistem Terdistribusi, melainkan infrastruktur dimana Sistem Terdistribusi dapat di aplikasikan pada jaringan tersebut.

>####2. Bagaimana hubungan antara Jaringan Komputer dengan Sistem Terdistribusi?
Apakah sama atau tidak?

Hal yang paling mempengaruhi antara jaringan komputer dan sister terdistribusi adalah bukan pada letak perangkatnya melainkan dari softwarenya, baik dari OS maupun aplikasinya. karena perangkat lunaklah yang menentukan tingkat keterpaduan antara perangkat.

jadi sebenarnya jaringan komputer dan sistem terdistribusi itu saling berkaitan karena sister terdistribusi ada sistem yang berada pada jaringan komputer. tetapi ada pula perbedaan dalam sistem yang di ambilnya baik dari jaringan komputer maupun dari sistem terdistribusi.

>####3. Apakah fungsi/manfaat dari Sistem Terdistribusi?

- Data sharing   : Mengijinkan pengguna untuk dapat mengakses data yang sama.
- Device sharing : Mengijinkan pengguna untuk dapat mengakses perangkat keras yang sama.
- Communication  : Mengijinkan pengguna untuk dapat malakukan komunikasi jauh lebih mudah.
- Fleksibility   : 
 - Membagi beban kerja pada perangkat yang tersedia dengan cara efektif.
 - Dapat menambah komponen secara individu tanpa harus melakukan duplikasi sistem.
 - Fasilitas local dapat disesuaikan  dengan kebutuhan local.
 - Memungkinkan pertumbuhan sistem secara terus menerus.
 - Susunan sistem bisa disesuaikan dengan pola organisasi perusahaan.
 - Mamungkinkan beberapa bagian/local melakukan percobaan dan konsep baru untuk mengurangi resiko kegagalan sistem secara keseluruhan.
- Multiuser computing : mengijinkan banyak user untuk melakukan akses dalam waktu yang bersamaan.

>####4. Bagaimana karakter Sistem Terdistribusi?

- Sistem Terdistribusi adalah sistem *concurrent*
 - Setiap komponen hardware/software ersifat otonom (proses)
 - Komponen menjalankan tugas bersamaan
 - Sinkronisasi dan koordinasi dengan message passing
- Masalah umum dalam sistem *concurrent*
 - *Deadlock*
 - *Lifelock*
 - Komunikasi yang tidak handal
- *independen failure*
 - Kemungkinan adanya kegagalan proses tunggal yang tidak diketahui
 - Proses tunggal mungkin tidak peduli pada kegagalan sistem keseluruhan

>####5. Model seperti apakah yang dapat kita implementasikan kedalam sistem terdistribusi?

**1. Model Client Server**

Sistem *client-server* mempunyai satu atau lebih proses client dan satu atau lebih proses server, dan sebuah proses client dapat mengirim query ke sembarang proses server. Client bertanggung jawab pada antar muka untuk user, sedangkan server mengatur data dan mengeksekusi transaksi. Sehingga suatu proses client berjalan pada sebuah personal computer dan mengirim query ke sebuah server yang berjalan pada mainframe.

Arsitektur ini menjadi sangat popular untuk beberapa alasan. Pertama, implementasi yang relatif sederhana karena pembagian fungsi yang baik dan karena server tersentralisasi. Kedua, mesin server yang mahal utilisasinya tidak terpengaruh pada interaksi pemakai, meskipun mesin client tidak mahal. Ketiga, pemakai dapat menjalankan antarmuka berbasis grafis sehingga pemakai lebih mudah dibandingkan antar muka pada server yang tidak *user-friendly*. perlu diingat batasan antara client dan server dan untuk menjaga komunikasi antara keduanya yang berorientasi himpunan. Khususnya membuka kursor dan mengambil tupel pada satu waktu membangkitkan beberapa pesan dan dapat diabaikan.

**2. Model Proxy Server**

Proxy server menyediakan hasil copy (replikasi) dari resource yang di atur oleh server lain. Biasa nya proxy server di pakai untuk menyimpan hasil copy web resources. Ketika client melakukan request ke server, hal yang pertama dilakukan adalah memeriksa proxy server apakah yang diminta oleh client terdapat pada proxy server. Proxy server dapat diletakkan pada setiap client atau dapat di pakai bersama oleh beberapa client. Tujuannya adalah meningkatkan performance dan availibity dengan mencegah frekwensi akses ke server.

**3. Model Peer To Peer**

Bagian dari model sistem terdistribusi dimana sistem dapat sekaligus berfungsi sebagai client maupun server. Sebuah arsitektur dimana tidak terdapat mesin khusus yang melayani suatu pelayanan tertentu atau mengatur sumber daya dalam jaringan dan semua kewajiban dibagi rata ke seluruh mesin, yang dikenal sebagai peer. Pola komunikasi yang digunakan berdasarkan aplikasi yang digunakan. Peer-to-peer merupakan model yang paling general dan fleksible.

>####6. Kendala apakah yang akan kita hadapi dalam Sistem Terdistribusi?

- Bagaimana kita merancang dan mengatur software yang tepat dalam distribusi sistem.
- Ketergantungan pada jaringan infrastruktur sangat memperngaruhi sistem terdistribusi bila tidak direncanakan dengan baik hal ini dapat menimbulkan gangguan-gangguan yang diakibatkan bentuk infrastruktur yang kurang baik sehingga menggangu dari kinerja sistem tersebut.
Secara umum masalah infrastruktur jaringan sering terjadi, namun dengan perencanaan yang baik permasalahan ini sangat mudah untuk dicari sumber kesalahannya dan memudahkan proses peraikan.
- Kemudahan akses kedata yang dishare, memunculkan masalah keamanan.
- Sistem Terdistribusi sangat dipengaruhi oleh jaringan komputer. Permasalahan akan timbul jika suatu jaringan sistem tersebut tidak aman, Dimana tidak terdapat firewall atau proteksi terhadap data didalam jaringan tersebut. Firewall dapat digunakan untuk menentukan host mana yang dapat mengakses data atau memberi batasan terhadap host dalam mengakses data sedangkan proteksi terhadap data dilakukan dengan pengguanaan password atau enkripsi, namun hal ini tidak menjamin data tersebut dalam keadaan aman.

>####7. Sebutkan contoh-contoh Sistem Terdistribusi?

- Sistem Telepon seperti ISDN, PSTN
- Manajemen Jaringan seperti Administrasi sesumber jaringan.
- *Network File System* (NFS) Seperti Arsitektur untuk mengakses sistem file melalui jaringan.