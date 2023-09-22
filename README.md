## Praktikum Modul 1 Jaringan Komputer

**Kelompok A16 :**

| Nama | NRP |
| ----------- | ----------- |
| Clarissa Luna Maheswari | 5025211033 |
| Heru Dwi Kurniawan | 5025211055 |

   
### Soal 1

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/dbc3e690-b9a9-4a8d-8d9c-4dfd947936aa)

User melakukan berbagai aktivitas dengan menggunakan protokol FTP

**Penyelesaian**

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/67e89770-15f6-4da2-886a-b0590da6d49f)

Melakukan filtering dengan menuliskan perintah FTP, bertujuan agar memfilter protokol FTP saja sesuai soal yang diminta.


![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/b0ff7d38-6e12-4ca5-8d5e-ee4165f12c7a)

Selanjutnya klik info untuk mendapatkan response, scroll dan temukan Perintah STOR dengan tujuan untuk meng-upload file ke FTP Server. 


![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/4c9d252e-6c23-4bd2-b52d-61f15938da2d)

didapatkan Sequence Number ( raw ) dan acknowledgment number ( raw) untuk request


![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/3e589970-abd8-4c04-a8dc-fe2d1a33b7e0)

dan didapatkan Sequence Number ( raw ) dan acknowledgment number ( raw) untuk response


![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/e1a2bf67-453b-4d8c-83e7-e1719ca864ae)


## Soal 2

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/d307835f-28d7-4332-839f-49c2551f3faa)

**Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer! nc 10.21.78.111 13579**

**Penyelesaian**

Pada soal no 2 kita di suruh mencari web server yang digunakan portal praktikum jaringan komputer.

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/8ccdff2a-e3bf-41b1-96ca-728f815d8f59)

Lakukan filter http yang bertujuan untuk mendapatkan web server.

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/d4c559e2-97f7-4051-9309-fc846f347767)   

Setelah kefilter klik kanan di protokol kttp => kemudian tekan follow => http stream ( bertujuan untuk mendapatkan server )

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/3d5f7d1c-609e-4c62-b92c-ae8a4c996e57)

kemudian didapatkan server **gunicorn**

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/e9e46503-6e7f-4cb4-82df-473e6591e147)


3\. **Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut: nc 10.21.78.111 13590**

1. **Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?**
       1.
   ```bash
   filter (ip.src == 239.255.255.250 || ip.dst == 239.255.255.250) && udp.port == 3702
   ```
   check ip.src atau ip.dst benar atau bukan dan check port udp

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


## Soal 9


![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/0c8bfa33-0110-489a-a1bc-b42354c59547)

Berikut kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1. tetapi tidak menuju ke alamat 10.39.55.34  

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/ad432c87-99f9-4c3f-8898-b2d1448c4e7b)

``` bash
Seperti contoh di github bahwa ip.src == 192.168.0.1 or ip.dst == 192.168.0.1
```

( Menampilkan semua paket yang berasal dari alamat 192.168.0.1 atau menuju ke alamat 192.168.0.1 ). 

untuk soal no 9 diperintahkan untuk mengambil paket yang berasal dari alamat 10.51.40.1. bisa menggunakan **ip.src == 10.51.40.1**. 

Kemudian untuk mengambil paket tetapi tidak menuju ke alamat 10.39.55.34! bisa menggunakan **ip.dst != 10.39.55.34**. 

Sehingga untuk kuerinya **ip.src == 10.51.40.1 && ip.dst != 10.39.55.34 ( && maksutnya untuk memenuhi 2 kondisi ).**

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/8a05bfa2-e997-435e-a6c6-fb028892dc8f)


**10. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet! nc 10.21.78.111 7373**

1. filter by telnet

1. password ketemu di dua paket
1. follow streamnya dan ketemu usernamenya juga






