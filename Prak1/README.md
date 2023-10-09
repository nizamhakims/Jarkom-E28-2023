# Jarkom-Modul-1-E28-2023
## Kelompok E28
- Shafa Nabilah Hanin / 5025211222
- Nizam Hakim Santoso / 5025211209

## Lapres Praktikum 1 
### 1. User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
#### a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 
#### b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut?
#### c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
#### d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
### Answer:
Karena aktivitasnya adalah mengupload maka cari packet dengan kata kunci “STOR”. <br>
![](Prak1/Dokumentasi/1a.png) <br>
Didapatkan sequence number dan acknowledgement number seperti berikut. <br>
![](Prak1/Dokumentasi/1b.png) <br>
Dari packet diatas kita mengetahui nama file yang dikirim adalah “c75-GrabThePisher.zip”, sehingga untuk mencari packet response kita dapat menggunakan  “GrabThePisher” sebagai kata kunci. <br>
![](Prak1/Dokumentasi/1c.png) <br>
Didapatkan sequence number dan acknowledgement number seperti berikut. <br>
![](Prak1/Dokumentasi/1d.png) <br>
Submission: <br>
![](Prak1/Dokumentasi/1e.png) <br>
<br>

### 2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
### Answer:
Gunakan ip address Portal Praktikum sebagai kata kunci filtering. <br>
![](Prak1/Dokumentasi/2a.png) <br>
Pilih salah satu packet kemudian follow tcp stream. Dapat dilihat server Portal Praktikum Jarkom adalah gunicorn. <br>
![](Prak1/Dokumentasi/2b.png) <br>
Submission: <br>
![](Prak1/Dokumentasi/2c.png) <br>
<br> 

### 3. Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
#### a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
#### b. Protokol layer transport apa yang digunakan?
### Answer:
Gunakan ip address dan port number sebagai kata kunci filtering. <br>
![](Prak1/Dokumentasi/3a.png) <br>
Jika dihitung banyaknya packet adalah 21 dan bisa dilihat bahwa protocol yang digunakan adalah UDP. <br>
Submission: <br>
![](Prak1/Dokumentasi/3b.png) <br>
<br>

### 4. Berapa nilai checksum yang didapat dari header pada paket nomor 130?
### Answer:
Cari packet nomor 130 kemudian lihat atribut checksum pada field UDP. <br>
![](Prak1/Dokumentasi/4a.png) <br>
Submission: <br>
![](Prak1/Dokumentasi/4b.png) <br>
<br>

### 5. Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
#### a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
#### b. Port berapakah pada server yang digunakan untuk service SMTP?
#### c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
### Zip:
Cari password yang dibutuhkan untuk membuka zip file yang diberikan menggunakan filtering dengan kata “zip”. <br>
![](Prak1/Dokumentasi/5a.png) <br>
Kemudian follow TCP stream dan decode password yang didapatkan. <br>
![](Prak1/Dokumentasi/5b.png) <br>
Hasil decode adalah sebagai berikut. <br>
![](Prak1/Dokumentasi/5c.png) <br>
Buka zip file dan buka txt yang ada untuk mendapatkan netcat untuk menjawab soal. <br>
![](Prak1/Dokumentasi/5d.png) <br>
### Answer:
Bisa dilihat bahwa terdapat 60 packet yang berhasil di capture dari file terlampir. <br>
![](Prak1/Dokumentasi/5e.png) <br>
Dikutip dari [Modul 1](https://github.com/arsitektur-jaringan-komputer/Modul-Jarkom/tree/master/Modul-1#12-alokasi-port) port yang digunakan untuk service SMTP adalah port 25. <br>
![](Prak1/Dokumentasi/5f.png) <br>
Dikutip dari [geeksforgeeks](https://www.geeksforgeeks.org/difference-between-private-and-public-ip-addresses/)  perbedaan private dan public ip address adalah seperti berikut. <br>
![](Prak1/Dokumentasi/5g.png) <br>
Sehingga kita bisa mengetahui public ip address dengan mencari ip address yang tidak dalam rentang private ip address seperti berikut. <br>
![](Prak1/Dokumentasi/5h.png) <br>
Submission: <br>
![](Prak1/Dokumentasi/5i.png) <br>
<br>

### 6. Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.
### Answer:
Ket: Revisi <br>
Huruf kapital pada soal tidak memenuhi kaidah penulisan KBBI, jika semua huruf kapital disusun akan membentuk kata SUBSTITUSI. <br>
![](Prak1/Dokumentasi/6a.png) <br>
Hasil pencarian “a1 e5 u21” bisa diartikan sebagai a1z26 cipher. <br>
![](Prak1/Dokumentasi/6b.png) <br>
"server SOURCE ADDRESS 7812 is invalid" merujuk pada ip source dari packet ke 7812 pada file pcapng yaitu 104.18.14.101 <br>
![](Prak1/Dokumentasi/6c.png) <br>
104.18.14.101 dapat dipisah menjadi 10 4 18 14 10 1 yang jika di decode menghasilkan JDRNJA. <br>
![](Prak1/Dokumentasi/6d.png) <br>
<br>

### 7. Berapa jumlah packet yang menuju IP 184.87.193.88?
### Answer:
Gunakan ip address sebagai kata kunci filtering
![](Prak1/Dokumentasi/7a.png) <br>
Bisa dilihat bahwa terdapat 6 packet yang menuju ip address tersebut <br>
![](Prak1/Dokumentasi/7b.png) <br>
<br>

### 8. Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
### Answer:
Filter port = 80 untuk TCP dan UDP kemudian gunakan relasi OR <br>
![](Prak1/Dokumentasi/8.png) <br>
<br>

### 9. Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
### Answer:
Filter packet yang berasal dari 10.51.40.1 dan packet yang tidak menuju ke 10.39.55.34 kemudian gunakan relasi AND <br>
![](Prak1/Dokumentasi/9.png) <br>
<br>

### 10. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
### Answer:
Gunakan “Login” sebagai kata kunci pencarian, didapatkan 1 packet dengan protocol telnet <br>
![](Prak1/Dokumentasi/10a.png) <br>
Follow TCP stream untuk melihat username dan password <br>
![](Prak1/Dokumentasi/10b.png) <br>
Dapat dilihat bahwa username adalah dhafin dan password adalah kesayangannyak0k0 <br>
![](Prak1/Dokumentasi/10c.png) <br>
<br>
