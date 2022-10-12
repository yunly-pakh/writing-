## Tugas Writing Week 3
# Day 1
- # JS Intermediate-Array
  # Apa itu Array?
  Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya. Array dapat menyimpan tipe data String, Number, Boolean, dan lainnya.
  # Cara membuat Array
  Terdapat 3 langkah untuk membuat array:
 
       • Mendeklarasikan variabel array 
       • Meng-create array beserta ukurannya.
       • Memberikan sebuah nilai pada setiap element array. 
   Ketiga langkah tersebut bisa dikombinasikan, dalam satu statement, kita dapat mendeklarasikan sekaligus membuat array.
   
   # Mengakses Array
   Array pada javascript dihitung dari index data ke-0.
   Data pertama adalah index ke-0.
   # Const in Array
   
   • Jika menggunakan let, kita dapat mengubah array  dengan array baru dan konten nilai yang ada di dalam array dengan nilai lain
   
   • Const tidak bisa melakukan update data. Namun pada Array kita dapat melakukan update konten nilai di dalam array (mutable).
   
   • Yang tidak bisa adalah mengubah array dengan array yang baru jika menggunakan const
   
   # Array Properties
    Array memiliki 5 properti yang sering digunakan yaitu constructor, length, index, input, dan prototype.
    
   # Array Method
   Array memiliki method atau biasa disebut built-in methods.
   Artinya Javascript sudah memudahkan kita dengan menyediakan function/method umum yang bisa kita gunakan.
   Kita tidak perlu membuat function lagi jika method yang kita butuhkan sudah tersedia.

  # Looping pada Array
  Array memiliki built in methods untuk melakukan looping yaitu .map() dan .forEach()
  
  .forEach() digunakan jika hanya memerlukan looping untuk menampilkan saja atau menyimpan ke database.
  
  .map() digunakan jika akan melakukan operasi pada array seperti yang dapat mengubah nilai array sebelumnya.
  
- # JS Intermediate-Multidimensional Array
   # Multidimensional Array
    Multidimensional Array bisa dianalogikan dengan Ada array didalam array.
       
    # Akses index multidimensional array
    Sama seperti array satu dimensi, multidimensional array juga dapat menggunakan Property dan Method built-in Array.
    
# Day 2
- # JS Intermediate-Object
  # Apa itu Object?
  Object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method)
  
  Properti adalah data lengkap dari sebuah object.
  
  Method adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.
  
  # Membuat sebuah object
  Object dapat diassign kedalam sebuah variabel. didalam object kita dapat menyimpan properti dengan tipe data apapun. 
  
  # Delete Object Property
  Kita dapat menghapus properti dari object menggunakan delete operator. 
  
  # Method
  Jika value yang kita masukkan pada property berupa function. Maka itu disebut method. Nah console adalah global javascript object. log() adalah property yang berupa function dari object console. Sehingga kita memanggil dengan cara console.log().
  
  # Pass by reference
  Kita bisa mengubah data yang ada pada object melalui sebuah function dan memasukkan object sebagai parameter function. Ini biasa disebut passed by reference.
  
  # Looping Object
  Jika kita ingin menampilkan seluruh object properti. Kita bisa menggunakan looping. Jadi tidak perlu mengakses secara manual memanggil setiap propertinya.
  
  # Array of Object
  Object sama seperti Array yang bisa menyimpan banyak data. Kita dapat menggunakan array of object untuk data yang lebih dari satu.
  
  # Day 3
  - # Js Intermediate-Recursive
      # apa itu Recursive?
      Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu.
      
     # Ciri dari rekursif:
      Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar.
      Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.

Recursive kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.
  
# Day 4
  - # JavaScript Intermediate - Asynchronous - Introduction
   # Introduction
   
   Javascript adalah bahasa pemrograman single-thread yang artinya hanya dapat mengeksekusi satu task pada satu waktu atau biasa disebut synchronous.

Pada konsep pemrograman (web development pada case kita) dikenal istilah Asynchronous.

  # Apa itu Asynchronous 
  
   mengizinkan komputer memproses task yang lain sambil menunggu proses yang masih berlangsung.
    
Kita bisa membuat asynchronous secara simulasi artinya tidak murni asynchronous dengan beberapa cara:
- Callback

Callback function adalah function yang kita letakan di dalam argumen/parameter pada function, dan function tersebut akan dieksekusi setelah function pertama menyelesaikan tugasnya.
- Promise

Promise adalah salah satu fitur baru di ES6, biasa digunakan untuk melakukan http request/fetch data dari API.

Dalam pengambilan data, promise memiliki 3 kemungkinan state.

    - Pending(sedang dalam proses)
    - Fulfilled (berhasil)
    - Rejected (gagal)

 - Async-Await
 
 Async - await adalah salah satu fitur baru dari javascript yang digunakan untuk menangani hasil dari sebuah Promise. Sedangkan await berfungsi untuk menunda sebuah kode dijalankan sampai proses asynchronous berhasil.

# HTTP Request fetch()
Fetch adalah native web API untuk melakukan HTTP calls dari external network.
fetch() memiliki parameter utama yaitu URL/endpoint API, dan parameter kedua yaitu options, options ini berisi method, headers dan body. Tergantung keinginan kita.


- # JavaScript Intermediate - Asynchronous - Promise
# Apa itu promise ?

Promise adalah salah fitur terbaru dari ES6. Jika anda sebelumnya sudah pernah menggunakan .then maka anda sudah menggunakan promise.

# Callback vs Promise

Promise umumnya digunakan sebagai alternative callback. Salah satu tantangan di callback adalah callback hell. Disebut neraka ketika ada callback didalam callback didalam callback lagi dan di dalam callback lagi. Problemnya adalah kode sulit dibaca dan penanganan error nya juga menjadi sulit. Disaat seperti ini maka promise menjadi solusi.

Promise bukan untuk menggantikan callback, karena promise akan selalu berjalan asynchronous sedangkan callback bisa digunakan untuk synchronous maupun asynchronous. Benefit utama dari promise adalah membuat code lebih readable dan manajemen error yang lebih baik.

# Membuat dan Menggunakan Promise

- Untuk membuat promise cukup dengan memanggil constructor nya :

![image](https://user-images.githubusercontent.com/113356785/195260464-19d57fe3-6fe5-4a84-ae06-4219847edb11.png)

  output dari code atas adalah Promise {<pending>}  
  
  - Lalu bagaimana untuk mengatur state Fullfilled dan Reject ?
  
  gunakan salah satu listener, resolve() atau reject()
  
  ![image](https://user-images.githubusercontent.com/113356785/195261070-b34c7437-ef69-4f16-b7a4-d61e3e394602.png)
  
  Untuk menggunakan promise diatas gunakan method then dan catch

![image](https://user-images.githubusercontent.com/113356785/195261294-48763e55-d234-4fff-b3ce-b5a54dbb6692.png)

Output dari code diatas ada 2 kemungkinan,

Jika comment pada resolve( ) di hapus maka hasilnya “berhasil” dan Jika comment pada reject( ) di hapus maka hasilnya “Janji di batalkan”

# Request dengan Fetch

fetch adalah API yang di perkenalkan sejak ES6, untuk melakukan request ajax. Berikut boilerplate untuk penggunaan fetch.

![image](https://user-images.githubusercontent.com/113356785/195261697-8e87d595-e5e6-42fd-9f67-20f6f56db877.png)


kita coba request ke API public

![image](https://user-images.githubusercontent.com/113356785/195261955-422c4694-3a31-494b-94f3-6d8ff4129d34.png)


Ouput dari code diatas json data user.

![image](https://user-images.githubusercontent.com/113356785/195262339-e11acb3e-2567-4136-85b9-31d3c402df72.png)
 
 
 # kenapa method .then di panggil 2 kali ?
 - Response fetch pada #1 hasilnya adalah object Response, untuk lebih detailnya adan bisa lihat disini. Untuk mendapat response dalam bentuk json() maka digunakan method Body.json()
- Hasil dari method Body.json() dibaca pada #2. Selain json kita juga menerima respon dalam format plain text menggunakan method Body.text()

# Day 5
- # Js Intermediate-Web Storage
# Apa itu responsive web design?

Responsive Web Design (RWD) adalah bertujuan membuat desain website kita dapat diakses dalam device apapun.

# Setting up chrome Dev tools

Pada browser chrome biasa disebut dengan Chrome Dev Tools. Kita akan belajar cara menggunakannya sebagai tools dari RWD.

- Akses chrome Dev tools

![image](https://user-images.githubusercontent.com/113356785/195265177-210daddd-5d09-43ec-bb51-874192381ef9.png)

- Add Viewport in HTML

![image](https://user-images.githubusercontent.com/113356785/195265680-3ad1287b-8c16-4410-88a6-1f7851b7da43.png)

- Use max-width element

![image](https://user-images.githubusercontent.com/113356785/195265999-a22b7b07-c135-4738-89ac-a02d22cc736f.png)

# Media Query

RWD sangat menyenangkan dan mudah jika kita menggunakan media query

# Jenis Media query

- media query untuk responsive web design umumnya hanya mengunakan 2 jenis media query kedanya yaitu min-width dan max-width

# ada 2 pattern dalam menggunakan media query

- membuat file CSS berbeda untunk masing-masing device 
- kita menggabungkan 1 file CSS untuk setting styling berbagai device

# Breakpoint 

perubahan yang terjadi pada tampilan saat berganti device atau ukuran width 
















  








