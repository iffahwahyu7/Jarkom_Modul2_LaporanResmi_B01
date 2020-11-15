# Jarkom_Modul2_LaporanResmi_B01
 
Kalian diminta untuk membuat sebuah website utama dengan
 
1. alamat http://semeruyyy.pw
 
![alt text](mod2/2.png)
 
![alt text](mod2/3.png)
 
![alt text](mod2/4.JPG)
 
![alt text](mod2/pingsemeru.JPG)
 
2. alias http://www.semeruyyy.pw
 
![alt text](mod2/3.png)
 
![alt text](mod2/pingwwwsemeru.JPG)
 
3. subdomain http://www.penanjakan.semeruyyy.pw yang diatur DNS-nya pada MALANG dan mengarah ke IP Server PROBOLINGGO
 
![alt text](mod2/3.png)
 
![alt text](mod2/pingpenanjakan.JPG)
 
4. reverse domain untuk domain utama
 
![alt text](mod2/2.png)
 
![alt text](mod2/5.JPG)
 
![alt text](mod2/6.JPG)
 
5. DNS Server Slave pada MOJOKERTO
 
![alt text](mod2/3.png)
 
![alt text](mod2/7.JPG)
 
![alt text](mod2/servicebind9stop.JPG)
 
![alt text](mod2/pingsemerumojo.JPG)
 
6. subdomain dengan alamat http://gunung.semeruyyy.pw yang didelegasikan pada server MOJOKERTO dan mengarah ke IP Server PROBOLINGGO
 
![alt text](mod2/3.png)
 
![alt text](mod2/7.JPG)
 
![alt text](mod2/8.JPG)
 
7. subdomain dengan nama http://naik.gunung.semeruyyy.pw domain ini diarahkan ke IP Server PROBOLINGGO
 
![alt text](mod2/delegasi.JPG)
 
![alt text](mod2/9.JPG)
  
 
Setelah selesai membuat keseluruhan domain, kamu diminta untuk segera mengatur web server.
 
8. Domain http://semeruyyy.pw memiliki *DocumentRoot* pada /var/www/semeruyyy.pw. Awalnya web dapat diakses menggunakan alamat http://semeruyyy.pw/index.php/home.
 
![alt text](mod2/10.JPG)
  
![alt text](mod2/11.JPG)
  
![alt text](mod2/semerub01.pwindex.phphome.png)
  
9. Karena dirasa alamat urlnya kurang bagus, maka diaktifkan mod rewrite agar urlnya menjadi http://semeruyyy.pw/home
 
![alt text](mod2/12.JPG)
 
![alt text](mod2/semerub01.pwhome.png)
  
 10. Web http://penanjakan.semeruyyy.pw akan digunakan untuk menyimpan assets file yang memiliki *DocumentRoot* pada /var/www/penanjakan.semeruyyy.pw dan memiliki struktur folder sebagai berikut:
 
/var/www/penanjakan.semeruyyy.pw 
                                /public/javascripts 
                                /public/css 
                                /public/images 
                                /errors  
 

![alt text](mod2/13.JPG)
 
![alt text](mod2/16.JPG)
 
11. Pada folder /public dibolehkan directory listing namun untuk folder yang berada di dalamnya tidak dibolehkan.
 
![alt text](mod2/14.JPG)
 
![alt text](mod2/penanjakan.semerub01.pwpublic.png)
 
![alt text](mod2/penanjakan.semerub01.pwpubliccss.png)
 
![alt text](mod2/penanjakan.semerub01.pwpublicimages.png)
 
![alt text](mod2/penanjakan.semerub01.pwpublicjavascripts.png)
 
12. Untuk mengatasi HTTP Error code 404, disediakan file 404.html pada folder /errors untuk mengganti error default 404 dari Apache.
 
![alt text](mod2/17.JPG)
 
![alt text](mod2/error404.png)
 
13. Untuk mengakses file assets javascript awalnya harus menggunakan url http://penanjakan.semeruyyy.pw/public/javascripts. Karena terlalu panjang maka dibuatkan konfigurasi virtual host agar ketika mengakses file assets menjadi http://penanjakan.semeruyyy.pw/js.
 
![alt text](mod2/15.JPG)
 
![alt text](mod2/penanjakan.semerub01.pwjs.png)
 
14. sedangkan web http://naik.gunung.semeruyyy.pw sudah bisa diakses hanya dengan menggunakan port 8888. *DocumentRoot* berada pada /var/www/naik.gunung.semeruyyy.pw.
 
15. Bibah meminta kamu membuat web http://naik.gunung.semeruyyy.pw agar diberi autentikasi password dengan username “semeru” dan password “kuynaikgunung” supaya aman dan tidak sembarang orang bisa mengaksesnya.
![alt_text](mod2/nomer15-0.png)

![alt_text](mod2/nomer15.png)
16. Karena dirasa kurang profesional, maka setiap Bibah mengunjungi IP PROBOLINGGO akan dialihkan secara otomatis ke http://semeruyyy.pw.
 
![alt text](mod2/19.JPG)
 
![alt text](mod2/ip.png)
 
![alt text](mod2/semerub01.pw.png)
 
17. Karena pengunjung pada /var/www/penanjakan.semeruyyy.pw/public/images sangat banyak maka semua request gambar yang memiliki substring “semeru” akan diarahkan menuju semeru.jpg.

![alt_text](mod2/nomer16config1.png)

![alt_text](mod2/nomer16config2.png)

![alt_text](mod2/nomer16web.png)
