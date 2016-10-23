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

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : IP Address Spoofing Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: attacker menanam source IP address palsu pada packet. Dengan mengganti source IP address, response dari pakcet akan dikirim pada IP address yang salah, dengan demikian attacker bisa mendapatkan data tersebut.
* Counter Measure/Prevent &nbsp;: Packet filtering adalah metode untuk mencegah IP Spoofing attack. Mem-block packet dari luar network dengan source address di dalam network (filter jalan masuk) dan mem-block packet dari dalam network dengan source address di luar network (filter jalan keluar) dapat membantu pencegahan IP spoofing attack.

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

### 1. Transport Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Teardrop / IP Fragmentation Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Teardrop attack adalah suatu serangan Denial of Service (DoS) yang memanfaatkan kelemahan yang ada di TCP/IP yaitu packet fragmentation atau pemecahan paket  pada waktu paket-paket yang terfragmentasi tersebut disatukan kembali. Penyerang melakukan spoofing/pemalsuan/rekayasa terhadap paket-paket yang dikirim ke server yang hendak diserangnya, misalnya gap dan overlap pada waktu paket-paket tersebut disatukan kembali. Sehingga saat menyatukannya kembali, server akan bingung dan akhirnya crash, hang, atau melakukan reboot.
* Counter Measure/Prevent &nbsp;: paket filtering melalui firewall yang sudah dikonfigurasi untuk memantau dan memblokir paket-paket yang mencurigakan, misalnya apakah melanggar ketentuan fragmentation (contoh: menggunakan router atau proxy yang aman). Selain itu juga dapat dilakukan mekanisme blacklisting / whitelisting yang memfilter traffic berdasarkan faktor misalnya IP reputation dan rate pattern.

### 2. Application Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : DNS Poisoning
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Confidentiality
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Serangan dengan cara menyampaikan informasi IP Address yang salah mengenai sebuah host, dengan tujuan untuk mengalihkan lalu lintas paket data dari tujuan yang sebenarnya. DNS Poisoning mengacaukan DNS Server asli dengan cara mengeksploitasi vulnerability pada DNS Service agar pengguna Internet terkelabui untuk mengakses web site palsu yang dibuat benar-benar menyerupai aslinya tersebut, agar data dapat masuk ke server palsu.
* Counter Measure/Prevent &nbsp;: Melakukan otentikasi host yang akan kita hubungi, misalnya mempergunakan digital certificate. Dengan digital certificate, seseorang dapat dengan yakin bahwa host yang dia akses adalah host yang sebenarnya.

- - - -

## Adlin M. Hasri - 14.111.1642

### 1. Data-Link Layer

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : MAC Flooding
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: Availability
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;: Sebuah serangan yang langka, dimana penyerang mengirimkan beberapa frame Ethernet boneka, masing-masing dengan alamat MAC yang berbeda, Network switch memperlakukan alamat MAC secara terpisah, dan menyebabkan pemesanan beberapa sumber daya untuk setiap permintaan. Ketika semua memori di switch digunakan, hal tersebut dapat mematikan atau penyebab sistem tidak responsif. Dalam beberapa jenis router, serangan MAC Flooding dapat menyebabkan seluruh tabel routing mereka down, sehingga mengganggu seluruh jaringan yang ada dibawah domain routing.
* Counter Measure/Prevent &nbsp;: Gunakan "port-security" untuk membatasi sebuah port ke nomor (mungkin satu) sumber alamat MAC. Setelah jumlah ini melebihi batas, Switch dapat menjebak, shutdown port atau membuang frame yang masuk.

### 2. Layer Name Here

* Nama Penyerangan &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Smurf Attack
* Penyerangan Terhadap &nbsp; &nbsp; &nbsp;: A
* Deskripsi Penyerangan &nbsp; &nbsp; &nbsp;:  sebuah serangan yang dibangun dengan menggunakan pemalsuan terhadap paket-paket ICMP echo request, yakni sebuah jenis paket yang digunakan oleh utilitas troubleshooting jaringan, PING. Si penyerang akan memulai serangan dengan membuat paket-paket "ICMP echo request" dengan alamat IP sumber berisi alamat IP host target yang akan diserang (berarti alamat telah dipalsukan atau telah terjadi address spoofing). Paket-paket tersebut pun akan dikirimkan secara broadcast ke jaringan di mana komputer target berada, dan host-host lainnya yang menerima paket yang bersangkutan akan mengirimkan balasan dari "ICMP echo request" ("ICMP echo reply") kepada komputer target, seolah-olah komputer target merupakan komputer yang mengirimkan ICMP echo request tersebut. Semakin banyak komputer yang terdapat di dalam jaringan yang sama dengan target, maka semakin banyak pula ICMP echo reply yang dikirimkan kepada target, sehingga akan membanjiri sumber daya komputer target, dan mengakibatkan kondisi penolakan layanan (Denial of Service) yang menjadikan para pengguna tidak dapat mengakses layanan yang terdapat di dalam komputer yang diserang. Beberapa sistem bahkan mengalami crash atau hang, dan lagi, banjir yang berisi paket-paket "ICMP echo request/reply" akan membuat kongesti (kemacetan) jaringan yang dapat memengaruhi komputer lainnya.
* Counter Measure/Prevent &nbsp;: Beberapa langkah preventif :
Langkah 1. Amplifier Konfigurasi. router harus dikonfigurasi sehingga tidak maju diarahkan siaran ke jaringan. Penting untuk dicatat bahwa broadcast tersebut harus dinonaktifkan pada semua router dan tidak hanya hanya yang eksternal. Perintah "no ip directed-broadcast" pada router Cisco harus melakukan tugas dalam banyak kasus. Ini juga akan memastikan bahwa karyawan pada jaringan internal tidak akan dapat memulai serangan Smurf. Namun juga disarankan bahwa seseorang memiliki perangkat penyaringan (seperti firewall) di perimeter, sehingga memberikan lapisan tambahan keamanan.

Langkah 2. Konfigurasi sistem operasi server. Server harus dikonfigurasi sehingga mereka tidak akan menanggapi permintaan broadcast diarahkan. FreeBSD adalah salah satu sistem tersebut yang secara default tidak menanggapi permintaan ini.

Langkah 3. Victim issues, tidak banyak yang dapat dilakukan pada korban terakhir dan kerusakan akan selesai kecuali ISP korban mengambil beberapa tindakan untuk memblokir ICMP Echo Reply floods. Bahkan jika korban router parameter menyangkal ICMP Echo Reply, link dari ISP ke situs korban akan menderita.

- - - -
