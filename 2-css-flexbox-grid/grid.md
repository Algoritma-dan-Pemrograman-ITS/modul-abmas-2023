**Pembelajaran Grid CSS**

Grid CSS adalah teknik tata letak yang kuat yang memungkinkan Anda mengatur tampilan elemen-elemen dalam grid dua dimensi (baris dan kolom). Dalam tutorial ini, kita akan menjelaskan secara mendalam konsep dasar Grid CSS dan cara menggunakannya.

### Daftar Isi

1. Pengenalan ke Grid CSS
2. Display dan Container Grid
3. Properti Utama Grid Container
   - `grid-template-columns` dan `grid-template-rows`
   - `grid-gap`
   - `grid-template-areas`
4. Properti Grid Item
   - `grid-column` dan `grid-row`
   - `grid-area`
5. Penggunaan Grid dalam Kasus Sederhana
6. Responsif dengan Grid
7. Tips dan Trik

### 1. Pengenalan ke Grid CSS

Grid CSS adalah teknik tata letak yang memungkinkan Anda untuk mengatur elemen-elemen dalam baris dan kolom, mirip dengan tata letak tabel. Namun, Grid lebih fleksibel dan kuat, memungkinkan Anda mengontrol posisi, ukuran, dan urutan elemen secara lebih detail.

### 2. Display dan Container Grid

Pertama, Anda perlu mengubah elemen induk menjadi wadah (container) untuk elemen-elemen yang akan diatur dalam grid. Anda melakukannya dengan mengubah properti `display` dari elemen tersebut.

```css
.container {
  display: grid; /* Mengubah elemen menjadi container Grid */
}
```

### 3. Properti Utama Grid Container

**a. `grid-template-columns` dan `grid-template-rows`**

Properti ini digunakan untuk menentukan jumlah dan lebar (atau tinggi) kolom dan baris dalam grid.

```css
.container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr; /* Tiga kolom dengan lebar relatif */
  grid-template-rows: 100px auto; /* Dua baris dengan tinggi tetap dan sisa ruang */
}
```

**b. `grid-gap`**

Properti ini mengatur jarak antara kolom dan baris dalam grid.

```css
.container {
  display: grid;
  grid-gap: 10px; /* Jarak antara kolom dan baris */
}
```

**c. `grid-template-areas`**

Properti ini memungkinkan Anda memberi nama area-area dalam grid untuk kemudian ditempatkan oleh elemen-elemen.

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
}
```

### 4. Properti Grid Item

**a. `grid-column` dan `grid-row`**

Properti ini digunakan pada elemen individual untuk menentukan di mana elemen tersebut akan ditempatkan dalam grid.

```css
.item {
  grid-column: 1 / 3; /* Elemen menempati kolom 1 hingga 3 */
  grid-row: 2; /* Elemen menempati baris 2 */
}
```

**b. `grid-area`**

Properti ini menggabungkan `grid-row` dan `grid-column` dalam satu nilai untuk menentukan area elemen dalam grid.

```css
.item {
  grid-area: 2 / 1 / 3 / 3; /* Elemen menempati area dari baris 2 kolom 1 hingga baris 3 kolom 3 */
}
```

### 5. Penggunaan Grid dalam Kasus Sederhana

Misalkan Anda ingin membuat tampilan dengan header, sidebar, dan konten utama:

```html
<div class="container">
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="main">Main Content</div>
</div>
```

```css
.container {
  display: grid;
  grid-template-columns: 1fr 200px;
  grid-template-rows: auto;
  grid-gap: 10px;
}

.header {
  grid-column: 1 / 3;
}

.sidebar {
  grid-column: 2;
}

.main {
  grid-column: 1;
} 
