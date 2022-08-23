# BOOTSTRAP RWD
## RWD
### Apa itu RWD?
RWD adalah singkatan dari **Responsive Web Design**. RWD bertujuan untuk membuat design website kita dapat diakses dalam device apapun contohnya laptop/pc, Handphone dan Tablet. Seorang developer website wajib menggunakan tools bawaan dari setiap browser yang memudahkan proses development website , pada browser chorme biasa disebut dengan **Chrome Dev Tools**. Jika tidak menggunakan responsive pada website maka panjang image menjadi **overflow** karena mengikuti **width** real bawaan dari file image.
### **Menggunakan **Max-Width** element.**
Menaruh **style= "max-width"** pada tag img  yang akan ditampilkan dan dapat menaruh ukuran berapa saja pada max-width tersebut. contoh *style="max-width: 100%*. Dengan menggunakan max-width maka tidak ada **overflow width** pada image dan tampilan **mobile device/Smartphone** menyesuaikan dengan baik.

### **Media query untuk responsive web design umumnya hanya menggunakan 2 jenis media query.**
1. MIN-WIDTH

@media screen and (min-width: your pixel) { /* didalam element html dan css }.

2. MAX-WIDTH

@media screen and (max-width: your pixel) { /* didalam element html dan css }.

### Ada dua cara/pattern dalam menggunakan media query


1. membuat file css berbeda untuk masing" device.
 ada dua file css yaitu:
* main.css
body {
    background-color: white;
}
* main.mobile.css.
body {
    background-color: aquamarine;
}. 

2. kita menggabungkan 1 file css untuk setting styling berbagai device dengan menaruh 

        @media screen and (max-width: 500px){
        body {
        background-color: aquamarine;
         }
        }
untuk tampilan pada **Mobile Device** maka body akan berwarna *aquamarine*.

### Breakpoint
Breakpoint yaitu perubahan yang terjadi pada tampilan saat berganti device atau ukuran width.
Ada tiga tampilan yg berbeda untuk 3 jenis device.
### Complex Breakpoint Media Query
Jika ingin tampilan yg diterapkan pada range ukuran device tertentu, kita bisa membuat menjadi range media query.
menggunakan range media query min dan max.

       body {
          background-color: white;
        }
       @media screen and (min-width: 500px) and (max-width: 700px) {
        body{
            background-color: aquamarine;
        }
       }

Jika kita menggunakan media query dengan ukuran min-width 700 maka tampilan website akan lebih besar dibandingkan dengan ukuran min-width 500 jauh lebih kecil.

## Bootstrap Grid

* HTML

       <div class="container text-center">
           <div class="row">
             <div class="col">
              Column
           </div>
             <div class="col">
              Column
           </div>
              <div class="col">
              Column
            </div>
            </div>
           </div>

Code diatas akan menghasilkan 3 kolom dalam satu baris dengan lebar dan panjang yang sama. Kolom tersebut dipusatkan di halaman dengan induknya .container.

### Sistem grid Bootstrap 
Sistem grid Bootstrap dapat beradaptasi di enam **breakpoint default**, dan setiap breakpoint yang Anda sesuaikan. Enam tingkatan grid default adalah sebagai berikut:

* Ekstra kecil **(xs)**
* Kecil **(sm)**
* Sedang **(md)**
* Besar **(lg)**
* Ekstra besar **(xl)**
* Ekstra ekstra besar **(xxl)**

# React Js

## React Js adalah?
React JS yaitu **Framework view library Javascript** untuk membuat tampilan *(user interface)* pada website.
React JS dibuat oleh Tim Engineer Facebook. Facebook menggunakan React JS pada sisi front-end. dan React JS masih unggul diantara **Framework javascript** lainnya.

## Mengapa menggunakan React js?
* React js bisa membuat aplikasi menjadi lebih cepat walaupun harus menghandle berbagai data.
* kita dapat menerapkan konsep modular javascript pada react js, contohnya react js membagi 1 tampilan pada website menjadi komponen-komponen kecil seperti Navbar, Form dan Title.
* Dapat digunakan pada aplikasi berskala kecil hingga besar dan kompleks.
* Banyak perusahaan menggunakan React js.

**Vanilla JS** adalah kita menggunakan native javascript (default).

## Tag HTML pada file javascript
karena itu merupakan **JSX**, **JSX**
adalah **syntax extension for 
javascript**, JSX dikembangkan untuk digunakan pada React JS, namun JSX perlu dicompile untuk menjadi Javascript, dengan JSX kita dapat menggunakan HTML didalam *file extension Javascript (.js)*

## JSX Rules
Setiap JSX hanya bisa memiliki 1 parent element, jika **parent element** lebih dari satu maka terjadi ***ERROR***. dan gunakan tag element < div> / fragment <> sebagai parent dari element. Pada JSX attribute class di tag element HtMl harus menggunakan **className**. Kita bisa menggunakan syntax Javascript di dalam element HTML dengan ***curly braces***

## The Virtual Dom
Dengan DOM kita dapat berinteraksi seperti mengupdate data di *web page*.

Virtual DOM adalah ***duplikasi*** dari real DOM yang sebenarnya.

# React JS Component
## Apa itu Component?
Component dibuat jika component tersebut bersifat **reusable code**. pada skala project maka kita harus membuat componet jika component tersebut akan dibutuhkan pada section atau page lain.

## Membuat Component
Ada 2 cara membuat Component:
1. Functional
2. Class

## State dan Props
Hal yang berhubungan dengan **Stateless & Stateful Component**. **stateles** yang berarti tidak memiliki state dia hanya memiliki props, sedangkan **stateful** berarti memiliki state dan bisa mengirim state tersebut ke component. Jadi **state** adalah data Local sedangkan **Props** digunakan agar component memiliki data yang dinamis yang dikirim dari component lain.