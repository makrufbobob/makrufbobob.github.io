---
layout: post
title:  "Sistem Terdistribusi"
date:   2015-10-5 11:35:33
---
 
<h3><center>BAB I</center></h3>

<blockquote>
1. Apa itu sistem terdistribusi?<br>
2. Bagaimana hubungan antara jaringan komputer dengan sistem terdistribusi?<br>
   Apakah sama atau tidak?<br>
3. Apakah fungsi/manfaat dari sistem terdistribusi?<br>
4. Bagaimana karakter sistem terdistribusi?<br>
5. Model seperti apakah yang dapat kita implementasikan kedalam sistem terdistribusi?<br>
6. Kendala apakah yang akan kita hadapi dalam sistem terdistribusi?<br>
7. Sebutkan contoh-contoh sistem terdistribusi?
</blockquote>

<h4>1. Apa itu sistem terdistribusi?</h4>
Sistem Terdistribusi adalah Sekumpulan komputer otonom yang terhubung
ke suatu jaringan, dimana bagi pengguna sistem terlihat sebagai satu komputer.<br>
Maksud komputerotonomi adalah walaupun komputertidak terhubung
ke jaringan, komputer tersebut tetap data berjalan.<br>
Dengan menjalankan sistem terdistribusi, komputer dapat melakukan :<br>
1). Koordinasi Aktivitas<br>
2). Berbagi sumber daya : hardware, software dan data<br>
Dengan devinisi tersebut diatas maka internet sesungguhnya bukanlah suatu sistem terdistribusi, melainkan infrastruktur dimana sistem terdistribusi
dapat di aplikasikan pada jaringan tersebut.
<h4>2. Bagaimana hubungan antara jaringan komputer dengan sistem terdistribusi?
   Apakah sama atau tidak?</h4>
Hal yang paling mempengaruhi antara jaringan komputer dan sister terdistribusi adalah bukan pada letak perangkatnya melainkan dari softwarenya, baik dari OS maupun aplikasinya. karena perangkat lunaklah yang menentukan tingkat keterpaduan antara perangkat.<br>
jadi sebenarnya jaringan komputer dan sistem terdistribusi itu saling berkaitan karena sister terdistribusi ada sistem yang berada pada jaringan komputer. tetapi ada pula perbedaan dalam sistem yang di ambilnya baik dari jaringan komputer maupun dari sistem terdistribusi.
<br>

<h4>3. Apakah fungsi/manfaat dari sistem terdistribusi?</h4>
<ol>
<li>Data sharing   : mengijinkan pengguna untuk dapat mengakses data yang sama</li>
<li>Device sharing : mengijinkan pengguna untuk dapat mengakses perangkat keras yang sama</li>
<li>Communication  : mengijinkan pengguna untuk dapat malakukan komunikasi jauh lebih mudah</li>
<li>Fleksibility</li>
<ul><li>Membagi beban kerja pada perangkat yang tersedia dengan cara efektif</li>
<li>Dapat menambah komponen secara individu tanpa harus melakukan duplikasi sistem</li>
<li>Fasilitas local dapat disesuaikan  dengan kebutuhan local</li>
<li>Memungkinkan pertumbuhan sistem secara terus menerus</li>
<li>Susunan sistem bisa disesuaikan dengan pola organisasi perusahaan</li>
<li>Mamungkinkan beberapa bagian/local melakukan percobaan dan konsep baru untuk mengurangi resiko kegagalan sistem secara keseluruhan</li></ul>
<li>Multiuser computing : mengijinkan banyak user untuk melakukan akses dalam waktu yang bersamaan</li></ol>


<h4>4. Bagaimana karakter sistem terdistribusi?</h4>
<ul>Sistem Terdistribusi adalah sistem <i>concurrent</i>
<li>Setiap komponen hardware/software ersifat otonom (proses)</li>
<li>Komponen menjalankan tugas bersamaan</li>
<li>Sinkronisasi dan koordinasi dengan message passing</li></ul>
<ul>Masalah umum dalam sistem concurrent
<li>Deadlock</li>
<li>Lifelock</li>
<li>Komunikasi yang tidak handal</li></ul>
<ul>independen failure
<li>Kemungkinan adanya kegagalan proses tunggal yang tidak diketahui</li>
<li>Proses tunggal mungkin tidak peduli pada kegagalan sistem keseluruhan</li></ul>
<h4>5. Model seperti apakah yang dapat kita implementasikan kedalam sistem terdistribusi?</h4>
<strong>1. Model Client Server</strong><br>

Sistem client-server mempunyai satu atau lebih proses client dan satu atau lebih proses server, dan sebuah proses client dapat mengirim query ke sembarang proses server. Client bertanggung jawab pada antar muka untuk user, sedangkan server mengatur data dan mengeksekusi transaksi. Sehingga suatu proses client berjalan pada sebuah personal computer dan mengirim query ke sebuah server yang berjalan pada mainframe.<br>
Arsitektur ini menjadi sangat popular untuk beberapa alasan. Pertama, implementasi yang relatif sederhana karena pembagian fungsi yang baik dan karena server tersentralisasi. Kedua, mesin server yang mahal utilisasinya tidak terpengaruh pada interaksi pemakai, meskipun mesin client tidak mahal. Ketiga, pemakai dapat menjalankan antarmuka berbasis grafis sehingga pemakai lebih mudah dibandingkan antar muka pada server yang tidak user-friendly. perlu diingat batasan antara client dan server dan untuk menjaga komunikasi antara keduanya yang berorientasi himpunan. Khususnya membuka kursor dan mengambil tupel pada satu waktu membangkitkan beberapa pesan dan dapat diabaikan.
<br><br>

<strong>2. Model Proxy Server</strong><br>

Proxy server menyediakan hasil copy (replikasi) dari resource yang di atur oleh server lain. Biasa nya proxy server di pakai untuk menyimpan hasil copy web resources. Ketika client melakukan request ke server, hal yang pertama dilakukan adalah memeriksa proxy server apakah yang diminta oleh client terdapat pada proxy server. Proxy server dapat diletakkan pada setiap client atau dapat di pakai bersama oleh beberapa client. Tujuannya adalah meningkatkan performance dan availibity dengan mencegah frekwensi akses ke server.<br><br>

<strong>3. Model Peer To Peer</strong><br>

Bagian dari model sistem terdistribusi dimana sistem dapat sekaligus berfungsi sebagai client maupun server. Sebuah arsitektur dimana tidak terdapat mesin khusus yang melayani suatu pelayanan tertentu atau mengatur sumber daya dalam jaringan dan semua kewajiban dibagi rata ke seluruh mesin, yang dikenal sebagai peer. Pola komunikasi yang digunakan berdasarkan aplikasi yang digunakan. Peer-to-peer merupakan model yang paling general dan fleksible.<br><br>

<h4>6. Kendala apakah yang akan kita hadapi dalam sistem terdistribusi?</h4>
<ol><li>Bagaimana kita merancang dan mengatur software yang tepat dalam distribusi sistem.</li>
	<li>Ketergantungan pada jaringan infrastruktur sangat memperngaruhi sistem terdistribusi bila tidak direncanakan dengan baik hal ini dapat menimbulkan gangguan-gangguan yang diakibatkan bentuk infrastruktur yang kurang baik sehingga menggangu dari kinerja sistem tersebut.
	Secara umum masalah infrastruktur jaringan sering terjadi, namun dengan perencanaan yang baik permasalahan ini sangat mudah untuk dicari sumber kesalahannya dan memudahkan proses peraikan.</li>
	<li>Kemudahan akses kedata yang dishare, memunculkan masalah keamanan.</li>
	<li>Sistem Terdistribusi sangat dipengaruhi oleh jaringan komputer. Permasalahan akan timbul jika suatu jaringan sistem tersebut tidak aman, Dimana tidak terdapat firewall atau proteksi terhadap data didalam jaringan tersebut. Firewall dapat digunakan untuk menentukan host mana yang dapat mengakses data atau memberi batasan terhadap host dalam mengakses data sedangkan proteksi terhadap data dilakukan dengan pengguanaan password atau enkripsi, namun hal ini tidak menjamin data tersebut dalam keadaan aman.</li></ol>

<h4>7. Sebutkan contoh-contoh sistem terdistribusi?</h4>
<ol><li>Sistem Telepon seperti ISDN, PSTN</li>
	<li>Manajemen Jaringan seperti Administrasi sesumber jaringan</li>
	<li>Network File System (NFS) Seperti Arsitektur untuk mengakses sistem file melalui jaringan</li>
</ol>