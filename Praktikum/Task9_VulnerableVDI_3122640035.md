<div class="cover" align="center">

<h3>
    <b>PRAKTIKUM KEAMANAN JARINGAN</b><br>
    "MENCARI KERENTANAN PADA VDI"
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

<div class="isiLaporan">

<hr>

<h3 align="center"> MENCARI KERENTANAN PADA VDI </h3> <br>

**A. Mengambil Data dari Database Menggunakan SQLMap**

**B. Mencari Tahu Password Root Menggunakan NMap**

1. Masuk ke root dan berikan perintah ifconfig untuk mengetahui IP address
   <img src="../Images/Task 9 - A06 Vulnerable Component/10.png">

2. Gunakan perintah ipcalc untuk menghitung dan menganalisis IP address dan subnet
   <img src="../Images/Task 9 - A06 Vulnerable Component/11.png">

3. Berikan perintah nmap untuk memindai jaringan <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/12.png"> <br>
   Dalam hal ini, digunakan nmap untuk memindai rentang IP address dan menampilkan IP address yang memiliki port 22 (SSH) yang terbuka. Kemudian didapatkan IP address 192.168.1.90

4. Lakukan brute force dengan nmap
   <img src="../Images/Task 9 - A06 Vulnerable Component/13.png"> <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/14.png"> <br>
   Brute force dilakukan dengan mengambil list username dan list password pada folder wordlist. Namun sayangnya, tidak ditemukan pasangan username dan password yang tepat.

</div>
