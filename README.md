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

### 1. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Teardrop
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: C
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Teardrop attack adalah suatu serangan bertipe Denial of Service (DoS) terhadap suatu server/komputer yang terhubung dalam suatu jaringan. Teardrop attack ini memanfaatkan fitur yang ada di TCP/IP yaitu packet fragmentation atau pemecahan paket, dan kelemahan yang ada di TCP/IP pada waktu paket-paket yang terfragmentasi tersebut disatukan kembali. Dalam suatu pengiriman data dari satu komputer ke komputer yang lain melalui jaringan berbasis TCP/IP, maka data tersebut akan dipecah-pecah menjadi beberapa paket yang lebih kecil di komputer asal, dan paket-paket tersebut dikirim dan kemudian disatukan kembali di komputer tujuan. Dalam teardrop attack, penyerang melakukan spoofing/pemalsuan/rekayasa terhadap paket-paket yang dikirim ke server yang hendak diserangnya.
* Counter Measure/Prevent &nbsp;: Server bisa diproteksi dari tipe serangan teardrop ini dengan paket filtering melalui firewall yang sudah dikonfigurasi untuk memantau dan memblokir paket-paket yang berbahaya.

### 2. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Half-Open Connection
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: A
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Half-open connection attack juga disebut sebagai SYN attack karena memanfaatkan paket SYN (synchronization) dan kelemahan yang ada di 3-way handshake pada waktu hubungan TCP/IP ingin dibentuk antara 2 komputer. Dalam serangan half-open connection, penyerang mengirimkan ke server yang hendak diserang banyak paket SYN yang telah dispoof atau direkayasa sehingga alamat asal (source address) menjadi tidak valid. Dengan kata lain, alamat asal paket-paket SYN tersebut tidak menunjuk pada komputer yang benar-benar ada. Pada waktu server menerima paket-paket SYN tersebut, maka server akan mengirimkan paket SYN/ACK untuk menjawab tiap paket SYN yang diterima. Namun, karena paket SYN/ACK dari server tersebut dikirim ke alamat yang tidak ada, maka server akan terus menunggu untuk menerima jawaban berupa paket ACK. Jika server tersebut dibanjiri oleh paket-paket SYN yang tidak valid tersebut, maka akhirnya server akan kehabisan memory dan sumber daya komputasi karena server terus menunggu untuk menerima jawaban paket ACK yang tidak akan pernah datang. Akhirnya server akan crash, hang, atau melakukan reboot dan terjadilah gangguan terhadap layanan (denial of service).
* Counter Measure/Prevent &nbsp;: Tipe serangan half-open connection atau SYN attack ini dapat dicegah dengan paket filtering dan firewall, sehingga paket-paket SYN yang invalid tersebut dapat diblokir oleh firewall sebelum membanjiri server.

- - - -

