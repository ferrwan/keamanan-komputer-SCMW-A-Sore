## Setup
1. Buka git bash
2. CD ke directory folder yang anda inginkan
3. Git clone dengan command ```git clone https://github.com/ferrwanz/keamanan-komputer-SCMW-A-Sore.git ```
4. cd ke dalam folder ```cd keamanan-komputer-SCMW-A-Sore```
5. Edit file README.md dengan editor anda. Copy text dari Nama - NIM sampai "- - - -" kemudian paste kan dibawahnya (Ingat untuk enter 1 line sebelum "- - - -". 1 line kosong adalah enter dalam file .md ini). Cukup edit pada bagian Nama - NIM, Nama Layer, dan kata - kata setelah 'titik-dua' (: )
6. Siap edit, git add dengan command ```git add README.md```
7. Commit sesuai dengan deskripsi anda ```git commit -m "Deskripsi yang sesuai kerjaan anda"```
8. Silahkan push ```git push origin master```. Masukkan username dan password anda.
9. Bila ada conflict ketika push. Silahkan git pull dulu dengan command ```git pull origin master```
10. Bila ada conflict dalam pull, silahkan git merge ```git merge```
11. Apabila bingung dengan git merge, maka pakai branch baru saja dengan command ```git checkout -b new-branch-name```. Nanti akan saya merge-kan.
12. Git susah? Tidak. Hanya kurang pengalaman memakai saja.

Mohon untuk tidak sembarangan mengupload, mengubah dan menghapus file ataupun hasil kerja teman - teman lain ya. Thanks

- - - -

## Name - NIM Here

### 1. Layer Name Here

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Finger Of Death
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: C atau I atau A (Terserah)
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Memberikan magic damage terhadap lawan sebesar 800 damage
* Counter Measure/Prevent &nbsp;: Memakai BKB, Pipe of Insight

### 2. Layer Name Here

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Kuota Habis
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: C atau I atau A (Terserah)
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Tidak bisa menghubungkan client ke server untuk bermain DotA
* Counter Measure/Prevent &nbsp;: Connect WiFi / Hotspot teman or tempat publik, Beli Kuota Bung !

- - - - 

## Denny Ho - 14.111.0191

### 1. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Cross-Site_Request_Forgery
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: C
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Sebuah penyerangan yang memaksa user untuk submit data ke website yang user sedang login misalnya ketika login pada website perbankan user dipaksa untuk transfer uang. Cross site request forgery dapat dipadukan dengan XSS (cross site scripting) yang melakukan submit data otomatis dengan script yang diberi.
* Counter Measure/Prevent &nbsp;: Menggunakan CSRF Token

### 2. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Regex Denial of Services
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: A
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerangan terhadap service yang memiliki validasi dengan regex yang mengandung "evil regex (misalnya (.*a){x} | for x > 10 ) yang rentan terhadap inputan aaaaaaaaaaaaaaaaaaaaaaaa! dimana terdapat 65536 jalur yang ada dalam mengeceknya via evil regex tersebut)" 
* Counter Measure/Prevent &nbsp;: 

   - Memastikan regex yang digunakan bukan merupakan evil regex.
   - Pastikan membatasi inputan jika memungkinkan.

- - - - 

## Willy - 14.111.0311

### 1. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Session Hijacking 
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: C
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Salah satu metode dalam session hijacking adalah  : Session fixation , dimana penyerang ini menempatkan suatu session-id yang diketahui si target lalu si penyerang hanya menunggu target untuk melakukan akses login sehingga penyerang ini mengetahui segala info yang dimiliki oleh si target saat login.
* Counter Measure/Prevent &nbsp;:
    1. Menggunakan Enskripsi pada jalur data diantara kedua pihak yang berkomunikasi dengan menggunakan SSL/TLS. 
    2. Menggunakan sebuah angka random string pada session.


### 2. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Fraggle Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: A
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Fraggle Attack merupakan variasi serangan Distribute Denial Of Service ( DDOS ) dimana penyerang memalsukan alamat sumber lalu mengirimkan flooding berupa paket data yang besar dan banyak melalui jalur UDP kepada 7 port (Echo Protocol) dan 19 port (Charater Generator Protocol) pada alamat IP Broadcast.  
* Counter Measure/Prevent &nbsp;: Untuk mencegah penyerangan ini sejauh ini masih tidak ada caranya , hanya ada cara meringankan penyerangan ini berupa :
    1. Mengkonfigurasi host individu dan router untuk tidak menanggapi permintaan ICMP atau Broadcast.
    2. Mengkonfigurasi router untuk tidak meneruskan paket yang diarahkan untuk alamat Broadcast.

- - - - 

## Christopher Ganda - 14.111.3368

### 1. Network Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : ICMP Flooding
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: A
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: penyerangan pada layer 3 dengan infrastruktur metode penyerangan DDoS yang menggunakan ICMP untuk mengoverload bandwith dari target yang akan diserang. Biasa ping digunakan untuk mengecek konektifitas antara 2komputer dengan cara request ICMP dikirim dan komputer target membalas balik dengan ICMP pula.ICMP flooding bekerja dengan mengirimkan request tersebut(ping) secepat mungkin tanpa menunggu komputer target mereply/membalas sehingga terjadi overloading pada jaringan target.
* Counter Measure/Prevent &nbsp;: Dengan membatasi limit dari traffic ICMP atau biasa disebut dengan ICMP flood protection.Satuan traffic yang digunakan adalah packets per second(pps)

### 2. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : SIP Malformed Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: A
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerangan yang terjadi pada Session Initiation Protocol(SIP) pada service VoIP.Penyerangan DDoS ini menyerang server SIP. Penyerang mengirim pesan-pesan malformed yang tidak valid untuk mencari celah yang dapat masuk ke sistem SIP sehingga tidak dapat di generate oleh protokol standar SIP. 
* Counter Measure/Prevent &nbsp;: Menggunakan algoritma-algoritma yang dapat memvalidasi pesan-pesan invalid tersebut

- - - - 

## Kenedy Lukito - 14.111.0043

### 1. Data Link Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : MAC Address alteration and MAC Flooding attacks
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Perangkat jaringan yang terkena serangan MAC flooding, semua resource CPU akan seperti tersedot. Dengan MAC Address alteration, laju lalu lintas jaringan dapat diubah dengan mudah. Serangan MAC Flooding menyebabkan terjadinya overflow pada MAC table di switch. Switch akan melambat dan bisa menyebabkan crash
* Counter Measure/Prevent &nbsp;: Dengan mengunakan fungsi dari port-security yang disediakan oleh Cisco ISO

### 2. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : TCP,UDP flooding attacks
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Ancaman ini menyerang dengan mengirimkan traffic UDP yang sangat banyak ke target tertentu atau melakukan request TCP 3 way handshaking setelah mengganti IP addressnya. Akibatnya akan menyebabkan kerusakan pada perangkat networking dan server akan mengalami kelebihan muatan.
* Counter Measure/Prevent &nbsp;: Dengan menggunakan SYN cookies
>>>>>>> a7dc462d145e32dff7ff45495ad7ac4ec16f3092

- - - - 

### Kelvin Angviesta - 14.111.1511

### 1. Network Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Fake Access Point
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentialty
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: melakukan pencurian hak akses oleh sebuah AP untuk dapat tergabung kedalam sebuah jaringan wireless dan ikut melayani para penggunanya, akses ini disebabkan karena AP palsu mendapakan SSID dari jaringan tersebut dan melakukan broadcast SSID, Selain itu AP juga bisa memalsukan alamat MAC. 
* Counter Measure/Prevent &nbsp;: Menyembunyikan SSID,Mengunci WEP,Menggunakan MAC Filtering dan Captive Portal

### 2. Transport layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Smurf Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Broadcast ping yang terkirim dan sumber IP terlihat sama dengan IP address korban. Komputer akan merespon balik dan mengirim dan akan mengirim Ping Reply ke korban secara terus-menerus, sampai mesin korban atau link mengalami overload dan dalam kondisi Denial of Service.
* Counter Measure/Prevent &nbsp;: Menggunakan Shorewall

- - - - 

### Ferry Irawan - 14.111.0507

### 1. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Slow-Rate Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Mengirimkan paket - paket kecil kepada sebuah website dimana dengan mengirimkan paket seperti permitaan HTTP POST yang sah dengan 'content-length' yang panjangnya tidak normal pada field header dalam tingkat yang lambat. Penyerangan ini akan menguras connection table server dan membuat server tersebut crash
* Counter Measure/Prevent &nbsp;: Dengan me-monitoring resource server seperti connection table, server Memory dan CPU dan rangkaian aplikasi untuk mengidentifikasi penyalahgunaan resource

### 2. Presentation Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Zeus (Malware)
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Mencuri data - data orang khususnya data berupa informasi bank melalui Man-in-the-browser, keystroke logging (menangkap apa saja yang ditekan pada keyboard) dan form grabbing (mengambil data autorisasi dari form) dan bisa menginstallkan CryptoLocker ransomware. Kebanyakan terjadi pada Windows
* Counter Measure/Prevent &nbsp;: Menggunakan antivirus yang bisa mendeteksi Malware, tetapi Zeus tidak mudah untuk dideteksi karena bisa menyembunyikan dirinya dengan Stealth Techniques. Cara pencegahan yang utama adalah dengan mengajarkan atau melatih para staff (untuk bisnis), murid, teman - teman dan keluarga untuk tidak sembarangan dalam mendownlod file, tidak sembarangan memasuki link - link yang ada, usahakan untuk memasang ad-block dan usahakan perlindungan antivirus berada dalam versi yang terbaru

- - - - 

## William Sumitro - 14.111.1821

### 1. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : SQL Injection
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality dan Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: menginput data ke dalam query SQL kesebuah aplikasi. Apabila SQL injection tersebut berhasil, maka attacker ini dapat membaca isi semua yang ada didalam database juga dapat memodify (edit, add, delete) data tersebut.
* Counter Measure/Prevent &nbsp;: Menggunakan parameter, seperti SQL parameters.

### 2. Network Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Ping of Death (PoD)
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Attacker mengirimkan malformed atau packet berukuran lebih dari 65536 bytes dengan menggunakan perintah ping yang simple dimana dengan tujuan untuk membuat target komputer tersebut crash, reboot ataupun freeze. 
* Counter Measure/Prevent &nbsp;: Upgrade perangkat yang terhubung ke jaringan. Karena pada tahun 1998, semua perangkat telah diupgrade untuk mencegah serangan tersebut.

- - - - 