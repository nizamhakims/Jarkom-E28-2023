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
![](Dokumentasi/1a.png) <br>
Didapatkan sequence number dan acknowledgement number seperti berikut. <br>
![](Dokumentasi/1b.png) <br>
Dari packet diatas kita mengetahui nama file yang dikirim adalah “c75-GrabThePisher.zip”, sehingga untuk mencari packet response kita dapat menggunakan  “GrabThePisher” sebagai kata kunci. <br>
![](Dokumentasi/1c.png) <br>
Didapatkan sequence number dan acknowledgement number seperti berikut. <br>
![](Dokumentasi/1d.png) <br>
Submission: <br>
![](Dokumentasi/1e.png) <br>
<br>

### 2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
### Answer:
Gunakan ip address Portal Praktikum sebagai kata kunci filtering. <br>
![](Dokumentasi/2a.png) <br>
Pilih salah satu packet kemudian follow tcp stream. Dapat dilihat server Portal Praktikum Jarkom adalah gunicorn. <br>
![](Dokumentasi/2b.png) <br>
Submission: <br>
![](Dokumentasi/2c.png) <br>
<br> 

### 3. Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
#### a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
#### b. Protokol layer transport apa yang digunakan?
### Answer:
Gunakan ip address dan port number sebagai kata kunci filtering. <br>
![](Dokumentasi/3a.png) <br>
Jika dihitung banyaknya packet adalah 21 dan bisa dilihat bahwa protocol yang digunakan adalah UDP. <br>
Submission: <br>
![](Dokumentasi/3b.png) <br>
<br>

### 4. Berapa nilai checksum yang didapat dari header pada paket nomor 130?
### Answer:
Cari packet nomor 130 kemudian lihat atribut checksum pada field UDP. <br>
![](Dokumentasi/4a.png) <br>
Submission: <br>
![](Dokumentasi/4b.png) <br>
<br>

### 5. Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
#### a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
#### b. Port berapakah pada server yang digunakan untuk service SMTP?
#### c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
### Zip:
Cari password yang dibutuhkan untuk membuka zip file yang diberikan menggunakan filtering dengan kata “zip”. <br>
![](Dokumentasi/5a.png) <br>
Kemudian follow TCP stream dan decode password yang didapatkan. <br>
![](Dokumentasi/5b.png) <br>
Hasil decode adalah sebagai berikut. <br>
![](Dokumentasi/5c.png) <br>
Buka zip file dan buka txt yang ada untuk mendapatkan netcat untuk menjawab soal. <br>
![](Dokumentasi/5d.png) <br>
### Answer:
Bisa dilihat bahwa terdapat 60 packet yang berhasil di capture dari file terlampir. <br>
![](Dokumentasi/5e.png) <br>
Port yang digunakan untuk service SMTP adalah port 25. <br>
![](Dokumentasi/5f.png) <br>
Dikutip dari https://www.geeksforgeeks.org/difference-between-private-and-public-ip-addresses/ perbedaan private dan public ip address adalah seperti berikut. <br>
![](Dokumentasi/5g.png) <br>
Sehingga kita bisa mengetahui public ip address dengan mencari ip address yang tidak dalam rentang private ip address seperti berikut. <br>
![](Dokumentasi/5h.png) <br>
Submission: <br>
![](Dokumentasi/5i.png) <br>
<br>

### 6. Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.
### Answer:
<br>

### 7. Berapa jumlah packet yang menuju IP 184.87.193.88?
### Answer:
<br>

### 8. Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
### Answer:
<br>

### 9. Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
### Answer:
<br>

### 10. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
### Answer:
<br>
