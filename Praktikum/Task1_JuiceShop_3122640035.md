<div class="cover" align="center">

<h3>
    <b>PRAKTIKUM KEAMANAN JARINGAN</b><br>
    "OWASP TOP 10 DAN JUICE SHOP"
</h3><br>

<img src="../Images/Logo_PENS.png" width="300"><br>

<p>Dosen Pengampu:<br>
Ferry Astika Saputra, S.T., M.Sc.</p> <br>

<p>Disusun Oleh:<br>
Jihan Ghaniyyah Putri Arrochim (3122640035)</p><br>

<p>
    <b>
        KELAS 1 D4 LJ IT B <br>
        JURUSAN D4 LJ TEKNIK INFORMATIKA <br>
        DEPARTEMEN TEKNIK INFORMATIKA DAN KOMPUTER <br> 
        POLITEKNIK ELEKTRONIKA NEGERI SURABAYA <br>
        2023
    </b>
</p>

</div> <br><br>

<hr>

<div class="isiLaporan">

<h3 align="center">OWASP TOP 10</h3><br>

OWASP atau Open Web Application Security Project merupakan sebuah komunitas non-profit yang bekerja untuk meningkatkan keamanan pada suatu software [1]. OWASP tidak berafiliasi dengan perusahaan teknologi manapun, meskipun OWASP berperan penting terhadap perkembangan teknologi sekuritas [2]. OWASP memiliki banyak software projectterbuka yang dipimpin oleh komunitas, ratusan cabang di penjuru dunia, puluhan ribu anggota, dan konferensi pendidikan juga pelatihan terbuka. Yayasan OWASP adalah pusat bagi developer dah expert untuk mengamankan website [1]. <br><br>
OWASP 10 atau OWASP Top 10 adalah 10 panduan yang dapat digunakan oleh programmer dan security team aplikasi website untuk mengatasi kerentanan. OWASP 10 dapat mengidentifikasi berbagai macam risiko keamanan yang sering terjadi dan harus segera diatasi oleh aplikasi website. Selama bertahun-tahun, OWASP 10 beralih untuk mengatasi berbagi tren serangan siber. Berikut adalah perubahan OWASP 10 dari tahun 2017 untuk 2021 [3-4]. <br>

<a href="https://owasp.org/Top10/id/"><img src='../Images/Task 1 - Apnic Module 1/owasp10.png' width=800></a><br>

-   **A01:2021-Broken Access Control (Kelemahan Access Control)**<br>
    Naik dari posisi kelima; 34 CWE (Common Weakness Enumeration) yang dipetakan ke Broken Access Control memiliki lebih banyak kemunculan dalam aplikasi dariapda kategori lainnya. Broken Access Control memungkinkan entri yang tidak sah yang dapat mengakibatkan kerentanan data dan file yang bersifat sensitif. Kontrol akses yang lemah terkait manajemen kredensial dapat diatasi dengan metode coding yang unik dan beberapa tindakan khusus seperti mematikan akun admin dan two-factor authentication.<br>
-   **A02:2021-Cryptographic Failures (Kegagalan Kriptografi)**<br>
    Naik dari posisi kedua. Sebelumnya dikenal sebagai Pengungkapan Data Sensitif. Fokus baru di sini adalah pada kegagalan terkait Kriptografi yang sering mengarah pada sistem yang telah terserang oleh peretas. API (Application Programming Interface) yang menghasilkan koneksi dan layanan pihak ketiga dapat dimanfaatkan oleh peretas karena data transmisi tidak aman.<br>
-   **A03:2021-Injection (Injeksi)**<br>
    Turun ke posisi ketiga; Injeksi mungkin terjadi apabila peretas memanipulasi kode yang tidak aman kemudian diinjeksikan ke dalam suatu program. Seringkali program yang diinjeksikan tidak dapat mengidentidikasi data yang terinjeksi. Jadi, peretas dapat mengetahui informasi rahasia, karena sistem mengidentifikasi bahwa peretas adalah pengguna yang terpercaya.<br>
-   **A04:2021-Insecure Design (Kekurangan pada Desain)**<br>
    Merupakan sebuah kategori baru dengan fokus pada risiko yang terkait dengan kekurangan desain. Kategori ini membahas pentingnya penggunaan pemodelan ancaman, pola dan desain yang aman, dan arsitektur referensi.<br>
-   **A05:2021-Security Misconfiguration (Kelemahan Konfigurasi Keamanan)**<br>
    Naik ke posisi kelima; Kategori ini sangat diperlukan karena mampu menunjukkan perangkat lunak yang dapat dikonfigurasi. Kategori ini mengatasi kesalahan konfigurasi yang dapat menimbulkan signifikan dengan memberikan akses kepada penyerang untuk masuk ke dalam sistem.<br>
-   **A06:2021-Vulnerable and Outdated Components (Komponen yang Rentan dan Kadaluarsa)**<br>
    Naik ke posisi keenam. Sebelumnya dikenal dengan Using Components with Known Vulnerabilities. Peretas dapat menyerang dan memanipulasi keamanan kode serta API sistem. Serangan ini dilakukan karena komponen pihak ketiga dan ketergantungan yang tidak aman. <br>
-   **A07:2021-Identification and Authentication Failures (Kegagalan Identifikasi dan Autentikasi)**<br>
    Turun dari posisi kedua. Sebelumnya dikenal dengan Broken Authentication dan sekarang termasuk CWE yang lebih terkait dengan kegagalan identifikasi. Risiko yang signifikan dapat memungkinkan peretas untuk menyalin peran dari identitas pengguna yang sah. Penggunaan alat pemindai DAST dan SCA dapat mendeteksi dan mengatasi permasalahan yang mencakup kesalahan implementasi sebelum programmer mengaplikasikan kode.<br>
-   **A08:2021-Software and Data Integrity Failures (Kegagalan Perangkat Lunak dan Keutuhan Data)**<br>
    Merupakan sebuah kategori baru pada tahun 2021. Kategori ini berfokus pada keputusan terkait pembaruan perangkat lunak, data penting, dan pipeline CI/CD tanpa memverifikasi integritas. Kategori ini merupakan salah satu dampak dari CVE (Common Vulnerability and Exposures) dan CVSS (Common Vulnerability Scoring System).<br>
-   **A09:2021-Security Logging and Monitoring Failures (Kegagalan pada Keamanan Logging dan Monitoring Data)**<br>
    Naik ke posisi kesembilan. Kategori ini diperluas untuk mencakup lebih banyak jenis kegagalan. Peretas bergantung pada kurangnya pemantauan dan pemulihan yang lambat untuk melakukan penyerangan. Aktivitas login tanpa kegagalan, kontrol akses dan validasi data dari server dapat mengidentifikasi aktivitas yang mencurigakan dalam sistem.<br>
-   **A10:2021-Server-Side Request Forgery (SSRF)**<br>
    Merupakan kategori baru dan berfokus pada pengujian. SSRF berkaitan dengan cakupan pengujian di atas rata-rata terhadap potensi eksploitasi dan dampak. Pada kategori ini, skenario pada tim keamanan juga menuntut relevansi data.<br>

<hr>

<h3 align="center">OWASP TOP 10 DENGAN JUICE SHOP</h3><br>

OWASP Juice Shop adalah aplikasi vulnerable website yang dikelola oleh OWASP. Aplikasi ini digunakan sebagai media pembelajaran terhadap kerentanan OWASP Top 10 [5].OWASP Juice Shop dibuat dengan Node.js, Express, dan Angular [6]. Aplikasi Juice Shop merupakan aplikasi website yang mencakup sejumlah besar kerentanan dari OWASP Top 10 di mana pengguna dapat meretas kerentanan tersebut [7]. Progres peretasan yang dilakukan dapat dilihat melalui score board. <br><br>
Score board dapat diketahui dengan cara mencari kata ‘score’ pada source tree sehingga dapat diketahui bahwa ‘score’ berada di file main.js. Pada file main.js, terdapat path score board untuk menuju halaman score board seperti pada gambar di bawah ini. <br>

<img src='../Images/Task 1 - Apnic Module 1/score-board.png' width=600> <br>

Berikut adalah halaman score board yang juga salah satu challenge pada aplikasi Juice Shop.

<img src='../Images/Task 1 - Apnic Module 1/score-board2.png' width=600> <br>

<a href='https://owasp.org/www-project-juice-shop/'>
<img src='../Images/Task 1 - Apnic Module 1/juiceshop.png' width=600> </a><br>

OWASP Juice Shop merupakan sebuah aplikasi website yang diimplementasi melalui JavaScript dan TypeScript. Pada bagian frontend digunakan framework Angular untuk membuat Single Page Application. Pada bagian layout user interface digunakan Material Design menggunakan komponen Angular Material. <br><br>
Bahasa pemrograman JavaScript juga digunakan pada bagian backend melalui Express yang dihosting di server Node.js untuk mengirimkan kode client-side ke browser. Express juga berperan dalam pembuatan fungsi backend melalui RESTful API. SQLite dipilih sebagai database karena SQLite merupakan database yang ringan karena berbasis file. Sebagai penyimpanan tambahan, MarsDB juga ditambahkan karena banyak digunakan dan kompatibel dengan Sebagian besar operasi query. <br><br>
Notifikasi push juga dapat terlihat saat challenge berhasil dilakukan yang mana hal ini diimplementasikan melalui WebSocket Protocol. Aplikasi tersebut juga memiliki fitur registrasi pengguna melalui OAuth 2.0 yang memungkinkan pengguna dapat menggunakan akun Google [8].

<hr>

<h3 align="center">INSTALASI OWASP JUICE SHOP</h3><br>

<img src='../Images/Task 1 - Apnic Module 1/1.png' width=600> </a><br>

Di sini penulis menggunakan OS Kali Linux versi 2022.1 dengan Oracle VM VirtualBox versi 6.1.18 sebagai virtual machine. Berikut adalah tahapan instalasi OWASP Juice Shop [9].

**Tahap 1. Unduh OWASP Juice Shop**<br>

Unduh OWASP Juice Shop versi terbaru dari halaman official <a href='https://github.com/juice-shop/juice-shop/releases/tag/v14.0.1'>GitHub</a>. Saat ini digunakan versi 14.0.1. Kemudian digunakan perintah **wget** untuk mengunduh paket OWASP Juice Shop. <br>

<img src='../Images/Task 1 - Apnic Module 1/2.png' width=600>

Kemudian diperlukan perintah **tar** untuk extract file yang telah diunduh.<br>

<img src='../Images/Task 1 - Apnic Module 1/3.png' width=300><br>

**Tahap 2. Install NodeJS dan NPM**<br>
Proses mengunduh NodeJS diperlukan perhatian khusus yaitu sebaiknya mengunduh versi NodeJS yang mirip dengan versi aplikasi Juice Shop. Aplikasi Juice Shop yang telah terunduh adalah versi 14.0.1, maka dari itu diperlukan NodeJS versi 14. <br>

Unduh NodeJS dari halaman resmi dan unduh NodeJS setup untuk Linux. Gunakan perintah **wget** untuk mengunduh. <br>

<img src='../Images/Task 1 - Apnic Module 1/4.png' width=600>

Kemudian diperlukan perintah **tar** untuk extract file yang telah diunduh.

<img src='../Images/Task 1 - Apnic Module 1/5.png' width=600>

Kemudian gunakan perintah **npm --version** dan **node --version** untuk melihat versi NPM dan Node yang telah terunduh.

<img src='../Images/Task 1 - Apnic Module 1/6.png' width=300><br>

**Tahap 3. Install Node Dependencies**<br>

Setelah NPM dan Node berhasil terunduh, masuk ke direktori OWASP Juice Shop yang telah diunduh dengan menggunakan perintah **cd**. Kemudian gunakan perintah **npm install** untuk mengunduh dependency dari NodeJS.

<img src='../Images/Task 1 - Apnic Module 1/7.png' width=600>

Gunakan perintah **npm start** untuk memulai web app. Kemudian akan terdapat responsebahwa website berada di **port 3000**

<img src='../Images/Task 1 - Apnic Module 1/8.png' width=600>

Buka http://localhost:3000// pada web browser dan OWASP Juice Shop sukses ter-install.

<img src='../Images/Task 1 - Apnic Module 1/9.png' width=600>

<hr>

<h3>Referensi</h3>
[1] “OWASP Foundation, the Open Source Foundation for Application Security | OWASP Foundation.” https://owasp.org/ (accessed Feb. 22, 2023).<br>
[2] “Tentang OWASP - OWASP Top 10:2021.” https://owasp.org/Top10/id/A00-about-owasp/ (accessed Feb. 22, 2023).<br>
[3] “Pengenalan - OWASP Top 10:2021.” https://owasp.org/Top10/id/A00_2021_Introduction/ (accessed Feb. 22, 2023).<br>
[4] “Apa itu Top 10 OWASP dan Bagaimana Cara Kerjanya? | Mandreel.com.” https://www.mandreel.com/indonesia/owasp/ (accessed Feb. 22, 2023).<br>
[5] “Kerentanan IDOR, SQL Injection dan Broken Authentication pada aplikasi OWASP Juice Shop.” https://securxcess.com/blog/kerentanan-idor-sql-injection-dan-broken-authentication-pada-aplikasi-owasp-juice-shop-58 (accessed Feb. 21, 2023).<br>
[6] “OWASP Juice Shop | OWASP Foundation.” https://owasp.org/www-project-juice-shop/ (accessed Feb. 22, 2023).<br>
[7] “GitHub - juice-shop/juice-shop: OWASP Juice Shop: Probably the most modern and sophisticated insecure web application.” https://github.com/juice-shop/juice-shop (accessed Feb. 22, 2023).<br>
[8] “Architecture overview · Pwning OWASP Juice Shop.” https://pwning.owasp-juice.shop/introduction/architecture.html (accessed Feb. 22, 2023).<br>
[9] “Install OWASP Juice Shop on Kali Linux [Step-by-Step] | GoLinuxCloud.” https://www.golinuxcloud.com/install-owasp-juice-shop-kali-linux/ (accessed Feb. 21, 2023)<br>
