# Git 
Git merupakan perangkat lunak pengendali versi atau proyek manajemen kode perangkat lunak yang diciptakan oleh Linus Torvalds, yang pada awalnya ditujukan untuk pengembangan kernel Linux.

## Cara install Git
1. Download git-scm di website resmi nya https://git-scm.com/downloads
2. Jika menggunakan arch based linux bisa dengan command
````
    sudo pacman -S git
````
3. Cek versi git
````
    git --version
````

## Cara Penggunaan Git
1. Konfigurasi terlebih dahulu username dan email pada global repository-nya
````
git config --global user.name “nama_user”
````
````
git config --global user.email “email_user”
````

2. Buat repository local
````
mkdir bahasa_pemrograman
````
````
cd bahasa_pemrograman
````
````
mkdir praktikum1
````

3. Jika sudah, jalankan command (command git init digunakan untuk menginisialisasi repositori git baru)
````
git init
````

## Menambahkan File Baru Pada Repository Lokal
1. Untuk membuat file baru bisa juga dengan text editor

disini akan menggunakan terminal
````
echo # Latihan 1 >> README.md
````

2. Untuk menambahkan file yang baru saja dibuat, gunakan command
````
git add README.md
````

3. Untuk menyimpan perubahan yang ada pada database repositori 
lokal, gunakan command
````
git commit -m
````

## Membuat Repository Server

1. Server repository yang digunakan adalah github
2. Buat akun github terlebih dahulu
3. Klik tombol + new repository
4. Isi nama repository-nya,
````
   contoh: praktikum1
````
5. lalu klik tombol Create repository

## Menambahkan Remote Repository
* Remote Repository merupakan  server repositori yang akan  digunakan untuk menyimpan segala perubahan yang dilakukan pada repositori lokal, dan bisa diakses oleh banyak pengguna
* Untuk menambahkan remote repository server, gunakan command
````
git remote add origin [url]
````

## Mengirim perubahan ke server (Push)
* Untuk mengirim perubahan pada repositori lokal ke server, gunakan command
````
git push -u origin master
````

## Clone Repository
* git clone digunakan untuk mengambil salinan dari repositori Git dari server ke repositori lokal
* gunakan command ini untuk melakukan kloning ke repositori lokal
````
git clone [url]
````
