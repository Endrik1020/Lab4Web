# Lab4Web
# Pemograman Web
~~~
Nama   = Endrik
NIM    = 311910088
Kelas  = TI.19.C.1
Universitas Pelita Bangsa
~~~
## 1. MEMBUAT BOX ELEMENT 
Buka aplikasi Visual Code
Masukann sourcode ini pada new file html :
~~~
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Box Element</title>
</head>
<body>
 <header>
 <h1>Box Element</h1>
 </header>
</body>
</html>
~~~
![1](https://user-images.githubusercontent.com/81820421/115934842-2ff00c80-a4bc-11eb-94cb-00832fa7e1f1.JPG)

#Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut
~~~
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div>
</section>
~~~
![2](https://user-images.githubusercontent.com/81820421/115935207-dfc57a00-a4bc-11eb-9dfd-3e06198b243c.JPG)
## 2. CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut:
~~~
<style>
 div {
 float:left;
 padding: 10px;
 }
 .div1 {
 background: red;
 }
 .div2 {
 background: yellow;
 }
 .div3 {
 background: green;
 }
</style>
~~~
![3](https://user-images.githubusercontent.com/81820421/115935470-6f6b2880-a4bd-11eb-9a29-6e259add71ab.JPG)
Kemudian buka browser untuk melihat hasilnya.
## 3. Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.
Tambahkan element div lainnya seteleah div3 seperti berikut
~~~
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div>
 <div class="div4">Div 4</div>
</section>
~~~
Kemudian atur property clear pada CSS, seperti berikut.
~~~
div4 {
 background-color: blue;
 clear: left;
 float: none;
}
~~~
Selanjutnya buka browser dan refresh kembali.

![4](https://user-images.githubusercontent.com/81820421/115936053-865e4a80-a4be-11eb-9ac2-692b7a166957.JPG)
Lakukan eksperimen terhadap penggunaan property clear dengan nilai lainnya (left, both, right),
dan amati perubahannya.
coba ubah posisi menjadi right .
~~~
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
   </section>
   <style>
    div {
    float:right;
    padding: 10px;
    }
    .div1 {
    background: red;
    }
    .div2 {
    background: yellow;
    }
    .div3 {
    background: green;
    }
    .div4 {
 background-color: blue;
 clear: right;
 float: both;
}
~~~
![5](https://user-images.githubusercontent.com/81820421/115936659-0fc24c80-a4c0-11eb-88a3-125be97be59a.JPG)

Coba lakukan refresh pada Web dan lihat hasilnya.

## 4.Membuat Layout Sederhana
Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama
home.html, dan file css dengan nama style.css.
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
   </head>
   <body>
    <div id="container">
   
    </div>
   </body>
   </html>
   ~~~
   Kemudian tulis kode berikut.
   ~~~
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
   </head>
   <body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
           </header>
           <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
           </nav>
           <section id="hero"></section>
           <section id="wrapper">
            <section id="main"></section>
            <aside id="sidebar"></aside>
           </section>
           <footer>
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
           </footer>
   
    </div>
   </body>
   </html>
   ~~~
  
   ![6](https://user-images.githubusercontent.com/81820421/115937529-6466c700-a4c2-11eb-9457-4503f5be8fe0.JPG)
   Kemudian buka browser dan lihat hasilnya.

