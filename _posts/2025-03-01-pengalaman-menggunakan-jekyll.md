---
layout: post
title: Pengalaman Saya 3 Bulan Nge-Blog Menggunakan Jekyll
description: Pendapat saya tentang jekyll setelah menggunakannya nge-blog selama 3 bulan, tanpa tahu coding, dan pengalaman ruby sama sekali. Kelebihan dan Kekurangan jekyll menurut saya.
keywords: jekyll, membuat blog jekyll, tutorial jekyll, kelebihan jekyll, kekurangan jekyll, apa itu jekyll, ruby blog, jekyll blog
permalink: 
image: 
date: 2025-03-03
category: Jekyll
comments: true
tags:
  - blogging
  - writing
  - coding
  - jekyll
---
Bosan ngeblog menggunakan blogger, akhirnya saya memutuskan untuk mencoba CMS baru untuk ngeblog agar terasa lebih fresh, yang akhirnya mempertemukan saya dengan *[Jekyll](https://kinin.web.id)* dan Github Pages.

Berbeda dengan blogger, dengan Jekyll kita harus membuat postingan secara manual, menguploadnya dan baru mempublikasikan blog tersebut. Langkah-langkah yang cukup ribet dibandingkan dengan menggunakan platform blogger seperti *wordpress* ataupun *blogger*. Tapi disini letak keseruannya, mencoba hal baru yang sebelumnya belum saya ketahui.

Lalu, apakah saya punya pengalaman di sini sebelumnya? Tentu saja belum sama sekali, *Jekyll* menggunakan bahasa *Ruby* yang bahkan sampai sekarang belum saya pahami, membuat postingannya harus manual dengan menggunakan dokumen *Markdown* (bagian ini cukup mudah).

Dalam artikel ini saya akan menceritakan bagaimana pengalaman saya selama 3 bulan lebih menggunakan jekyll tanpa ada dasar apapun sebelumnya.

## Apa Itu Jekyll?
Jekyll adalah *static site generator* (pembangun situs statis) yang ditulis dalam bahasa Ruby. Jadi, Jekyll mirip dengan CMS blog lainnya seperti Blogger, tapi dengan Jekyll blog akan di generate menjadi situs statis. 

Jika kalian belum mengerti, mudahnya blog Jekyll itu mirip dengan kalian membuat file HTML biasa dan membukanya, berbeda dengan CMS lain yang lebih dinamis dimana setiap bagian blog diload dari server atau hosting blog. Sedangkan pada jekyll, halaman tersebut sudah dijadikan satu bagian.

## Keunggulan Jekyll dibanding Blogger 
Selama menggunakan Blog jekyll, ada beberapa kelebihan jekyll dibandingkan dengan CMS blog lainnya yang bisa saya rasakan.

1. Loading Lebih Cepat
Jekyll mengubah konten berupa file Mardown, HTML, dan file konfigurasi menjadi situs web statis, artinya, halaman web yang dihasilkan berpa file statis (HTML, CSS dan JavaScript) tanpa memerlukan basis data atau server dinamis. Sehingga proses memuat halaman jadi lebih cepat

2. Tidak Perlu Hosting Berbayar
Membuat situs jekyll kamu tidak membutuhkan hosting berbayar untuk menyimpan file blog. Beberapa situs memberikan layanan penyimpanan gratis seperti Github Pages dan Netlify (walaupun untuk netlify ada batasan untuk pengguna gratis)

3. Cukup Mudah digunakan
Butuh beberapa waktu untuk terbiasa menggunakan blog jekyll, tapi saya yakinkan lagi ini cukup mudah. 

4. Integrasi dengan Github Pages
Jekyl dan Ruby terintegrasi dengan baik dengan GitHub Pages, sehingga menghosting blog statis jekyll lebih mudah dan gratis.

5. Kostumisasi dan Template
Jekyll mendukung sistem tema dan layout yang fleksibel, memungkinkan kita untuk mendesain tampilan situs sesuai keinginan tanpa mengubah konten utama, dengan menggunakan CSS, JavaScript ataupun HTML. 

Tema jekyll juga dikembangkan oleh banyak orang yang bergabung di github, Template jekyll gratis mudah ditemukan di Internet

## Kekurangan Blog Jekyll
Selama menggunakan jekyll, beberapa kelemahan fatal yang saya temukan antara lain

1. Konten Dinamis yang Terbatas
Karena jekyll menghasilkan situs statis, fitur-fitur dinamis seperti komentar, search real-time, atau interaksi pengguna jadi sulit ditambahkan. Untuk mengatasi hal ini kita memerlukan bantuan pihak ketiga, seperti menggunakan Disqus di jekyll, menginstall komentas github, ataupun lainnya.

2. Plugin yang Terbatas
Tidak seperti Wordpress, plugin jekyll cukup terbatas. Tapi menurut saya hal ini tidak terlalu memberikan pengaruh besar untuk blog sederhana, toh Blogger saja juga memiliki plug in yang terbatas sampai sekarang.

3. Permasalahan Saat Mengganti Template Jekyll
Walaupun ada banyak pilihan template dan theme jekyll, sayangnya mengganti template yang sedang digunakan menjadi template baru cukup tricky dan sulit dilakukan.
Hal ini karena setiap template menggunakan settingan yang berbeda, dan file markdown juga terkadang menggunakan *frontmatter* yang berbeda setiap tema jekyll. Jadi, penyesuaian harus dilakukan secara manual
Tentu saja akan menjadi semakin ribet jika blog kamu sudah punya banyak postingan. 
Solusi saya, buat blog dari awal, atau pelajari CSS dan HTML untuk menyesuaikan sendiri tampilan blog menjadi seperti yang kita inginkan.

 4. Kadang Sering Terjadi Error
Karena belum cukup terbiasa dengan script, saat melakukan configurasi situs sering terjadi error uang membuat blog gagal di Build.

Oh ya, bagi kamu yang gak ngerti maksud frontmatter, jadi frontmatter itu kayak gini

```
---
layout: post
title: 
description: 
image: 
date: 
category: 
tags: 
featured:
---
```

Jekyll akan menggenerate blog kamu berdasarkan informasi tertentu, salah satunya dari frontmatter.

## Apakah Jekyll Bagus untuk Blog?
>Jadi, apakah jekyll bagus untuk blog? Jawabannya kembali kepada kebutuhan untuk apa dan seberapa besar blog yang akan dibuat.

Jika Kamu hanya ingin membuat blog sederhana berisikan postingan artikel, gambar ataupun sedikit video tanpa konten dinamis lainnya Jekyll bisa jadi jawaban untuk itu.

Jika kamu ingin membuat blog berita, pusat belanja online kemungkinan besar cukup sulit direalisasikan dengan jekyll karena butuh pengelolaan konten yang besar, walaupun bukan berarti tidak bisa sama sekali.

### Jekyll vs Blogger dan Wordpress
Jika dibuat perbandingan kasar antara lebih baik mana antara Jekyll dan Blogger atau Jekyll dan Wordpress. Jawaban saya masih sama seperti sebelumnya, semua kembali pada kebutuhan kamu, jika menginginkan blog yang mudah dikelola, tanpa perlu ribet dan gratis Blogger jadi jawabannya. Jika menginginkan web yang lebih besar dan kompleks Wordpress menjadi pilihan yang tepat. Dan bagi kamu yang menginginkan blog yang sederhana, kecil dan cepat kamu bisa mencoba menggunakan **Jekyll**

![membuat blog jekyll](/assets/img/jekyll.webp)
Jika kamu tertarik membuat blog jekyll, Kinin akan secara bertahap membagikan *[tutorial jekyll](https://kinin.web.id)* ruby untuk pemula. Karena saya harus mempelajarinya juga terlebih dahulu. 

Selain Jekyll, juga ada CMS web statis lain seperti Gosh, Hugo dan lainnya yang akan kita coba bahas dilain kesempatan, karena tentunya saya harus mempelajarinya terlebih dahulu.