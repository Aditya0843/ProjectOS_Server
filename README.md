# ProjectOS_ServerAditya
Membuat Web Server menggunakan Ubuntu Versi 22.04.3
https://drive.google.com/file/d/1c_E6OgQlTXNLNRaxUaDBWtJTxunPJ6EL/view?usp=share_link
1. Web Server
OS Server
Ubuntu 22.04

Service Yang Digunakan
   -Install Apache2
   https://drive.google.com/file/d/1CV-m2OoheCQoWaiawfm7a0ptUzvbKEQD/view?usp=sharing
   -Install Mysql
   https://drive.google.com/file/d/17-JgTSKJsvSCT6izwYvxE6zgYpNx__YL/view?usp=share_link
   -Install Bind9 sebagai DNS dan Konfigurasinya
   https://drive.google.com/file/d/1axLQnrDc-jUCAcXTNZ2LRDhzmxDmmnb3/view?usp=share_link
   -Konfigurasi SSH
   https://drive.google.com/file/d/1pNDZcIGvpC4ZS9HWm7W5QQTwa4iCvrDf/view?usp=share_link
   - Install Ngrok
Step Pengerjaan
1.** Install Apache2 ** sudo apt install apache2

2.** Cek status ** sudo systemctl status apache2

3.** Cek hostname ** hostname -I

4.** Ubah pemilik folder ** sudo chown -R www-data:www-data /var/www/html

5.** Beri ijin anggota grup untuk merubah folder ** sudo chmod -R g+rw /var/www/html

6.** Tambahkan user name kita ** sudo usermod -a -G www-data

7.** Restart ubuntu **

8.** Tambahkan rule untuk apache difirewall ** sudo ufw allow 'Apache'

9.** Cek status firewall ** sudo ufw status

10.** Install ssh ** sudo apt install openssh-server

11.** Install ngrok ** snap install ngrok

12.** Masukkan token authtoken ** ngrok config add-authtoken 2ZlR0DFXPuzK2a1nMQY6ONP1FLn_4oDZYTuGDNHW3jJPJHT5R

13.** Masuk cmd ketikkan ** ssh "username"@"ip ubuntu"

14.** http 80 untuk mendapatkan url *** ngrok http 80

15.** Untuk mengedit index.html ** masuk folder /var/www/html open menggunakan texteditor
     
