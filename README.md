**Jaringan Komputer A**

**Kelompok A16 :**

1. Clarissa Luna Maheswari - 5025211003
1. Heru Dwi Kurniawan - 5025211055

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/dbc3e690-b9a9-4a8d-8d9c-4dfd947936aa)

Soal no 1: User melakukan berbagai aktivitas dengan menggunakan protokol FTP


Melakukan filtering dengan menuliskan perintah FTP, bertujuan agar memfilter protokol FTP saja sesuai soal yang diminta.


Selanjutnya klik info untuk mendapatkan response, scroll dan temukan Perintah STOR dengan tujuan untuk meng-upload file ke FTP Server. 


didapatkan Sequence Number ( raw ) dan acknowledgment number ( raw) untuk request



dan didapatkan Sequence Number ( raw ) dan acknowledgment number ( raw) untuk response



2\.  **Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer! nc 10.21.78.111 13579**




Sebutkan web server yang digunakan pada portal praktikum jaringan komputer !

Pada soal no 2 kita di suruh mencari web server yang digunakan portal praktikum jaringan komputer. 

Lakukan filter http yang bertujuan untuk mendapatkan web server.



Setelah kefilter klik kanan di protokol kttp => kemudian tekan follow => http stream ( bertujuan untuk mendapatkan server )

kemudian didapatkan server **gunicorn**



3\. **Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut: nc 10.21.78.111 13590**

1. **Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?**
       1. filter (ip.src == 239.255.255.250 || ip.dst == 239.255.255.250) && udp.port == 3702 -> check ip.src atau ip.dst benar atau bukan dan check port udp

2\. check berapa yang terdisplay

1. **Protokol layer transport apa yang digunakan?**
   udp -> 

4\. **Berapa nilai checksum yang didapat dari header pada paket nomor 130? nc 10.21.78.111 13591**

1. klik paket no 130
1. di bagian user datagram protocol, terdapat checksum dan nilainya

5\. **Elshe menemukan suatu file packet capture yang menarik. Bantulah elshe untuk menganalisis file packet capture tersebut.
a. berapa packet yang berhasil dicapture dari file?** 60**


**b. port berapa server yang digunakan untuk service smtp?**


**c. berapa public ip?**
ketika ditrace/difollow, ip 74.53.140.153 smtp dan mengirim pesan/mail**


6\. PESAN TERSEMBUNYI: Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. nc 10.21.78.111 6666

**7. Berapa jumlah packet yang menuju IP 184.87.193.88? nc 10.21.78.111 6565**

1. filter paket

1. jumlah ada di kanan bawah

8\. **Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)! nc 10.21.78.111 7171**

1. filter tcp.dstport == 80 || udp.dstport == 80

mencakup semua paket yang menuju ke port tcp 80. diurutkan sesuai abjad apabila lebih dari satu port**


9\. 


Berikut kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1. tetapi tidak menuju ke alamat 10.39.55.34  



` `Seperti contoh di github bahwa ip.src == 192.168.0.1 or ip.dst == 192.168.0.1 ( Menampilkan semua paket yang berasal dari alamat 192.168.0.1 atau menuju ke alamat 192.168.0.1 ). 

untuk soal no 9 diperintahkan untuk mengambil paket yang berasal dari alamat 10.51.40.1. bisa menggunakan **ip.src == 10.51.40.1**. Kemudian untuk mengambil paket tetapi tidak menuju ke alamat 10.39.55.34! bisa menggunakan **ip.dst != 10.39.55.34**. Sehingga untuk kuerinya **ip.src == 10.51.40.1 && ip.dst != 10.39.55.34 ( && maksutnya untuk memenuhi 2 kondisi ).**



**10. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet! nc 10.21.78.111 7373**

1. filter by telnet

1. password ketemu di dua paket
1. follow streamnya dan ketemu usernamenya juga






