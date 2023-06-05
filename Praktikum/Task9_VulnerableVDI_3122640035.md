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

1. Dapatkan IP address VDI untuk menyerang <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/18.png" width="600">
2. Buka IP address pada browser <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/15.jpeg" width="600">
3. Mencari halaman yang memerlukan ID, seperti halaman detail artikel. Kemudian masukkan url 192.168.0.9/index.php?tampil=artikel_detail&id=85. Setelahnya jalankan SQLMap dengan perintah sqlmap -u "http://192.168.0.9/index.php?tampil=artikel_detail&id=85" --dbs <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/16.png" width="600"> <br>
   Database berhasil ditemukan
4. Melihat tabel yang ada pada database dengan menjalankan perintah sqlmap -u "http://192.168.0.9/index.php?tampil=artikel_detail&id=85" -D vulnweb --tables <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/17.png"> <br>
   Database vulnweb memiliki 7 tabel, yaitu user, artikel, galeri, halaman, komentar, menu, dan pesan
5. Menuju tabel user untuk mengetahui username dan password dengan script<br>
   sqlmap -u "http://192.168.30.148/?tampil=halaman&id=78" -C id_user, password, username --dump <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/67.png" width="300"> <br>
   Dapat diketahui bahwa username adalah **vulnweb** dan password juga **vulnweb**
6. Buka browser, tuju halaman "http://192.168.1.90/admin/index.php" untuk Login <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/68.jpeg" width="600"> <br>
   Masukkan username dan password
7. Berhasil masuk ke halaman Admin <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/69.jpeg" width="600"> <br>
8. Pada halaman Admin terdapat beberapa menu di bagian navigation bar. Salah satunya adalah menu Daftar Halaman <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/70.jpeg" width="600"> <br>

**B. Mencari Tahu Password Root Menggunakan NMap**

1. Masuk ke root dan berikan perintah ifconfig untuk mengetahui IP address <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/10.png" width="600">

2. Gunakan perintah ipcalc untuk menghitung dan menganalisis IP address dan subnet <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/11.png" width="600">

3. Berikan perintah nmap untuk memindai jaringan <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/12.png"> <br>
   Dalam hal ini, digunakan nmap untuk memindai rentang IP address dan menampilkan IP address yang memiliki port 22 (SSH) yang terbuka. Kemudian didapatkan IP address 192.168.1.90

4. Lakukan brute force dengan nmap <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/13.png"> <br>
   <img src="../Images/Task 9 - A06 Vulnerable Component/14.png"> <br>
   Brute force dilakukan dengan mengambil list username dan list password pada folder wordlist. Namun sayangnya, tidak ditemukan pasangan username dan password yang tepat.

</div>
