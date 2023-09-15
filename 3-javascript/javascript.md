# Javascript

## Untuk Apa JavaScript?

JavaScript adalah sebuah bahasa pemrograman yang pada umumnya dalam pemrograman web digunakan untuk menambahkan interaksi antara halaman web dengan pengguna.

### Contoh Pemakaian

- #### CodePen

  - <https://codepen.io/tofjadesign/pen/xxmdGEM>
  - <https://codepen.io/HowToSolutions/pen/ozbWKN>
  - <https://codepen.io/slc/pen/xgQPjJ>

- #### YouTube

  - <https://youtu.be/ec8vSKJuZTk?si=eHi70-wnZf33NkEM>
  - <https://youtu.be/GFO_txvwK_c?si=iisDJbWhdxEm1QDl>
  - <https://youtu.be/EOemfVmD-1M?si=5x5BRK70GlYOO96I>
  - <https://youtu.be/9EZ0TpuHYvI?si=SWXWNmTJEqK3ztNQ>
  - <https://youtube.com/shorts/ii98D1OtWfg?si=sFMT5Jep4QxvVI7p>

## Percabangan

Pada bahasa JavaScript, percabangan dapat dilakukan dengan kode berikut:

```js
if (kondisi){
    // potongan kode yang akan dijalankan
}
```

Apabila teman-teman ingin agar program teman-teman ingin melakukan sesuatu yang lain jika "kondisi" tidak terpenuhi, teman-teman dapat penggunakan *else*.

```js
if (kondisi){
    // potongan kode yang akan dijalankan
}

else {
    // potongan kode yang akan dijalankan
}
```

Contoh:

```js
let a = 5;

if (a === 5){
    console.log("a adalah 5");
}

else {
    console.log("a bukan 5");
}
```

Jika teman-teman ingin membuat percabangan lebih dari 2, teman-teman dapat menggunakan *else if*.

```js
if (kondisi){
    // potongan kode yang akan dijalankan
}

else if (kondisi_2){
    // potongan kode yang akan dijalankan
}

else {
    // potongan kode yang akan dijalankan
}
```

Contoh:

```js
let a = 5;

if (a === 5){
    console.log("a adalah 5");
}

else if (a === 3){
    console.log("a adalah 3");
}

else {
    console.log("a bukan 3 atau 5");
}
```

Apa yang dimaksud dengan **``(a === 5)``**?

Potongan kode tersebut adalah pernyataan untuk mengecek kondisi variabel **`a`** apakah bernilai **`5`** atau bukan. Pernyataan tersebut dinamakan dengan pernyataan kondisi atau *conditional statement*.

### Pernyataan Kondisi

|Operator|Description|Comparing|Returns|
|--------|-----------|---------|-------|
|==|equal to|x == 8|false|
|||x == 5|true|
|||x == "5"|true|
|===|equal value and equal type|x === 5|true|
|||x === "5"|false|
|!=|not equal|x != 8|true|
|!==|not equal value or not equal type|x !== 5|false|
|||x !== "5"|true|
|||x !== 8|true|
|>|greater than|x > 8|false|
|<|less than|x < 8|true|
|>=|greater than or equal to|x >= 8|false|
|<=|less than or equal to|x <= 8|true

## Array dan Perulangan

Array (secara harfiah adalah himpunan) adalah sebuah tipe variabel yang dapat menyimpan beberapa nilai dalam satu nama.

```js
const arr = [1, 2, 3, 6, 9];
```

> lalu, bagaimana cara kita memodifikasi nilai array?

Teman-teman dapat mengakses setiap "ruangan" pada array dengan cara seperti ini:

```js
const arr = [1, 2, 3, 6, 9];

console.log(arr[0]); // akan mengeluarkan nilai 1
console.log(arr[1]); // akan mengeluarkan nilai 2
console.log(arr[4]); // akan mengeluarkan nilai 9
```

### Perulangan Pada Array

Apabila ukuran array terlalu besar, maka akan lebih mudah menggunakan perulangan (sebuah potongan kode yang dijalankan secara berulang-ulang) daripada menulis kode yang hampir sama berkali-kali.

```js
const arr = [1, 2, 3, 6, 9];

arr.forEach((item, index) => {
    console.log(item, index);
})
```

## Manipulasi DOM

DOM (*Document Obejct Model*) adalah standardisasi dokumen seperti HTML, CSS, sehingga memungkinkan dokumen-dokumen tersebut bekerja semestinya tanpa dipengaruhi hal lain seperti komputer yang digunakan. JavaScript menawarkan manipulasi pada dokumen seperti HTML dan CSS.

### getElementById

getElementById adalah sebuah fungsi dari JavaScript untuk mendapat sebuah elemen dari HTML berdasarkan id.

|![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/039c1d57-8872-4748-8321-44206b75a6d9)|![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/aca079ec-91bf-4e73-bf56-62675520b072)|
|-|-|

Pada contoh diatas, teks "The Document Object" berwarna merah karena penggunaan fungsi getElementById.

Kode:

```html
<!DOCTYPE html>
<html>
<body>

<h1 id="demo">The Document Object</h1>
<h2>The getElementById() Method</h2>

<script>
const myElement = document.getElementById("demo");
myElement.style.color = "red";
</script>

</body>
</html>
```

### getElementsByClassName

Mirip seperti getElementById, getElementsByClassName mengambil **semua elemen** dengan class yang dimaksud, sehingga yang didapat adalah **array yang berisi beberapa elemen** ketimbang satu elemen saja.

|![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/fdc50d54-c897-470c-9374-82622bd0b05d)|![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/710a41c1-4150-49f1-8005-092a7aeca48f)|
|-|-|

Contoh diatas hampir sama dengan contoh sebelumnya.

Kode:

```html
<!DOCTYPE html>
<html>
<body>

<h1>The Document Object</h1>
<h2>The getElementsByClassName() Method</h2>

<p>Change the text of the first element with class="example":</p>

<div class="example">Element1</div>
<div class="example">Element2</div>

<script>
const collection = document.getElementsByClassName("example");
collection[0].innerHTML = "Hello World!";
</script>

</body>
</html>
```

### getElementsByTagName

Selain dengan id dan class, kita juga dapat mengambil elemen menggunakan tag pada HTML seperti body, p, dan sebagainya dengan getElementsByTagName.

|![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/cbbedf31-68b9-436d-9bc8-4e1298823e7d)|![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/be86496e-da07-4e69-87b6-e5e8d3f7f5a8)|
|-|-|

Kode:

```html
<!DOCTYPE html>
<html>
<body>

<h1>The Document Object</h1>
<h2>The getElementsByTagName() Method</h2>

<p>An unordered list:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<p>The innerHTML of the second li element is:</p>
<p id="demo"></p>

<script>
const collection = document.getElementsByTagName("li");
document.getElementById("demo").innerHTML = collection[1].innerHTML;
</script>

</body>
</html>
```

### innerHTML

Terakhir, innerHTML adalah sebuah properti pada setiap elemen yang didapat yang memudahkan kita untuk mengganti isi dari elemen yang kita dapat.

![image](https://github.com/Algoritma-dan-Pemrograman-ITS/modul-abmas-2023/assets/86661387/2df79f70-6256-482c-adec-520105d7b34c)
