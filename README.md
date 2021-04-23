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
Selanjutnya buka rowser dan refresh kembali.

![4](https://user-images.githubusercontent.com/81820421/115936053-865e4a80-a4be-11eb-9ac2-692b7a166957.JPG)

