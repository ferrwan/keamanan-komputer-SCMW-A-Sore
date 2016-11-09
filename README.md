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
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: penyerangan pada layer 3 dengan infrastruktur metode penyerangan DDoS yang menggunakan ICMP untuk mengoverload bandwith dari target yang akan diserang. Biasa ping digunakan untuk mengecek konektifitas antara 2 komputer dengan cara request ICMP dikirim dan komputer target membalas balik dengan ICMP pula.ICMP flooding bekerja dengan mengirimkan request tersebut(ping) secepat mungkin tanpa menunggu komputer target mereply/membalas sehingga terjadi overloading pada jaringan target.
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
na
* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;: Traffic Analysis Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentialty
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerangan dengan menganalisis pergerakan dari paket-paket yang berbeda pada jaringan, dengan tujuan mendapatkan informasi dari pola trafik paket-paket tersebut, semakin banyak paket yang terobservasi semakin banyak pula informasi yang didapatkan.
* Counter Measure/Prevent &nbsp;: Menyembunyikan alamat dari user dan sistem yang sedang berkomunikasi

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

### 2. Physical Layer &amp; Data Link Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Evil Twin attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Evil Twin attack dikenal sebagai wireless hijacking dimana hacker memisahkan komunikasi client dan Legitimate AP. Client kehilangan koneksi ke legitimate AP dan reconnect ke evil twin access point. Sehingga attacker dapat mencuri pasword, monitoring apa yang mereka lakukan, dsb
* Counter Measure/Prevent &nbsp;: Dibutuhkan 802.1X untuk WLAN, dimana menggunakan tipe EAP yang memberikan otentikasi secara bersama dan juga memeriksa sertifikasi dari sebuah server. Ada juga sebuah tool yang dinamakan EvilAP_defender dapat mencegah terjadinya evil twin attack.

- - - -

## Stephen - 14.111.0868

### 1. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Keylogger
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Keylogger adalah sebuat penyerangan yang berjalan pada proses background dari sebuah komputer, mencatat atau merekam semua tombol yang di ketikkan oleh user. Setelah user mengetikkan sebuah password, password tersebut disimpan pada sebuah log yang dibuat oleh Keylogger yang kemudian dapat dibaca oleh attacker
* Counter Measure/Prevent &nbsp;: User dapat menggunakan Keylogger detection software, Spybot, atau memberi pengetahuan / edukasi terhadap user untuk tidak sembarangan mengetikkan password pada sembarangan komputer.

### 2. Network Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Salami Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Integrity
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Dengan mengumpulkan data dengan jumlah yang kecil dan melibatkan attacker untuk mengubah informasi yang terdapar di database. Attacker mencuri hanya sedikit dalam jangka waktu yang lama dari jumlah transaksi yang besar.
* Counter Measure/Prevent &nbsp;: perusahaan mengupdate security system setinggi mungkin. Bank mengimbau customer untuk melapor pengurangan-pengurangan pada uang mereka yang tidak mereka ketahui penyebabnya.

- - - -

## Edwin Harly - 14.111.1014

### 1. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Man-in-the-Middle
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality & Integrity
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerang menyadap atau sniffing sebuah koneksi antara 2 user. Kedua user ini percaya bahwa mereka berkomunikasi satu sama lain, padahal dibalik itu mereka berkomunikasi melalui perantara si penyerang, sehingga pesan apapun yang dikirim akan melewati si penyerang dulu, dengan begitu penyerang bisa mengetahui isi pesan yang dikirim dan juga bisa mengubah isi pesan yang dikirim.
* Counter Measure/Prevent &nbsp;: Beberapa teknik untuk menangkalnya adalah DNSSEC (Secure DNS extensions), Public key infrastructures, Certificate pinning.

### 2. Session Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : SSH Downgrade Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerang akan meminta secara paksa kepada client dan server untuk menggunakan protokol SSH1 yang kurang aman sehingga penyerang bisa lebih mudah untuk menyerang. Biasanya terjadi kepada server yang mendukung SSH1 dan SSH2.
* Counter Measure/Prevent &nbsp;: Setting agar server hanya akan menerima versi protokol SSH terbaru

- - - -

## Calvin - 14.111.2028

### 1. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : CRIME (Compression Ratio Info-leak Made Easy)
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality & Integrity
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: CRIME adalah eksploitasi keamanan terhadap cookies melalui koneksi yang menggunakan HTTPS dan protokol SPDY yang juga mengkompresi data. Ketika digunakan untuk mendapatkan isi dari cookie yang berisi autentikasi rahasia, maka hal itu memungkinkan penyerang untuk melakukan pembajakan pada web yang terautentikasi oleh sesi,yang memungkinkan penyerang untuk melancarkan serangan lebih lanjut.
* Counter Measure/Prevent &nbsp;: CRIME bisa dihindari dengan menghindari penggunaan kompresi, baik pada client, melarang web untuk mengkompresi permintaan dengan SPDY, atau dari website dengan melarang penggunaan kompresi data transaksi tersebut dengan menggunakan fitur negosiasi protokol TLS.

### 2. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Application Layer DDoS
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerangan DDoS melalui Lapisan Application dilakukan terutuma untuk target yang khusus, termasuk mengganggu transaksi dan akses terhadap database.Penyerangan ini menghabiskan resource yang sedikit dan terkadang dibarengi dengan penyerangan di sisi network layer. Penyerangan ini menyamar seperti lalu lintas jaringan yang normal, kecuali pihaknya menargetkan pada aplikasi tertentu. Serangan pada application layer ini dapat mengganggu layanan seperti pengambilan informasi atau fungsi pencarian serta fungsi browser, layanan email dan aplikasi foto, untuk berhasil melakukan ddos, diperlukan lebih dari sekitar 3-5 node pada jaraingan yang berbeda harus digunakan.
* Counter Measure/Prevent &nbsp;: Perlindungan terhadap serangan ini membutuhkan DDoS Mitigation. Keberhasilan mitigasi membutuhkan pengecekan atau pengidentifikasian lalu lintas network yang masuk, membedakan apakah lalu lintas itu berasal dari manusia kah, atau dari bott atau program yang mengirimkannya.

- - - -
## Adrian Hartanto - 14.111.1537

### 1. Presentation Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : SSL Garbage Flood
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Salah satu bentuk penyerangan DDoS dengan mengirimkan request SSL yang berbahaya ke SSL server dan mencoba menghabiskan resource dari Server tersebut,serta memblokir layanan dari pengguna.
* Counter Measure/Prevent &nbsp;: Menggunakan IPS (Intrusion Prevention System) Signature , memaksimalkan settingan pada server, atau menggunakan jasa DDos Mitigation Service Provider.

### 2. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : FTP Bounce Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Penyerangan dengan mengeksploitasi protokol FTP dimana penyerang dapat menggunakan perintah PORT untuk meminta akses ke port secara tidak langsung melalui penggunaan device korban sebagai orang tengah untuk proses request. Penyerangan ini dapat digunakan untuk port scan host secara diam-diam , dan mengakses port tertentu yang mana penyerang tidak dapat mengaksesnya melalui koneksi langsung, contohnya dengan nmap port scanner.
* Counter Measure/Prevent &nbsp;: Memastikan agar server FTP tidak mengirimkan data melalui port-port TCP dibawah angka 1024, menggunakan password yang baik, dan tidak menggunakan user standar  (menghindari user enumeration).
- - - -

## Adlin M. Hasri - 14.111.1642

### 1. Network Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Sinkhole Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Integrity and Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Sinkhole attack merupakan salah satu active attack yang berada pada layer network. Serangan sinkhole ini akan memberikan informasi routing yang salah pada node - node yang ada pada jaringan, sehingga informasi yang dikirimkan dapat diketahui oleh penyerang. Cara kerja serangan ini biasanya menggunakan kelemahan protokol yang digunakan pada jaringan. Serangan pada AODV (Ad hoc On-demand Distance Vector) akan dilakukan dengan memaksimalkan sequence number atau meminimalkan jumlah hop pada jaringan AODV. Sedangkan untuk DSR (Debt Service Ratio), serangan ini akan memanfaatkan pesan RREQ (Route Request) yang berisi alamat pengirim atau tujuan dengan memasukkan node sinkhole sebagai hop tujuan.
* Counter Measure/Prevent &nbsp;: Pencengahan pendekatan mendasar :
    * Kryptografi "message digests algorithm" untuk mendeteksi sinkhole attacks.
    * 2 protocols, RESIST-0 dan RESIST-1, yang menggunakan pendekatan kriptografis di dalam routing protocols untuk mengatasi masalah sinkhole attacks
    * A Trust Based Routing Protocol untuk Mitigasi serangan Sinkhole di Wireless Sensor Networks

### 2. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Smurf Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;:  sebuah serangan yang dibangun dengan menggunakan pemalsuan terhadap paket-paket ICMP echo request, yakni sebuah jenis paket yang digunakan oleh utilitas troubleshooting jaringan, PING. Si penyerang akan memulai serangan dengan membuat paket-paket "ICMP echo request" dengan alamat IP sumber berisi alamat IP host target yang akan diserang (berarti alamat telah dipalsukan atau telah terjadi address spoofing). Paket-paket tersebut pun akan dikirimkan secara broadcast ke jaringan di mana komputer target berada, dan host-host lainnya yang menerima paket yang bersangkutan akan mengirimkan balasan dari "ICMP echo request" ("ICMP echo reply") kepada komputer target, seolah-olah komputer target merupakan komputer yang mengirimkan ICMP echo request tersebut. Semakin banyak komputer yang terdapat di dalam jaringan yang sama dengan target, maka semakin banyak pula ICMP echo reply yang dikirimkan kepada target, sehingga akan membanjiri sumber daya komputer target, dan mengakibatkan kondisi penolakan layanan (Denial of Service) yang menjadikan para pengguna tidak dapat mengakses layanan yang terdapat di dalam komputer yang diserang. Beberapa sistem bahkan mengalami crash atau hang, dan lagi, banjir yang berisi paket-paket "ICMP echo request/reply" akan membuat kongesti (kemacetan) jaringan yang dapat memengaruhi komputer lainnya.
* Counter Measure/Prevent &nbsp;: Beberapa langkah preventif :
    * Langkah 1. Amplifier Konfigurasi. router harus dikonfigurasi sehingga tidak maju diarahkan siaran ke jaringan. Penting untuk dicatat bahwa broadcast tersebut harus dinonaktifkan pada semua router dan tidak hanya hanya yang eksternal. Perintah "no ip directed-broadcast" pada router Cisco harus melakukan tugas dalam banyak kasus. Ini juga akan memastikan bahwa karyawan pada jaringan internal tidak akan dapat memulai serangan Smurf. Namun juga disarankan bahwa seseorang memiliki perangkat penyaringan (seperti firewall) di perimeter, sehingga memberikan lapisan tambahan keamanan.
    * Langkah 2. Konfigurasi sistem operasi server. Server harus dikonfigurasi sehingga mereka tidak akan menanggapi permintaan broadcast diarahkan. FreeBSD adalah salah satu sistem tersebut yang secara default tidak menanggapi permintaan ini.
    * Langkah 3. Victim issues, tidak banyak yang dapat dilakukan pada korban terakhir dan kerusakan akan selesai kecuali ISP korban mengambil beberapa tindakan untuk memblokir ICMP Echo Reply floods. Bahkan jika korban router parameter menyangkal ICMP Echo Reply, link dari ISP ke situs korban akan menderita.

- - - -

## Jeffry - 14.111.0027

### 1. Data-Link Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : PHP Injection
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: I
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Script PHP merupakan salah satu script yang sampai saat ini banyak digunakan oleh seorang webmaster, disamping rival nya JavaScript. PHP ini begitu 'Powerfull' karena dalam script php ini kita bisa melakukan banyak hal. Mulai dari membuat file, membuat counter, membuat date, membuat buku tamu, membuat forum (salah satunya PhpBB), mengakses database secara langsung maupun juga membuat gambar dan animasi. PHP Injection adalah mencari bugs pada script php yang ada yang dilakukan oleh sebagian hacker sehingga dapat mengubah data-data yang ada.
* Counter Measure/Prevent &nbsp;: Server bisa diproteksi dengan paket filtering melalui firewall yang sudah dikonfigurasi untuk memantau dan memblokir paket-paket yang berbahaya.

### 2. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Identify Spoofing
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: C
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Spoofing terjadi ketika penyerang menentukan dan menggunakan alamat IP dari  jaringan, komputer, atau jaringan komponen tanpa wewenang untuk melakukannya. Sebuah serangan yang sukses memungkinkan penyerang untuk  beroperasi sebagai jika penyerang adalah entitas biasanya diidentifikasi oleh alamat IP. Dalam konteks Office Communications Server 2007 R2, situasi ini datang ke dalam bermain hanya jika administrator telah melakukan kedua hal  berikut: Koneksi dikonfigurasi yang hanya mendukung Transmission Control Protocol (TCP) (yang tidak dianjurkan, karena komunikasi TCP tidak terenkripsi). Harus menandai alamat IP dari koneksi tersebut sebagai host yang terpercaya. Ini adalah kurang dari masalah untuk Transport Layer Security (TLS) koneksi, yang secara definisi dienkripsi. Tindakan pencegahan ini dapat mencegahnya untuk melakukan spoofing alamat IP pada koneksi tertentu (misalnya, hubungan timbal balik TLS). Tapi penyerang masih bisa spoof alamat server DNS yang menggunakan Office Communications Server. Meskipun spoofing ini merupakan ancaman bagi Office Communications Server, tidak ada server dapat lakukan untuk mencegahnya.
* Counter Measure/Prevent &nbsp;: Mencegah serangan ini membutuhkan TI-infrastruktur dan mitigasi jaringan tingkat.

- - - -

### Teddy - 141110035

### 1. Network Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Jamming Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Adalah cara membuat kacau sinyal di suatu daerah. Tindakan ini akan berbahaya apabila dilakukan oleh orang yang tidak bertanggung jawab karena hal ini bisa mengakibatkan jaringan sebuah kota lumpuh.
* Counter Measure/Prevent &nbsp;: Melakukan sistem blocking terhadap IP yang mencurigakan.

### 2. DataLink Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Eavesdrooping
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: suatu kegiatan melakukan intersepsi atau mengintip maupun menguping yang tak diizinkan baik itu komunikasi pribadi lewat telepon, sms. video conference, maupun transmisi fax. Kegiatan ini dilakukan guna mencuri data yang dikirim melalui jaringan yang tidak dienkripsi lebih dahulu.
* Counter Measure/Prevent &nbsp;: Dengan membuat teknologi enkripsi data terlebih dahulu sebelum data dikirim ke penerima

- - - -

### William Karno - 141112052

### 1. Transport Layer

* Nama Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: Beast
* Penyerangan Terhadap &nbsp;&nbsp;&nbsp;&nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;: Beast melakukan penyerangan pada bagian Transport layer dengan versi TLS 1.0. Beast melakukan exploitasi pada kelemahan Cipher Block Chainning (CBC) yang mengakibatkan dapat melakukan eksploitasi terhadap SSL. CBC dapat digunakan untuk melakukan MITM (man in the middle) untuk menyerang SSL dengan cara dekripsi dan memperoleh authentication token.
* Counter Measure/Prevent&nbsp;: dengan melakukan update terhadap browser dan teknology yang terintegrasi serta menggunakan TLS versi 1.1

### 2. Transport Layer

* Nama Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: Breach
* Penyerangan Terhadap &nbsp;&nbsp;&nbsp;&nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;: Breach melakukan ekploitasi pada bagian kompresi dan kombinasi enkripsi pada web server atau user. Breach menyerang kompresi dari http dengan mengambil token.
* Counter Measure/Prevent&nbsp;: dengan melakukan disabling compression

- - - -

### Hendra Tandiono - 141110370

### 1. Layer Network

* Nama Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: LAND Attack
* Penyerangan Terhadap &nbsp;&nbsp;&nbsp;&nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;: LAND attack adalah serangan terhadap suatu server atau komputer yang terhubung dalam jaringan yang bertujuan untuk menghentikan layanan yang diberikan oleh server tersebut sehingga terjadi gangguan terhadap jaringan komputer itu. Tipe serangan semacam ini disebut sebagai Denial of Service (DoS) attack. LAND attack dikategorikan sebagai serangan SYN(SYN attack) karena menggunakan packet SYN (synchronization) pada waktu melakukan 3-way handshake untuk membentuk suatu hubungan berbasis TCP/IP. 
* Counter Measure/Prevent &nbsp;:
    * Melakukan Pengecekan data transfer yang tidak sesuai dengan data yang kita kirim
    * Menginstall Firewall yang memiliki konfigurasi untuk menahan data yang tidak di inginkan atau mencurigakan

### 1. Layer Network

* Nama Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: Ping Kematian (Ping of death)
* Penyerangan Terhadap &nbsp;&nbsp;&nbsp;&nbsp;: Availability
* Deskripsi Penyerangan &nbsp;&nbsp;&nbsp;&nbsp;: Ping Kematian ( Ping of death disingkat POD) adalah jenis serangan pada komputer yang melibatkan pengiriman ping yang salah atau berbahaya ke komputer target. Sebuah ping biasanya berukuran 56 byte (atau 84 bytes ketika header IP dianggap). Dalam sejarahnya, banyak sistem komputer tidak bisa menangani paket ping lebih besar daripada ukuran maksimum paket IP, yaitu 65.535 byte. Mengirim ping dalam ukuran ini (65.535 byte) bisa mengakibatkan kerusakan (crash) pada komputer target.
* Counter Measure/Prevent &nbsp;:
    * Menginstall Firewall yang memiliki konfigurasi untuk menahan data yang tidak di inginkan atau mencurigakan
    * Melakukan update terhadap program yang bersangkutan

- - - -

## Kevin Fransetio - 141110876

### 1. Layer Network

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : DNS Poisoning
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality, Integrity, dan Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: DNS Poisoning merupakan sebuah cara untuk menembus pertahanan dengan cara menyampaikan informasi IP Address yang salah mengenai sebuah host, dengan tujuan untuk mengalihkan lalu lintas paket data dari tujuan yang sebenarnya. Cara ini banyak dipakai untuk menyerang situs-situs e-commerce dan banking yang saat ini bisa dilakukan dengan cara online dengan pengamanan Token. Teknik ini dapat membuat sebuah server palsu tampil identik dengan dengan server online banking yang asli. Oleh karena itu diperlukan digital cerficate untuk mengamankannya, agar server palsu tidak dapat menangkap data otentifikasi dari nasabah yang mengaksesnya. Jadi dapat disimpulkan cara kerja DNS (Domain Name System) poisoning ini adalah dengan mengacaukan DNS Server asli agar pengguna Internet terkelabui untuk mengakses web site palsu yang dibuat benar-benar menyerupai aslinya tersebut, agar data dapat masuk ke server palsu.
* Counter Measure/Prevent &nbsp;: Cara mengatasinya adalah gunakan DNS server yang terpercaya, dan bagi seorang admin agar selalu melakukan hardening thd DNS server miliknya, bisa dengan cara membatasi 'trust' peering DNS, dll.

### 2. Layer Network

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Trojan Horse
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality ,Integrity, dan Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Trojan horse atau Kuda Troya atau yang lebih dikenal sebagai Trojan dalam keamanan komputer merujuk kepada sebuah bentuk perangkat lunak yang mencurigakan (malicious software/malware) yang dapat merusak sebuah sistem atau jaringan. Tujuan dari Trojan adalah memperoleh informasi dari target (password, kebiasaan user yang tercatat dalam system log, data, dan lain-lain), dan mengendalikan target (memperoleh hak akses pada target).

Cara Kerja Trojan Horse
Trojan berbeda dengan jenis perangkat lunak mencurigakan lainnya seperti virus komputer atau worm karena dua hal berikut :
- Trojan bersifat "stealth" (siluman dan tidak terlihat) dalam operasinya dan seringkali berbentuk seolah-olah program tersebut merupakan program baik-baik, sementara virus computer atau worm bertindak lebih agresif dengan merusak sistem atau membuat sistem menjadi crash.
- Trojan dikendalikan dari komputer lain (komputer attacker).

Jenis-Jenis Trojan Horse
- Remote Access Trojan
Disingkat sebagai RAT,  adalah salah satu dari tujuh jenis utama dari Trojan horse dirancang untuk memberikan penyerang dengan kontrol penuh dari sistem korban. Penyerang biasanya menyembunyikan virus trojan horse ini dalam permainan dan program kecil lainnya yang tidak curiga pengguna kemudian dijalankan pada PC mereka.

- Data Sending Trojan
Jenis trojan horse ini merupakan program yang dirancang untuk mendapatkan data penting dari target serangan data-data penting tersebut seperti akun, password, informasi kartu kredit, file, log alamat e-mail atau lain sebagainya.

- Destruktive trojan / trojan perusak
Trojan perusak merupakan suatu jenis trojan horse yang dirancang untuk menghancurkan dan menghapus file, dan lebih seperti virus dari yang lain Trojan.

- Proxy trojan
Suatu jenis Trojan horse yang dirancang untuk menggunakan komputer korban sebagai server proxy.

- File Transfer Protocol (FTP)
Suatu jenis Trojan horse dirancang untuk membuka pelabuhan 21 (file transfer protokol) dan memungkinkan penyerang terhubung ke komputer anda menggunakan File Transfer Protocol (FTP).
  
- Security software disabler Trojan
Suatu jenis Trojan horse berhenti dirancang atau membunuh keamanan program seperti program antivirus atau firewall tanpa pengguna mengetahui. Jenis Trojan ini biasanya dikombinasikan dengan jenis lain dari Trojan sebagai payload.

- Pencatat penekanan tombol (keystroke logger/keylogger): Jenis Trojan ini akan memantau semua yang diketikkan oleh pengguna dan akan mengirimkannya kepada penyerang. Jenis ini berbeda dengan spyware, meski dua hal tersebut melakukan hal yang serupa (memata-matai pengguna).
Tool administrasi jarak jauh (Remote Administration Tools/RAT): Jenis Trojan ini mengizinkan para penyerang untuk mengambil alih kontrol secara penuh terhadap sistem dan melakukan apapun yang mereka mau dari jarak jauh, seperti memformat hard disk, mencuri atau menghapus data dan lain-lain. Contoh dari Trojan ini adalah Back Orifice, Back Orifice 2000, dan SubSeven.

- DDoS Trojan atau Zombie Trojan: Jenis Trojan ini digunakan untuk menjadikan sistem yang terinfeksi agar dapat melakukan serangan penolakan layanan secara terdistribusi terhadap host target.
Ada lagi sebuah jenis Trojan yang mengimbuhkan dirinya sendiri ke sebuah program untuk memodifikasi cara kerja program yang diimbuhinya. Jenis Trojan ini disebut sebagai Trojan virus.

- Cookies Stuffing, ini adalah script yang termasuk dalam metode blackhat, gunanya untuk membajak tracking code penjualan suatu produk, sehingga komisi penjualan diterima oleh pemasang cookies stuffing, bukan oleh orang yang terlebih dahulu mereferensikan penjualan produk tersebut di internet

Cara Penyebaran Trojan Horse

Penggunaan istilah Trojan atau Trojan horse dimaksudkan untuk menyusupkan kode-kode mencurigakan dan merusak di dalam sebuah program baik-baik dan berguna; seperti halnya dalam Perang Troya, para prajurit Sparta bersembunyi di dalam Kuda Troya yang ditujukan sebagai pengabdian kepada Poseidon. Kuda Troya tersebut menurut para petinggi Troya dianggap tidak berbahaya, dan diizinkan masuk ke dalam benteng Troya yang tidak dapat ditembus oleh para prajurit Yunani selama kurang lebih 10 tahun perang Troya bergejolak.

* Counter Measure/Prevent &nbsp;: Untuk mencegah dan menghapus virus Trojan pastikan anda memasang antivirus yang selalu ter-update, mengaktifkan Firewall baik bawaan dari Windows atau dari luar juga mengurangi resiko komputer kita diintai atau dikendalikan dari komputer lain.

- - - -