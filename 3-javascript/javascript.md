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

//TODO: translate

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

## DOM Manipulation

### innerHTML

### getElementById

### getElementsByClassName

### getElementsByTagName
