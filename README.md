## **LAPORAN PRAKTIKUM 4 — BOX ELEMENT & LAYOUT WEB SEDERHANA**

---

### **Identitas Mahasiswa**
Nama: Tiara Hayatul Khoir

NIM: 312410474

Kelas: TI.24.A.5

Mata Kuliah: Pemrograman Web

Dosen Pengampu: Agung Nugroho, S.Kom., M.Kom.

---

## **Bagian 1 — Box Element**

### Langkah 1 — Membuat File `lab4_box.html`

**Kode Program:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Box Element</title>
  <style>
    .box {
      background-color: #1d87e4;
      color: white;
      text-align: center;
      width: 200px;
      height: 150px;
      margin: 20px;
      float: left;
      border: 3px solid #0f4b8a;
    }
  </style>
</head>
<body>
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</body>
</html>
```

**Penjelasan:**
Pada langkah ini, dibuat tiga kotak menggunakan elemen `<div>` yang diberi class `box`. Properti CSS `float: left` digunakan agar kotak bisa tersusun sejajar ke samping.

**Hasil Screenshot:**
![Box Element](https://github.com/tir890/Lab4Web/blob/7c9832104dc8ad3b3d7ea3c47cd013d9feca3964/Screenshoot%20Lab4Web/1%20done.png)
---

### Langkah 2 — Menambahkan Padding, Border, dan Shadow

**Kode Program:**

```css
.box {
  background-color: #1d87e4;
  color: white;
  text-align: center;
  width: 200px;
  height: 150px;
  margin: 20px;
  float: left;
  border: 3px solid #0f4b8a;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0,0,0,0.3);
}
```

**Penjelasan:**

* `padding` menambahkan ruang antara isi dan batas kotak.
* `border` memberi garis tepi.
* `box-shadow` menambahkan efek bayangan agar tampilan lebih menarik.

📸 **Hasil Screenshot:**
*(tempelkan hasil kotak dengan efek bayangan di sini)*

---

### Langkah 3 — Menempatkan Kotak di Tengah Halaman

**Kode Program:**

```css
.box {
  background-color: #1d87e4;
  color: white;
  text-align: center;
  width: 200px;
  height: 150px;
  margin: 20px auto;
  border: 3px solid #0f4b8a;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0,0,0,0.3);
}
```

**Penjelasan:**
Dengan menambahkan `margin: auto`, posisi kotak akan berada di tengah halaman secara horizontal.

📸 **Hasil Screenshot:**
*(tempelkan hasil kotak di tengah halaman di sini)*

---

## 💻 **Bagian 2 — Layout Web Sederhana**

### Langkah 1 — Membuat Struktur Dasar HTML

**Kode Program:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Layout Sederhana</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div id="container">
  </div>
</body>
</html>
```

**Penjelasan:**
Membuat kerangka awal halaman web dan menghubungkan file CSS eksternal dengan tag `<link>`.

📸 **Hasil Screenshot:**
*(kosong atau tampilan awal browser)*

---

### Langkah 2 — Menambahkan Header dan Navigasi

**Kode Program:**

```html
<header>
  <h1>Layout Sederhana</h1>
</header>

<nav>
  <a href="home.html" class="active">Home</a>
  <a href="artikel.html">Artikel</a>
  <a href="about.html">About</a>
  <a href="kontak.html">Kontak</a>
</nav>
```

**Penjelasan:**
Bagian ini membuat header dan navigasi agar halaman memiliki identitas serta tautan antar menu.

📸 **Hasil Screenshot:**
*(tampilkan hasil header dan navbar biru)*

---

### Langkah 3 — Menambahkan Hero Section

**Kode Program:**

```html
<section id="hero">
  <h1>Hello World!</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
  <a href="#" class="btn btn-large">Learn more »</a>
</section>
```

**Penjelasan:**
Hero section berfungsi untuk memperkenalkan isi halaman dan menarik perhatian pengguna dengan teks utama dan tombol aksi.

📸 **Hasil Screenshot:**
*(tampilkan area abu-abu dengan teks “Hello World!”)*

---

### Langkah 4 — Menambahkan Wrapper, Main, dan Sidebar

**Kode Program:**

```html
<section id="wrapper">
  <section id="main"></section>
  <aside id="sidebar"></aside>
</section>
```

**Penjelasan:**
Membuat struktur utama halaman yang terdiri dari konten (`main`) dan sidebar (`aside`).

📸 **Hasil Screenshot:**
*(tampilkan dua kolom kosong di browser)*

---

### Langkah 5 — Menambahkan Konten Utama

**Kode Program:**

```html
<section id="main">
  <div class="row">
    <div class="box">
      <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
      <h3>Heading</h3>
      <p>Donec sed odio dui...</p>
      <a href="#" class="btn btn-default">View detail</a>
    </div>
    <!-- dua box lainnya -->
  </div>

  <hr class="divider">
  <article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Lorem ipsum dolor sit amet...</p>
  </article>
</section>
```

**Penjelasan:**
Bagian ini menampilkan tiga kotak sejajar serta artikel fitur dengan gambar dan teks.

📸 **Hasil Screenshot:**
*(tampilkan tiga kotak warna sejajar)*

---

### Langkah 6 — Menambahkan Sidebar

**Kode Program:**

```html
<aside id="sidebar">
  <div class="widget-box">
    <h3 class="title">Widget Header</h3>
    <ul>
      <li><a href="#">Widget Link</a></li>
      <li><a href="#">Widget Link</a></li>
    </ul>
  </div>

  <div class="widget-box">
    <h3 class="title">Widget Text</h3>
    <p>Vestibulum lorem elit...</p>
  </div>
</aside>
```

**Penjelasan:**
Sidebar berisi widget seperti link tambahan atau teks informasi. Letaknya di sebelah kanan halaman.

📸 **Hasil Screenshot:**
*(tampilkan sidebar di sisi kanan halaman)*

---

### Langkah 7 — Menambahkan Footer

**Kode Program:**

```html
<footer>
  <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

**Penjelasan:**
Footer berfungsi sebagai penutup halaman web dan memuat informasi hak cipta.

📸 **Hasil Screenshot:**
*(tampilkan hasil akhir layout lengkap)*

---

## ✅ **Hasil Akhir**

📸 **Tampilan akhir halaman web:**
*(tempelkan screenshot final layout yang udah rapi — sesuai modul dosen)*

---

## **Kesimpulan**

Dalam praktikum ini, mahasiswa telah memahami cara:

* Membuat box element dan mengatur tampilannya menggunakan properti CSS (margin, padding, border, box-shadow).
* Membangun layout web sederhana dengan struktur HTML5 (`header`, `nav`, `section`, `aside`, `footer`).
* Menggunakan kombinasi CSS (float, width, background, dan padding) untuk menghasilkan tampilan dua kolom yang rapi dan responsif.
