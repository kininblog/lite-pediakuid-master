---
layout: post
title: Cara Membuat dengan Blog Jekyll dan Github Pages
description: Untuk membuat blog di Jekyll sangat mudah, bahkan bagi pemula sekalipun. Kamu hanya perlu mengikuti panduan beberapa langkah untuk membuat blog jekyll, mempostingnya di github dan blog jekyll mu sudah jadi.
permalink: 
image: 
date: 2025-03-03
category: Jekyll
tags:
  - blogging
  - writing
  - coding
  - jekyll
---
**[Kinin](https://kinin.web.id) -** Untuk membuat blog di Jekyll sangat mudah, bahkan bagi pemula sekalipun. Kamu hanya perlu mengikuti panduan beberapa langkah untuk membuat blog jekyll, mempostingnya di github dan blog jekyll mu sudah jadi. 

Sebelumnya saya sudah menceritakan sedikit pengalaman selama *[menggunakan blog jekyll](https://kinin.web.id/pengalaman-menggunakan-jekyll/)* yang juga sudah membahas sedikit tentang apa itu jekyll, keunggulan dan kekurangan jekyll. Kamu bisa baca lebih lanjut di artikel kemarin.

Sesuai janji sebelumnya, kali ini Kinin akan membahas dan memberikan sebuah panduan lengkap memulai dan membuat blog jekyll di github pages ataupun melalui Local host. Saya akan berusaha membuat panduan ini sesederhana mungkin, anggap saja kita semua pemula dan belum ada dasar sama sekali. Ayo kita mulai panduan membuat blog jekyll.
![membuat blog jekyll](/assets/img/jekyll.webp)

## Apa itu Jekyll
Jekyll adalah static site generator (pembangun situs statis) yang ditulis dalam bahasa Ruby. Jadi, Jekyll mirip dengan CMS blog lainnya seperti Blogger, tapi dengan Jekyll blog akan di generate menjadi situs statis.

Jika kalian belum mengerti, mudahnya blog Jekyll itu mirip dengan kalian membuat file HTML biasa dan membukanya, berbeda dengan CMS lain yang lebih dinamis dimana setiap bagian blog diload dari server atau hosting blog. Sedangkan pada jekyll, halaman tersebut sudah dijadikan satu bagian.

## Software yang dibutuhkan
Untuk membuat blog jekyll, setidaknya kamu harus memiliki seperangkat laptop ataupun PC, serta beberapa software tambahan yang akan kita gunakan.
1. VSCode, Microsoft Visual Code atau VSCode digunakan untuk mempermudah proses mengelola blog Jekyll yang akan dibuat, agar lebih terorganisir. Pelajar *cara install visual code* di windows kamu
2. Ruby, Jekyll berjalan dalam bahasa program Ruby, jadi terlebih dahulu kita harus menginstall bahasa Ruby di laptop atau perangkat yang akan kita gunakan. Kinin akan membuat panduan lain terkait *cara install ruby di windows* pada artikel selanjutnya
3. GitHub Desktop, dengan github desktop akan lebih mudah membuat dan mengupdate repository github kita. Pelajari cara *install github desktop* 

## Hal yang Perlu diperhatikan Sebelum Membuat Blog Jekyll
Selama menggunakan jekyll, saya menemukan kelemahan fatal yaitu mengganti template jekyll yang sangat ribet dan butuh waktu lama. Untuk itu, sebelum memulai blog baru cari dan tentukan tema jekyll yang ingin kamu gunakan berdasarkan topik blog atau yang sekiranya kamu gak bakal ganti-ganti tema lagi.

>Percaya lah! Mengganti tema satu ketema lainnya di jekyll itu ribet banget. Jadi perhatikan ini baik-baik

## Membuat Blog Jekyll dengan Template Default
Setelah menginstall semua software yang dibutuhkan, kita lanjut ke step selanjutnya. Untuk membuat blog dengan jekyll cara pertama yaitu dengan langsung menggunakan template default atau template bawaan jekyll bernama minima. Untuk membuat blog ini cukup menggunakan Visual Studio Code.

1. Buat sebuah folder di komputer kamu tempat menyimpan semua blog. 
2. Buka visual code, kemudian tarik folder yang kamu buat ke visual code
3. Buka `terminal` visual code dengan cara tekan `CTRL + SHIFT + ~` di keyboard
4. Ketikkan script
```
gem install jekyll bundler
```
5. Kemudian 
```
jekyll new myblog
```
>`myblog` adalah nama folder blog kamu, bisa ubah dengan nama lain yang kamu inginkan

6. Selanjutnya menyimpannya ke directory
```
cd myblog
```
> Jika kamu menginstall Ruby versi terbaru langkah 6 ini tidak diperlukan

7. Langkah 5 tadi akan otomatis membuat file blog kamu, untuk melihat tampilan blog ketikkan perintah berikut di terminal.
```
bundle exec jekyll serve
```
>Blog akan otomatis di generate, untuk melihatnya buka Browser dan ketikkan `http://localhost:4000/` maka blog akan otomatis terbuka.


## Membuat Blog Jekyll dengan Template Lain
Pilihan kedua, kamu bisa membuat blog jekyll dengan menggunakan template pilihan. Silahkan cari saja tema jekyll yang kamu ingin gunakan di internet, banyak tema gratis yang bisa di download, atau jika kamu punya modal juga bisa membeli template jekyll premium.

Saran saya, gunakan tema blog yang benar-benar ingin kamu gunakan. Cek template apakah sudah responsive dan cepat, serta struktur data yang baik. Jika sudah, kita lanjut ke tahap selanjutnya
1. Jika kamu menggunakan github, fork template yang ingin kamu gunakan
2. Buka Github Desktop dan login
3. Kemudian clone respository yang sudah di fork tadi ke komputer kamu
4. Drag folder repository yang di clone ke visual code untuk membukanya
5. Kemudian pilih folder `Gemfile` dan ketikan perintah berikut di visual code
```
bundle installl
```
6. Tunggu proses install selesai, gunakan perintah berikut untuk melihat blog
```
bundle exec jekyll s
```
7. Buka blog di localhost seperti sebelumnya
8. Langkah selanjutnya, silahkan sesuaikan blog kamu mulai dari judul dan informasi lainnya dengan cara mengedit isi file `_config.yml` pada folder blog tadi.


## Rekomendasi Template Jekyll
Beberapa rekomendasi template jekyll gratis yang bisa kamu gunakan dan dapat dijadikan bahan pertimbangan dari [kinin](https://kinin.web.id) seperti

### 1. Mediumish
Mediumish - Tema Jekyll adalah tema blog bergaya Medium yang dibangun dengan Bootstrap 4. Tema ini bersih, modern, cocok untuk blog atau majalah, dan mendukung banyak penulis.

Fitur seperti Google Analytics, komentar Disqus, paginasi, serta arsip kategori menjadikannya solusi Jekyll yang lengkap untuk blogging. Selain itu, tema ini juga kompatibel dengan GitHub Pages, sehingga Anda dapat menghostingnya secara gratis di GitHub!

### 2. Mundana
Mundana adalah tema Jekyll gratis yang dirancang untuk penggemar desain situs web Medium.

Dibuat dengan indah, Mundana adalah pilihan sempurna untuk blog Jekyll Anda. Tersedia berbagai tata letak seperti beranda, pencarian, artikel, dan kategori. Sepenuhnya kompatibel dengan GitHub Pages.

## Kesimpulan
Membuat blog jekyll merupakan sebuah tantangan dalam blogging, kamu harus melakukannya secara manual. Tapi disitu letak keseruannya dibanding ngeblog dengan cara biasa. Cara membuat blog jekyll pun juga cukup simpel, cepat dan gratis 100%. 

Selain itu, blog jekyll juga bisa di costumisasi dengan mudah jika kamu bisa menggunakan css dan html.