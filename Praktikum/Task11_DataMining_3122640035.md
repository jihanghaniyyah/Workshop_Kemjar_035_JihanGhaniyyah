<div class="cover" align="center">

<h3>
    <b>PRAKTIKUM KEAMANAN JARINGAN</b><br>
    "DATA MINING USING KNIME"
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

<hr> <br>

<b><h3 align="center"> DATA MINING USING KNIME </h3></b><br>

1.  Bagi File menjadi 5 bagian : init.pcap, init2.pcap, init3.pcap, init4.pcap, init5.pcap <br>
    <img src="../Images/Task 10 - A10 A11/6.png" alt="" width="600"><br>
2.  Kemudian buka file tersebut secara bergantian menggunakan Wireshark. Pada langkah ini kita gunakan file init.pcap <br>
    <img src="../Images/Task 10 - A10 A11/7.png" alt="" width="600"><br>
3.  Untuk proses analisis yang akan dilakukan nantinya, kita akan mengambil data dengan ip versi 4 (ipv4) dan protocol TCP, DNS saja. Untuk proses tersebut dapat dilakukan pada wireshark menggunakan perintah ip.version==4 && tcp || dns pada kolom display filter tepat dibawah toolbar <br>
    <img src="../Images/Task 10 - A10 A11/8.png" alt="" width="600"><br>
4.  Untuk mendapatkan delta time dan delta time dan delta time display, klik Edit – Preferences – Column
    <img src="../Images/Task 10 - A10 A11/9.png" alt="" width="600"><br>
    Hasilnya <br>
    <img src="../Images/Task 10 - A10 A11/10.png" alt="" width="600"><br>
5.  Export file pcap tersebut keformat Comma-separated Value (.csv) dengan cara klik File – Export Packet Dissections – As CSV. Yang perlu diperhatikan yaitu pada Pacet Range, pastikan yang terpilih yaitu Displayed, karena data pada Displayed ini sudah terfilter denga nip version 4 <br>
    <img src="../Images/Task 10 - A10 A11/11.png" alt="" width="600"><br>
    <img src="../Images/Task 10 - A10 A11/12.png" alt="" width="600"><br>
6.  Membuat workflow/project baru. Dengan cara klik File – New – New Knime Workflow – Tulis Nama workflow dan Lokasi workflow tersebut – Klik Finish <br>
    <img src="../Images/Task 10 - A10 A11/13.png" alt="" width="600"><br>
7.  Tambahkan data ke dalam file reader <br>
    <img src="../Images/Task 10 - A10 A11/14.png" alt="" width="600"><br>
8.  Gabungkan kelima data dengan menggunakan concatenate dan data reader seperti gambar di bawah <br>
    <img src="../Images/Task 10 - A10 A11/15.png" alt="" width="600"><br>
9.  Untuk melakukan labeling data normal kita akan menggunakan Node Missing Value. Node ini digunakan untuk mengisi data kosong <br>
    <img src="../Images/Task 10 - A10 A11/16.png" alt="" width="600"><br>
10. Untuk memastikan bahwa kolom label sudah terisi dengan value Malicious atau Normal, dapat menggunakan node Value Counter. Node ini berfungsi untuk menghitung jumlah seluruh value pada kolom terpilih. <br>
    <img src="../Images/Task 10 - A10 A11/17.png" alt="" width="600"><br>
11. Export file ke dalam format .csv dengan menggunakan node CSV Writer <br>
    <img src="../Images/Task 10 - A10 A11/18.png" alt="" width="600"><br>
    Data diletakkan di dalam file hasil.csv <br>
    <img src="../Images/Task 10 - A10 A11/19.png" alt="" width="600"><br>
12. Data pre-processing <br>
    Proses dimana data akan dibersihkan (cleaning) karena biasanya didalam suatu data terdapat nilai-nilai yang tidak sempurna atau bahkan terdapat nilai-nilai yang hilang atau kosong yang nantinya akan dapat mempengaruhi proses kedepannya. Pada proses ini kita membutuhkan Node-node berikut : File Reader, Column Filter, Missing Value. <br>
    <img src="../Images/Task 10 - A10 A11/20.png" alt="" width="600"><br>
13. Proses data transformation, pada proses ini data akan diubah ke format yang sesuai untuk proses data mining. Node yang digunakan pada tahap ini yaitu Normalizer. Berikut konfigurasinya: <br>
    <img src="../Images/Task 10 - A10 A11/21.png" alt="" width="600"><br>
14. Data Mining <br>
    Setelah menyelesaikan tahap data transformation, kita akan menjalankan proses Data Mining, dalam proses ini kita akan menggunakan Metode Klasifikasi Decision Tree dengan teknik Cross Validation. Pada proses ini kita membutuhkan Node-node berikut : X-Partitioner, Decision Tree Learner, Decision Tree Predictor, X-Aggregator Sehingga akan membentuk flow seperti ini <br>
    <img src="../Images/Task 10 - A10 A11/22.png" alt="" width="600"><br>
15. Node Scorer yang didalamnya terdapat perhitungan untuk melihat seberapa baik model ini dengan menggunakan teknik confusion matrix. Berikut konfigurasinya. <br>
    <img src="../Images/Task 10 - A10 A11/23.png" alt="" width="600"><br>
16. Hasil prediksi <br>
    <img src="../Images/Task 10 - A10 A11/24.png" alt="" width="600"><br>

</div>
