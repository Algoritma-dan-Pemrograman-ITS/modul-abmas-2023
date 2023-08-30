**HTML**


### Daftar Isi

1. Apa itu HTML?
2. Elemen HTML
3. Jenis-jenis elemen HTML
   - `head`
   - `body`
   - `heading`
   - `paragraph`
   - `image`
   - `link`
   - ;
   - 
4. Hubungan HTML dengan CSS dan JS

### 1. Apa itu HTML?

HTML merupakan singkatan dari *Hypertext Markup Language*, yaitu bahasa markup standar untuk membuat dan menyusun halaman dan aplikasi web. HTML digunakan untuk mendefinisikan struktur dan elemen-elemen dalam halaman web, seperti teks, gambar, tautan, tabel, formulir, dan banyak elemen lainnya.

Contoh penulisan HTML sederhana adalah sebagai berikut

```
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Websiteku</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<h1>Hello World!</h1>
</body>
</html>
```

### 2. Elemen HTML

Elemen HTML terdiri dari beberapa komponen yaitu:

![elemen-html](img/html-element-diagram.png)

### 3. Jenis-Jenis Elemen HTML

**a. `head`**

Elemen `head` dalam HTML adalah bagian dari struktur dasar dari sebuah halaman web. Elemen ini berisi `metadata` dan elemen-elemen lain yang berhubungan dengan halaman web. Isi dari elemen ini tidak akan terlihat oleh pengguna, tetapi sangat penting untuk pengaturan dan optimasi halaman web.

**b. `link`**

Elemen `link` dalam HTML berfungsi untuk menghubungkan *resource* luar, biasanya stylesheet, ke dalam dokumen HTML.

**b. `body`**

Elemen `body` dalam HTML berisi semua elemen yang akan terlihat dalam halaman web.

**c. `heading`**

Elemen `heading` dalam HTML dapat dibayangkan seperti judul dan sub-judul sebuah buku. Dalam HTML, terdapat 6 macam heading mulai dari `<h1>` sampai `<h6>`. Berikut merupakan contoh penggunaan heading:
```
<h1>Hai namaku Bagas!</h1>
<h2>Hai namaku Bagas!</h2>
<h3>Hai namaku Bagas!</h3>
<h4>Hai namaku Bagas!</h4>
<h5>Hai namaku Bagas!</h5>
<h6>Hai namaku Bagas!</h6>
```

Hasil:

![elemen-heading](img/heading.png)


**d. `paragraph`**

Elemen ini digunakan untuk teks yang berupa paragraf, dilambangkan dengan tag `<p>`. Contoh penggunaannya adalah sebagai berikut:
```
<h1>Selamat datang di websiteku!</h1>
<p>Website ini adalah website terbaik di dunia</p>

```

Hasil:

![elemen-paragraph](img/paragraph.png)

**e. `image`**

Elemen ini berfungsi untuk memasang gambar kepada halaman web, dilambangkan dengan tag `<img>`. Contoh penggunaannya adalah sebagai berikut:

```

```

**f. `a`**

Elemen ini digunakan untuk memasang `hyperlink` dimana apabila ditekan dapat mengalihkan ke suatu halaman tertentu maupun sebuah website baru. Contoh penggunaannya adalah sebagai berikut:

**g. `ordered list`**

**h. `unordered list`**

-- kasih contohnya

### 4. Hubungan HTML dengan CSS dan JS
Meskipun dinyatakan sebagai bahasa markup yang canggih dan mudah, HTML tidak sepenuhnya bisa membuat website yang profesional dan responsif. Bahasa ini hanya bisa digunakan untuk menambah elemen dan membuat struktur konten.

Namun di satu sisi, bahasa ini bisa bekerja secara maksimal dengan dua bahasa frontend: CSS (Cascading Style Sheets) dan JavaScript. Jika digabungkan, kedua bahasa frontend ini bisa meningkatkan pengalaman user dan memberikan fungsi yang lebih canggih.

- CSS erat kaitannya dengan styling, seperti background, warna, layout, spacing, dan animiasi.
- JavaScript memungkinkan Anda menambahkan fungsionalitas yang dinamis, seperti slider, pop-up, dan galeri foto.

Jika digambarkan, berikut perbedaan HTML dan CSS dan JavaScript: HTML adalah orang yang tidak mengenakan busana apa pun, kemudian CSS adalah bajunya, kemudian JavaScript adalah aktivitas dan sikap orang tersebut.