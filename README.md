# Jarkom-Modul-1-C05-2022

5025201098 - Ibra Abdi Ibadihi [mengerjakan 8-10]
5025201028 - Muhammad Abror Al Qushoyy [mengerjakan 4-7]
5025201156 - Nazhifah Elqolbyi [mengerjakan 1-3]

## 1. Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
Pertama, buka file yang telah diberikan. Masukkan display command http.host == monta.if.its.ac.id
![1 1](https://user-images.githubusercontent.com/113155422/192207995-4ef170b2-56d8-499a-b04e-464a472c3a4b.PNG)
Klik kanan, follow TCP stream
![1 2](https://user-images.githubusercontent.com/113155422/192208001-d06c8d60-82c3-4678-9870-5ed591449f7b.PNG)

Server yang digunakan adalah: nginx/1.10.3

## 2. Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh Ishaq?
Buka file. Masukkan display command http.host == monta.if.its.ac.id
![1 1](https://user-images.githubusercontent.com/113155422/192208049-84295b25-c7f2-4eb2-9205-1b069194c19e.PNG)
Klik kanan, follow tcp, find topik.
![2 3](https://user-images.githubusercontent.com/113155422/192208088-f4aa696f-1c1c-451b-a26d-e0bd75c0b567.PNG)
Ditemukan link berikut http://monta.if.its.ac.id/index.php/topik/detailTopik/194
![2 4](https://user-images.githubusercontent.com/113155422/192208110-5a950044-a6a8-42c2-b46b-1d6a96dd4914.PNG)

Maka topik tugas akhir yang didapat Ishaq berjudul Evaluasi Unjuk Kerja User Space Filesystem (FUSE) oleh Wahyu Suadi.
## Filter sehingga wireshark hanya menampilkan paket yang menuju port 80! 
Pada display filter input command “tcp.dstport == 80”
![3](https://user-images.githubusercontent.com/113155422/192208393-5139f49a-cc43-4b55-b4cf-ef691b711054.PNG)

## 4. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!
Pada display filter input command “tcp.srcport == 21”
![4](https://user-images.githubusercontent.com/113155422/192208465-dd4ea249-e10d-4df4-99b0-10c9a3465bde.PNG)

## 5. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!
Pada display filter input command “tcp.srcport == 443”
![5](https://user-images.githubusercontent.com/113155422/192208481-0824f695-9f85-4088-b3cb-1a77c2552261.PNG)

## 6. Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !
Isi capture filter dengan: dst host lipi.go.id
![6 1](https://user-images.githubusercontent.com/113155422/192208510-80afecea-d5bc-4e01-864c-7725c0b461ab.PNG)


## 7. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
Isi capture filter dengan: src host <ip saya>
Contoh yang (bukan) ip saya sendiri
![7 1](https://user-images.githubusercontent.com/113155422/192208542-77a2e514-688c-435f-a26f-bc46b4f25c0b.PNG)

 
## 8. Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.
Filter display dengan : frame contains "soal" , lalu follow TCP stream-nya sehingga ketemu sebagai berikut.
![8 1](https://user-images.githubusercontent.com/113155422/192208591-fe95bf09-3f1a-4032-9b7f-9246e572197f.PNG)

## 9. Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.
  
Dari petunjuk yang diberikan, kita cari file yang ada “9002”-nya. Yang ada unsur 9002nya di file hanyalah kolom info dan kolom info tidak bisa difilter (atau setidaknya saya yang nggak bisa) sehingga terpaksa mengklik satu-satu seperti manusia zaman purba.
Setelah dihujani link koplo cat dan mas-mas indihom, akhirnya didapatkanlah file tersebut.
![9 1](https://user-images.githubusercontent.com/113155422/192208750-da9683e1-784d-4e9f-abca-d7fced770b0c.PNG)

Lalu save as raw biar bisa didekode. Didapatkanlah file berikut.
https://anonfiles.com/l1c5Md88y3/C05_des3
  
## 10. Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
Sesuai petunjuk, kita diminta mendekode file menggunakan openssl dan metode yang tertera. 
Namun, kita butuh password terlebih dahulu.
![10 1](https://user-images.githubusercontent.com/113155422/192208818-2f9cf530-6930-4f80-8d4c-5552e53c4e0b.PNG)

Setelah mendapatkan password, kita bisa melakukan dekode file sehingga didapatkanlah file berikut.
![10 2](https://user-images.githubusercontent.com/113155422/192208833-c13537bb-c23e-4e83-a8b0-5b506e60b570.PNG)


