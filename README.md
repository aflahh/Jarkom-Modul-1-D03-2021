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

## No 2
### Soal
Temukan paket dari web-web yang menggunakan basic authentication method!
### Penjelasan Jawaban

## No 3
### Soal
Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!
### Penjelasan Jawaban

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

## No 12
### Soal
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
### Penjelasan Jawaban

## No 13
### Soal
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
### Penjelasan Jawaban

## No 14
### Soal
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!
### Penjelasan Jawaban

## No 15
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
### Penjelasan Jawaban
