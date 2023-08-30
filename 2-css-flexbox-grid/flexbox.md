**Pembelajaran Flexbox CSS**

Flexbox (Flexible Box) adalah teknik tata letak dalam CSS yang memungkinkan Anda mengatur tata letak elemen dalam satu dimensi (baris atau kolom) dengan cara yang lebih mudah dan responsif. Dalam tutorial ini, kita akan menjelaskan konsep dasar Flexbox dan cara menggunakannya.

### Daftar Isi

1. Pengenalan ke Flexbox
2. Display dan Container Flexbox
3. Properti Utama Flex Container
   - `flex-direction`
   - `justify-content`
   - `align-items`
   - `align-content`
4. Properti Flex Item
   - `flex`
   - `align-self`
   - `order`
5. Penggunaan Flexbox dalam Kasus Sederhana
6. Responsif dengan Flexbox
7. Tips dan Trik

### 1. Pengenalan ke Flexbox

Flexbox adalah teknik tata letak yang sangat berguna dalam desain web responsif. Ini memberikan cara lebih mudah untuk mengatur posisi dan ukuran elemen dalam satu dimensi (baris atau kolom) sehingga membuat tampilan web lebih fleksibel dan teratur.

### 2. Display dan Container Flexbox

Pertama, Anda perlu mendefinisikan elemen induk yang akan menjadi wadah (container) untuk elemen-elemen yang akan diatur menggunakan Flexbox. Anda melakukannya dengan mengubah properti `display` dari elemen tersebut.

```css
.container {
  display: flex; /* Mengubah elemen menjadi container Flexbox */
}
```

### 3. Properti Utama Flex Container

**a. `flex-direction`**

Properti ini menentukan arah tata letak elemen dalam container Flexbox. Ada empat nilai yang bisa diaplikasikan: `row`, `row-reverse`, `column`, dan `column-reverse`.

```css
.container {
  display: flex;
  flex-direction: row; /* Default: mengatur elemen sejajar secara horizontal */
}
```

**b. `justify-content`**

Properti ini mengatur cara elemen-elemen di dalam container ditempatkan sepanjang sumbu utama (main axis). Ini mengontrol ruang di antara elemen dan cara mereka didistribusikan.

```css
.container {
  display: flex;
  justify-content: center; /* Mengatur elemen di tengah container */
}
```

**c. `align-items`**

Properti ini mengatur cara elemen-elemen di dalam container ditempatkan sepanjang sumbu lintang (cross axis).

```css
.container {
  display: flex;
  align-items: center; /* Mengatur elemen secara vertikal di tengah container */
}
```

**d. `align-content`**

Properti ini digunakan ketika ada lebih dari satu baris elemen dalam container. Ini mengatur cara baris-baris tersebut didistribusikan secara keseluruhan.

```css
.container {
  display: flex;
  flex-wrap: wrap; /* Perlu diatur agar ada lebih dari satu baris */
  align-content: space-between; /* Mengatur ruang di antara baris */
}
```

### 4. Properti Flex Item

**a. `flex`**

Properti ini menggabungkan `flex-grow`, `flex-shrink`, dan `flex-basis` dalam satu nilai singkat. Ini mengontrol seberapa banyak elemen akan meregang atau menyusut.

```css
.item {
  flex: 1; /* Elemen akan meregang sejauh mungkin */
}
```

**b. `align-self`**

Properti ini mengatur perataan lintang untuk elemen individual di dalam container Flexbox.

```css
.item {
  align-self: flex-end; /* Mengatur elemen tertentu ke bagian bawah */
}
```

**c. `order`**

Properti ini mengatur urutan tampilan elemen di dalam container. Nilai defaultnya adalah 0.

```css
.item {
  order: 2; /* Mengatur elemen tampil setelah elemen dengan order 1 */
}
```

### 5. Penggunaan Flexbox dalam Kasus Sederhana

Misalkan Anda ingin membuat tampilan header dengan logo di kiri dan menu di kanan. Anda bisa menggunakan Flexbox:

```html
<header class="container">
  <div class="logo">Logo</div>
  <nav class="menu">
    <a href="#">Beranda</a>
    <a href="#">Tentang</a>
    <a href="#">Kontak</a>
  </nav>
</header>
```

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  flex: 1;
}

.menu {
  flex: 2;
}
```
