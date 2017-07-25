HUMHUB "Social Networks and Forum"
===================

<h1 align="center"><img src="http://www.comneton.com/images/logos/logo-humhub.jpg"></h1>

----------
Kelompok 14

 1. Parhan Zikkry Padly (G614140011)
 2. Rahmad Ilham Pratama (G64140016)
 3. Emiel Noor Kautsar (G64140082)
 4. Amos Tiberio Sungguraja (G64140085)
 

-------------
## Sekilas Tentang
---
Humhub ada sebuah free social network software dan framework yang dibangun untuk memberikan anda sebuah alat komunikasi dan kolaborasi yang mudah. Ini ringan, kuat dan dilengkapi dengan antarmuka yang user-friendly. Dengan HumHub Anda dapat membuat jaringan Anda sendiri disesuaikan sosial, intranet sosial atau aplikasi perusahaan sosial yang besar yang benar-benar sesuai dengan kebutuhan Anda. Meningkatkan bisnis Anda, mendukung pelanggan Anda, mengajar siswa atau mengatur klub sepak bola Anda. Ini pada Anda.

Instalasi
---

## <i class="icon-pencil">Requirement</i>


 - LAMP Server 
 - PHP CUrl Extension (w/ SSL Support) http://de1.php.net/manual/en/curl.setup.php
 - PHP Multibyte String Support http://php.net/manual/en/mbstring.setup.php
 - PHP PDO MySQL Extension (http://www.php.net/manual/en/ref.pdo-mysql.php)
 - PHP Zip Extension (http://php.net/manual/en/book.zip.php)
 - PHP EXIF Extension (http://php.net/manual/en/book.exif.php)
 - PHP INTL Extension (http://php.net/manual/en/intro.intl.php)
 - PHP FileInfo Extension (http://php.net/manual/en/fileinfo.installation.php)

## <i class="icon-pencil">Langkah instalasi Requirement awal dalam CLI.</i>

### <i class="icon-pencil">Pra Instalasi</i>
> $ sudo apt-get install lamp-server
> 
> $ sudo apt-get install php7.0-curl php7.0-gd -y 
>
> $ sudo systemctl restart apache2
>
> $ sudo systemctl enable apache2 

### <i class="icon-pencil">Instalasi HumHub</i> 
	
##### Now login to the MySQL Database to create database and user for Humhub.
> $ sudo mysql -u root -p

> $ mysql> create database humhub;
	
> $ mysql> CREATE USER 'komdat14'@'localhost' IDENTIFIED BY '123';
	
> $ mysql> GRANT ALL ON humhub.* TO 'komdat14'@'localhost';
	
> $ mysql> SET GLOBAL sql_mode= 'TRADITIONAL'
	 
> $ mysql> flush privileges;
	 
> $ mysql> exit


##### Download the Humhub package
> $ sudo wget http://liquidtelecom.dl.sourceforge.net/project/humhub/humhub-1.1.0.tar.gz

##### Move the downloaded package into the default document root of your webserver.
> $ sudo mv humhub-1.1.0.tar.gz /var/www/html
> $ sudo cd /var/www/html 

##### Extract the downloaded package by running the belowcommand.
> $ sudo /var/www/html# tar -zxvf humhub-1.1.0.tar.gz

##### Rename the directory that is created after the extraction.
> $ sudo /var/www/html# mv humhub-1.1.0 humhub


##### Set the full permissions for the HumHub directory using chmod command.
> $ sudo /var/www/html# chmod -R 777 humhub 

##### <i class="icon-pencil">Melengkapi Dependencies yang Kurang</i> 
> $sudo /var/www/html# apt-get install php7.0-intl php7.0-ldap php7.0-sq
lite php7.0-apc -y
> $ sudo systemctl restart apache2 
	
## Cara Pemaikaian

### Konfigurasi

#### 1. ini adalah halaman pertama setelah berhasil menginsttal humhub
![1](https://github.com/emielnk/projek_komdat/blob/master/image/1.PNG)
	
#### 2. Buatlah nama social network yang kalian inginkan
![2](https://github.com/emielnk/projek_komdat/blob/master/image/2.PNG)
	
#### 3. pilih konfigurasi untuk apa social medai anda
![3](https://github.com/emielnk/projek_komdat/blob/master/image/3.PNG)

#### 4. pilih konfigurasi keamanan social media anda
![4](https://github.com/emielnk/projek_komdat/blob/master/image/4.PNG)

#### 5. pilih modul-modul yang bisa digunakan di social media anda
![5](https://github.com/emielnk/projek_komdat/blob/master/image/5.PNG)

#### 6. isi form admin sesuai identitas anda dan tekan create account
![6](https://github.com/emielnk/projek_komdat/blob/master/image/6.PNG)

#### 7. konfigurasi admin selesai
![7](https://github.com/emielnk/projek_komdat/blob/master/image/7.PNG)

#### 8. login dengan akun admin yang telah anda buat sebelumnya
![8](https://github.com/emielnk/projek_komdat/blob/master/image/8.PNG)

#### 9. tampilan dashboard anda
![9](https://github.com/emielnk/projek_komdat/blob/master/image/9.PNG)
