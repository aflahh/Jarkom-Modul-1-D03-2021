# Jarkom-Modul-1-D3-2021

- Zahrotul Adillah (05111940000139)
- Muhammad Nur Abdurrauf (05111940000140)
- Aflah Hilmy (05111940000177)

## Daftar Isi

- [No 1](#no-1)
- [No 2](#no-2)
- [No 3](#no-3)
- [No 4](#no-4)
- [No 5](#no-5)
- [No 6](#no-6)
- [No 7](#no-7)
- [No 8](#no-8)
- [No 9](#no-9)
- [No 10](#no-10)
- [No 11](#no-11)
- [No 12](#no-12)
- [No 13](#no-13)
- [No 14](#no-14)
- [No 15](#no-15)

## No 1
### Soal
Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! 
### Penjelasan Jawaban
- Menggunakan display filter 'http.src == "ichimarumaru.tech"'. kemudian pilih baris paling atas > klik kanan > pilih **Follow** > **TCP Stream**
![image](https://user-images.githubusercontent.com/72771774/134763283-367f7a1a-a71c-4412-94ce-f553e3b86f67.png)

- Maka akan terbuka informasi seperti berikut :
![image](https://user-images.githubusercontent.com/72771774/134763354-847ada63-b6f9-43ce-92d7-eddd87953c37.png)
Dari informasi di atas, dapat ditemukan bahwa server yang digunakan adalah `Server: nginx/1.18.0 (Ubuntu)`

## No 2
### Soal
Temukan paket dari web-web yang menggunakan basic authentication method!
### Penjelasan Jawaban
Untuk menemukan paket dari web-web yang menggunakan basic authentication method, kita bisa menggunakan display filter `http.authbasic`. Untuk hasilnya bisa dilihat pada gambar di bawah ini : 
![image](https://user-images.githubusercontent.com/72771774/134763384-1a5b6ba3-7c31-48fe-b2e1-2b440c59c39a.png)

## No 3
### Soal
Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!
### Penjelasan Jawaban
- Masukkan display filter `http.host contains "basic.ichimarumaru.tech"', lalu akan muncul seperti ini :
![image](https://user-images.githubusercontent.com/72771774/134763495-79bbc913-3b6b-4595-81a8-c7a9433a69d0.png)

- Pilih baris **Hypertext Transfer Protocol** > **Authorization**, maka pada bagian **Credential** akan terdapat user dan password untuk akses web `basic.ichimarumaru.tech`
![image](https://user-images.githubusercontent.com/72771774/134763610-be89a73b-f51a-4827-85d3-6df897f62ddd.png)

- Masukkan username dan passwordnya ke web `basic.ichimarumaru.tech`. Isi jawaban lalu screenshoot.
![image](https://user-images.githubusercontent.com/72771774/134763719-a610bcf4-2797-4564-a215-a037f4bf57c3.png)

## No 4
### Soal
Temukan paket mysql yang mengandung perintah query select!
### Penjelasan Jawaban
Dengan menggunakan display filter "mysql.query contains "select"". Terdapat 2 paket mysql yang mengandung query select.
![image](https://user-images.githubusercontent.com/74708771/134757362-6fe528a8-8d31-4610-8a34-664acab5bdf4.png)

Hasilnya adalah 2 query select berikut ini:
![image](https://user-images.githubusercontent.com/74708771/134757380-81a3d59d-4cdb-4938-8b4c-2a832a6a0f6e.png)
![image](https://user-images.githubusercontent.com/74708771/134757385-b12e474e-15d0-4906-a73c-16376de3b767.png)

Untuk nomer ini tidak ada kendala dalam pengerjaan.

## No 5
### Soal
Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!
### Penjelasan Jawaban
Mencari username dan password terlebih dahulu dengan menggunakan display filter "mysql.query contains "INSERT"". Terdapat 1 paket mysql yang mengandung query insert.
![image](https://user-images.githubusercontent.com/74708771/134757507-54f1a33d-1f90-49a6-bc00-ec5e3a4e33ee.png)

Hasilnya adalah usename dan password sebagai berikut:

username : akakanomi

password : pemisah4lautan

![image](https://user-images.githubusercontent.com/74708771/134757541-f33fcc29-065e-4cb8-9d52-f3b2526fe568.png)

Setelah itu membuka website yang terdapat di soal dan login. Lalu didapatkan soal seperti berikut:
![image](https://user-images.githubusercontent.com/74708771/134757560-7887f4eb-6a9e-4b1b-a691-e495ed6fd4a4.png)
Jawaban dari soal di atas adalah : Putih & Oranye - Oranye - Putih & Hijau - Biru - Putih & Biru - Hijau - Putih & Coklat - Coklat

Kendala dalam pengerjaan pada saat mencoba display filter "mysql.query contains "insert"" tidak ditemukan hasil yang diinginkan.
![image](https://user-images.githubusercontent.com/74708771/134757632-1cd399d1-45fd-4cea-9341-af5b45deba39.png)

## No 6
### Soal
Cari username dan password ketika melakukan login ke FTP Server!
### Penjelasan Jawaban
Dengan menggunakan display filter "ftp.request.command == USER or ftp.request.command == PASS"
![image](https://user-images.githubusercontent.com/74708771/134757842-0c525924-577c-426e-b3dd-b86da95178fe.png)

Hasilnya adalah usename dan password sebagai berikut:

username : secretuser

password : aku.pengen.pw.aja

Untuk nomer ini tidak ada kendala dalam pengerjaan.

## No 7
### Soal
Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")
### Penjelasan Jawaban
- Memasukkan display filter `ftp-data contains Real.pdf`
![image](https://user-images.githubusercontent.com/72771774/134764437-c4ebc21f-cc66-40a5-bca8-be8c2e78c915.png)

- Pilih baris paling atas > klik kanan > pilih Follow > TCP Stream lalu ganti `ASCII` menjadi `Raw` lalu simpan filenya
![image](https://user-images.githubusercontent.com/72771774/134764462-1b488575-2d5b-4dcc-9d6a-369dd8304538.png)

- Berikut tampilan file Real.pdf ketika dibuka 
![image](https://user-images.githubusercontent.com/72771774/134763877-cb373d23-66f9-4a89-8e73-9584d546d790.png)


## No 8
### Soal
Cari paket yang menunjukan pengambilan file dari FTP tersebut!
### Penjelasan Jawaban
Untuk mencari paket yang menunjukkan pengambilan file dari FTP ditandai dengan command "RETR". Maka dengan menggunakan display filter "ftp.request.command == "RETR"" didapatkan hasil berikut:
![image](https://user-images.githubusercontent.com/74708771/134757991-a635ee69-3ac9-4ab4-a373-9ba1662b4a40.png)

Kendala dalam pengerjaan soal ini adalah tidak ditemukannya hasil yang diingikan. Tetapi jika menggunakan "ftp.request.command == "STOR"" yaitu command penyimpanan file di FTP akan didapatkan hasil seperti berikut:
![image](https://user-images.githubusercontent.com/74708771/134758085-9ef736f6-2409-464c-9083-eab4f8c355fe.png)

## No 9
### Soal
Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!
### Penjelasan Jawaban
- Memasukkan filter `ftp-data.command ~ "secret.zip"`
![image](https://user-images.githubusercontent.com/72771774/134764298-1f1f465e-dc02-4e66-8fd8-0f3bf49139a9.png)

- Lalu klik kanan yang paling atas follow ->TCP Stream. Data disimpan sebagai Raw.
![image](https://user-images.githubusercontent.com/72771774/134764321-7c2424ca-cb3a-450d-b9d2-e15dff26edb8.png)

- Memasukkan password dari hasil nomor 10
![image](https://user-images.githubusercontent.com/72771774/134764356-3bc39fbd-a723-41a9-9683-2f50f8097590.png)

- Berikut adalah isi dari Wanted.pdf yang ada di dalam file secret.zip :
![image](https://user-images.githubusercontent.com/72771774/134764375-34d96ef9-3ead-4b12-b2b7-da5051017e24.png)

## No 10
### Soal
Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!
### Penjelasan Jawaban
Dengan menggunakan display filter "ftp-data contains "history"" ditemukan file history.txt
![image](https://user-images.githubusercontent.com/74708771/134758223-67a15c15-0b45-4f96-8636-850ac865479e.png)

Isi dari file history.txt mengarah ke file lain yaitu bukanapaapa.txt
![image](https://user-images.githubusercontent.com/74708771/134758237-1d5633c3-5ce5-4ef8-8b47-33330a66fa78.png)

Dengan menggunakan display filter "ftp-data contains "bukanapaapa"" ditemukan file bukanapaapa.txt
![image](https://user-images.githubusercontent.com/74708771/134758271-13060aeb-3c6a-4298-8cc2-4dd15fb97ea4.png)

Isi dari file bukanapaapa.txt adalah sebagai berikut
![image](https://user-images.githubusercontent.com/74708771/134758301-0f13e878-2e80-4fa2-b3db-869dc55be019.png)

Sehingga didapatkan password untuk file secret.zip adalah "d1b1langbukanapaapajugagapercaya"

Untuk nomer ini tidak ada kendala dalam pengerjaan.

## No 11
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80! 
### Penjelasan Jawaban
Karena di soal disebutkan "mengambil", maka menggunakan capture filter `src port 80`. Ketika dicoba membuka website yang menggunakan protokol http, maka akan menangkap paket tersebut seperti di gambar berikut:
![soal11](https://user-images.githubusercontent.com/29938033/134765868-e3a4b945-63ba-4e55-a94f-085c95a2c807.png)


## No 12
### Soal
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
### Penjelasan Jawaban
Mirip seperti soal 11, menggunakan capture filter `port 21`. Ketika dicoba menghubungkan ke ftp server, akan menangkap paket seperti gambar berikut:

![soal12](https://user-images.githubusercontent.com/29938033/134765913-d60e31f9-56f5-4627-a098-47d069d0b7e3.png)

## No 13
### Soal
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
### Penjelasan Jawaban
Karena disebutkan "menampilkan", maka menggunakan display filter `tcp.dstport == 443`. Ketika dicoba membuka website yang menggunakan protokol https, akan menampilkan paket seperti gambar berikut:

![soal13](https://user-images.githubusercontent.com/29938033/134765954-5eb0119c-00ef-4142-8498-308485c19d07.png)

## No 14
### Soal
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!
### Penjelasan Jawaban
Mirip seperti soal 11 dan 12, menggunakan capture filter `dst host kemenag.go.id`. Ketika dicoba membuka [kemenag.go.id](http://kemenag.go.id/), maka akan menangkap paket seperti di gambar berikut:

![Capture](https://user-images.githubusercontent.com/29938033/134766316-fe964395-7441-46f5-bffa-4923971c4903.PNG)

## No 15
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
### Penjelasan Jawaban
Untuk mengetahui ip kita, kita bisa menjalankan `ipconfig` di cmd/terminal lalu melihat IPv4 Address seperti di gambar berikut:

![soal15a](https://user-images.githubusercontent.com/29938033/134765973-5292b65a-7ca0-4980-8082-b842640dfa39.jpeg)

Setelah mengetahui ip komputer kita, dalam kasus ini ip-nya `192.168.43.241`, di Wireshark digunakan capture filter `src host 192.168.43.241`. Ketika dicoba membuka website apapun, akan menangkap paket seperti berikut:

![soal15b](https://user-images.githubusercontent.com/29938033/134765980-2ecba9af-6ac0-4031-8cc7-03e9dd009c47.png)
