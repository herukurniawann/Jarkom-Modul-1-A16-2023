## Praktikum Modul 1 Jaringan Komputer

**Kelompok A16 :**

| Nama | NRP |
| ----------- | ----------- |
| Clarissa Luna Maheswari | 5025211033 |
| Heru Dwi Kurniawan | 5025211055 |
   jsjjsjs
### Soal 1
**User melakukan berbagai aktivitas dengan menggunakan protokol FTP**
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/dbc3e690-b9a9-4a8d-8d9c-4dfd947936aa)

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

### Soal 2
**Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer! nc 10.21.78.111 13579**
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/d307835f-28d7-4332-839f-49c2551f3faa)
**Penyelesaian**
Pada soal no 2 kita diperintahkan untuk mencari web server yang digunakan portal praktikum jaringan komputer.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/8ccdff2a-e3bf-41b1-96ca-728f815d8f59)
Lakukan filter http yang bertujuan untuk mendapatkan web server.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/d4c559e2-97f7-4051-9309-fc846f347767)   
Setelah kefilter klik kanan di protokol kttp => kemudian tekan follow => http stream ( bertujuan untuk mendapatkan server )
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/3d5f7d1c-609e-4c62-b92c-ae8a4c996e57)
kemudian didapatkan server **gunicorn**
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/e9e46503-6e7f-4cb4-82df-473e6591e147)
### Soal 3
**Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut: nc 10.21.78.111 13590**
1. **Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?**
       1.
   ```bash
   filter (ip.src == 239.255.255.250 || ip.dst == 239.255.255.250) && udp.port == 3702
   ```
   check ip.src atau ip.dst benar atau bukan dan check port udp

2\. check berapa yang terdisplay
1. **Protokol layer transport apa yang digunakan?**
   udp ->
### Soal 4
**Berapa nilai checksum yang didapat dari header pada paket nomor 130? nc 10.21.78.111 13591**
1. klik paket no 130
1. di bagian user datagram protocol, terdapat checksum dan nilainya

### Soal 5
**Elshe menemukan suatu file packet capture yang menarik. Bantulah elshe untuk menganalisis file packet capture tersebut.**
a. Berapa packet yang berhasil dicapture dari file? 60
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/e5e10f4c-0fd5-431d-b870-11ad162251f9)
Jumlah paket terpapar di bagian bawah wireshark.
b. Port berapa server yang digunakan untuk service smtp? 25
Karena Public IP server adalah 74.53.140.153 berdasarkan info yang tertulis sedangkan IP 10.10.1.4 adalah IP dari user (terlihat dari aktivitas mulai dari memasukkan login dan password), sehingga klik salah satu paket yang sourcenya adalah 74.53.140.153 (berasal dari server).
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/69814b4a-4f08-4684-84f4-868311c8d59a)
Cek di bagian Transmission Control Protcol dan terlihat bahwa source portnya adalah 25.
c. Berapa public ip? 74.53.140.153
Public IP adalah 74.53.140.153 karena dari alamat ip ini terdapat beberapa kode status yang biasanya digunakan ke server web seperti angka "220", "250", "334", dan lainnya.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/c2f12f6a-86e3-415d-b700-b6a20830e26e)
Hal ini terlihat dapat dilihat di TCP Stream pada paket-paket dengan protokol SMTP (Simple Mail Transfer Protocol).

**Kendala yang dialami**: Tidak ada kendala dalam pengerjaan soal ini.

### Soal 6
PESAN TERSEMBUNYI: Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. nc 10.21.78.111 6666

**Penyelesaian**
1. Filter untuk frame nomor 7812
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/d78ab16c-f9c5-4d08-b65f-50da66d31c5e)
2. Pada soal dinyatakan bahwa source address 7812 invalid, ditemukan bahwa source address paket 7812 adalah 104.18.14.101
3. Hasil pencarian yang menampilkan a1 e5 u21 menunjukkan bahwa terdapat cipher sederhana. Dimana huruf A disubstitusi dengan angka 1, huruf e digantikan dengan angka 5, dan seterusnya
4. Sesuai dengan clue kapital SUBSTITUSI, angka yang tertera pada IP yaitu 104 18 14 101 di-decrypt dimana ditunjukkan bahwa hasilnya adalah JD R N JA
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/07a92d09-3d33-494d-9a90-0ca98ef28a8b)


**Kendala yang dialami**: Pada proses praktikum vpn cukup lambat, kurangnya waktu menyempitkan kesempatan untuk menjawab soal ini. Solusi baru ditemukan setelah praktikum selesai. 

### Soal 7
Berapa jumlah packet yang menuju IP 184.87.193.88? nc 10.21.78.111 6565**
**Penyelesaian**
Dilakukan filter pada paket-paket yang menuju IP 184.87.193.88.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/1ba8c1b9-9997-40f3-bc5e-42c91f7f65d0)
Dari proses filter ini, jumlah paket terpampang pada bagian bawah wireshark, tepatnya di sebelah kiri profile
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/ab1d6912-debe-4d12-8f4e-2a8727abb266)


**Kendala yang dialami**: Tidak ada kendala dalam pengerjaan soal ini.

### Soal 8
**Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)! nc 10.21.78.111 7171**

Dilakukan filter untuk mengambil semua protokol paket yang menuju port 80.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/947989bd-9355-41fb-8feb-ae2cb93083c6)
Filter tersebut mencakup semua paket baik paket dengan protokol transport TCP dan UDP.

**Kendala yang dialami**: Tidak ada kendala dalam pengerjaan soal ini.

### Soal 9
**Berikut kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1. tetapi tidak menuju ke alamat 10.39.55.34**

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/0c8bfa33-0110-489a-a1bc-b42354c59547)

**Penyelesaian**

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/ad432c87-99f9-4c3f-8898-b2d1448c4e7b)

``` bash
Seperti contoh di github bahwa ip.src == 192.168.0.1 or ip.dst == 192.168.0.1
```

( Menampilkan semua paket yang berasal dari alamat 192.168.0.1 atau menuju ke alamat 192.168.0.1 ). 

untuk soal no 9 diperintahkan untuk mengambil paket yang berasal dari alamat 10.51.40.1. bisa menggunakan **ip.src == 10.51.40.1**. 

Kemudian untuk mengambil paket tetapi tidak menuju ke alamat 10.39.55.34! bisa menggunakan **ip.dst != 10.39.55.34**. 

Sehingga untuk kuerinya **ip.src == 10.51.40.1 && ip.dst != 10.39.55.34 ( && maksutnya untuk memenuhi 2 kondisi ).**

![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/93961310/8a05bfa2-e997-435e-a6c6-fb028892dc8f)

### Soal 10
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet! nc 10.21.78.111 7373**
**Penyelesaian**
1. Paket difilter berdasarkan Protokol Telnet.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/01c21d18-dbd9-45ad-a2dc-13654a6e576e)
2. Bagian yang memberikan petunjuk kredensial (contoh: login, password) dicaari pada hasil pemfilteran.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/4ffc6a4f-3d69-4a6e-85a4-a671c12f85c1)
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/e8e2ddfd-2b66-46e9-a302-cf69b149c742)
3. Stream di Paket tersebut dilacak hingga menemukan petunjuk kredensial lainnya.
![image](https://github.com/herukurniawann/Jarkom-Modul-1-A16-2023/assets/121850356/a39a9bf0-6381-461f-a399-8231bf06a8cd)


**Kendala yang dialami**: Tidak ada kendala dalam pengerjaan soal ini.





