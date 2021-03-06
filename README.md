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
    Kemudian buka browser dan lihat hasilnya.
   ![6](https://user-images.githubusercontent.com/81820421/115937529-6466c700-a4c2-11eb-9457-4503f5be8fe0.JPG)
   # Dilanjut Kemudian tambahkan kode CSS untuk membuat layoutnya.
   ~~~
   /* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@importurl('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
 margin: 0;
 padding: 0;
}
body {
 line-height:1;
 font-size:100%;
 font-family:'Open Sans', sans-serif;
 color:#5a5a5a;
}
#container {
 width: 980px;
 margin: 0 auto;
 box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
 padding: 20px;
}
header h1 {
 margin: 20px 10px;
 color: #b5b5b5;
~~~
![7](https://user-images.githubusercontent.com/81820421/115943606-11e5d480-a4db-11eb-8ddb-d002c84e6288.JPG)
Dan lihat hasilnya setelah di refresh .
# Membuat Navigasi
Kemudian selanjutnya mengatur navigasi
Masukan sourcode ini ke style.css
~~~
/* navigasi */
nav {
 display: block;
 background-color: #1f5faa;
}
nav a {
 padding: 15px 30px;
 display: inline-block;
 color: #ffffff;
 font-size: 14px;
 text-decoration: none;
 font-weight: bold;
}
nav a.active,
nav a:hover {
 background-color: #2b83ea;}
 ~~~
 ![8](https://user-images.githubusercontent.com/81820421/115943961-304ccf80-a4dd-11eb-97e1-193dcd902b0f.JPG)
 
# Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML 
~~~
<section id="hero">
 <h1>Hello World!</h1>
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
 <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
~~~ 
Dan ini kode untuk css nya.
~~~
/* Hero Panel */
#hero {
 background-color: #e4e4e5;
 padding: 50px 20px;
 margin-bottom: 20px;
}
#hero h1 {
 margin-bottom: 20px;
 font-size: 35px;
}
#hero p {
 margin-bottom: 20px;
 font-size: 18px;
 line-height: 25px;}
 ~~~
 Dan lihat hasilnya setelah di refresh. 
 ![9](https://user-images.githubusercontent.com/81820421/115944355-7b67e200-a4df-11eb-9a19-93b35bf41fad.JPG)
# Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
~~~
/* main content */
#wrapper {
 margin: 0;
 }
 #main {
 float: left;
 width: 640px;
 padding: 20px;
}
/* sidebar area */
#sidebar {
 float: left;
 width: 260px;
 padding: 20px;
}
~~~
# Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
masukan code ini ke css 
~~~
/* main content */
#wrapper {
 margin: 0;
 }
 #main {
 float: left;
 width: 640px;
 padding: 20px;
}
/* sidebar area */
#sidebar {
 float: left;
 width: 260px;
 padding: 20px;
 }
 ~~~
 # Membuat Sidebar Widget
Kemudian selanjutnya menambahkan element lain dalam sidebar. 
Masukan code ini ke html 
~~~
<aside id="sidebar">
 <div class="widget-box">
 <h3 class="title">Widget Header</h3>
 <ul>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 <li><a href="#">Widget Link</a></li>
 </ul>
 </div>
 <div class="widget-box">
 <h3 class="title">Widget Text</h3>
 <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
pharetra est nunc, nec pretium nunc pretium ac.</p>
 </div>
</aside>
~~~
Tambahkan code css nya.
~~~
/* widget */
.widget-box {
 border:1px solid #eee;
 margin-bottom:20px;
}
.widget-box .title {
 padding:10px 16px;
 background-color:#428bca;
 color:#fff;
}
.widget-box ul {
 list-style-type:none;
}
.widget-box li {
 border-bottom:1px solid #eee;
 }
.widget-box li a {
 padding:10px 16px;
 color:#333;
 display:block;
 text-decoration:none;
}
.widget-box li:hover a {
 background-color:#eee;
}
.widget-box p {
 padding:15px;
 line-height:25px;}
 ~~~
 ![10](https://user-images.githubusercontent.com/81820421/115944845-79535280-a4e2-11eb-9442-cfa40b7f5c84.JPG)
 # Mengatur Footer
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
~~~
/* footer */
footer {
 clear:both;
 background-color:#1d1d1d;
 padding:20px;
 color:#eee;
 }
 ~~~
 ![11](https://user-images.githubusercontent.com/81820421/115944891-e4048e00-a4e2-11eb-9628-a198171338bc.JPG)
 # Menambahkan Elemen lainnya pada Main Content
 Masukan sourcode ini ke html 
 ~~~
 <section id="main">
 <div class="row">
 <div class="box">
 <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
 <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
 <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
 <h3>Heading</h3>
 <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 </div>
</section>
~~~
# Kemudian tambahkan CSS.
~~~
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
    text-align:center;
   }
   .box h3 {
    margin: 15px 0;
   }
   .box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
   }
   box img {
    border: 0;
    vertical-align: middle;
   }
   .image-circle {
    border-radius: 50%;
   }
   .row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
   }
   .row:after, .row:before,
   .entry:after, .entry:before {
    content:'';
    display:table;
   }
   .row:after,
   .entry:after {
    clear:both;
   
}
~~~
![12](https://user-images.githubusercontent.com/81820421/115945049-e0bdd200-a4e3-11eb-9309-30e40707e7e5.JPG)
Dan lihat hasilnya setelah direfresh .
# Menambahkan Content Artikel
Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
~~~
<hr class="divider" />
<article class="entry">
 <h2>First featurette heading.</h2>
 <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
 <h2>First featurette heading.</h2>
 <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
~~~
Kemudian tambahkan CSS.
~~~
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
   }
   /* entry */
   .entry {
    margin: 15px 0;
   }
   .entry h2 {
    margin-bottom: 20px;
}
.entry p {
 line-height: 25px;
}
.entry img {
 float: left;
 border-radius: 5px;
 margin-right: 15px;
}
.entry .right-img {
 float: right;
}
~~~
Dan lihat ini hasil nya stelah web di refresh .
![13](https://user-images.githubusercontent.com/81820421/115945218-d5b77180-a4e4-11eb-83c0-e7ea95b9d93e.JPG)

## Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll

# membuat layout untuk portofolio endrik photograpy 
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Endrik Photography </title>
 <link rel="stylesheet" href="style.css">
</head>
<header>
    <h1>Endrik Photography</h1>
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
   <section id="hero">
    <h1>Hello Calon Manten!</h1>
    <p>Kita adalah vendor Photography terbaik di Indonesia. Abadikan moment pernikahan kalian dengan kita 
        Moto kita adalah make classy your story .</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
   </section>
   <aside id="sidebar">
    <div class="widget-box">
    <h3 class="title">Widget Header</h3>
    <ul>
    <li><a href="#">Wedding Photo</a></li>
    <li><a href="#">Prewedding Photo</a></li>
    <li><a href="#">Maternity Photo</a></li>
    <li><a href="#">Casual Photo</a></li>
    <li><a href="#">Personal Photography</a></li>
    </ul>
   
   <footer>
    <p>&copy; 2021 - Wedding Photography Indonesia</p>
   </footer>
<body>
 <div id="container">

 </div>
</body>
</html>
~~~
![14](https://user-images.githubusercontent.com/81820421/115945891-fdf49f80-a4e7-11eb-9062-60fa2599f56b.JPG)



2. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Endrik Photography </title>
 <link rel="stylesheet" href="style.css">
</head>
<header>
    <h1>Endrik Photography</h1>
   </header>
   <nav>
    <a href="home.html" class="active">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
   </nav>
   <form>
       <fieldset>
           <legend>Kontak</legend>
           <p>
            <h1><br>Endrik Photography</p><h/1></h>

               <a href="https://mail.google.com/mail/u/0/#inbox"> Endrikbinsuwarih@gmail.com</a>
            </p>

              Telephone : 089654886651
              </fieldset>
   </form>
</body>
</html
~~~

![16](https://user-images.githubusercontent.com/81820421/115946240-149bf600-a4ea-11eb-99c0-f8578a861c87.JPG)






 
 




   
   

