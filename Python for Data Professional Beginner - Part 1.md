### DQLab x Komdigi
## Python for Data Professional Beginner - Part 1
# _Guide to Learn Python with AI at DQLab_

Apa dan Kenapa Python – Part 1?
Python adalah bahasa pemrograman yang ditujukan untuk general-purpose programming dan termasuk dalam kategori high-level programming language.Sebagai general-purpose programming language, Python digunakan untuk berbagai macam permasalahan seperti: pengembangan aplikasi web ataupun mobile, data science, dll.Python masuk ke dalam kategori high-level programming language dikarenakan bahasa pemrograman Python yang mudah untuk dibaca dan dituliskan oleh manusia.Bahasa  pemrograman  Python  diciptakan  oleh Guido van Rossum dan pertama kali diperkenalkan pada tahun 1991 sebagai sebuah proyek open-source.Sifat open-source dari Python mengartikan bahwa setiap orang dapat mengembangkan program komputer dengan menggunakan bahasa pemrograman Python baik untuk tujuan komersil/non-komersil.

Bahasa pemrograman Python bersifat dynamically typed (Python akan secara otomatis mengubah masukan dari pengguna) dan mendukung berbagai paradigma pemrograman baik pemrograman secara prosedural, berbasis objek (Object-Oriented), ataupun fungsional.Selain alasan di atas terdapat beberapa alasan lain untuk menggunakan bahasa pemrograman Python:
1. Python dikembangkan untuk bersifat extendible yang mengartikan bahwa Python dapat dikembangkan untuk berbagai macam tugas baik untuk pembuatan aplikasi web ataupun desktop, proses analisis data, dll.
2. Python memiliki komunitas yang besar yang secara aktif berkontribusi untuk menyediakan berbagai macam fungsionalitas (third-party libraries). Third-party libraries yang tersedia dalam bahasa pemrograman Python memungkinkan para pengembang untuk dapat fokus menyelesaikan permasalahan yang ada. Per Januari 2020, terdapat 214,922 modul third-party yang dapat kita gunakan secara cuma-cuma.
3. Python terintegrasi dengan baik dengan berbagai macam bahasa pemrograman dan layanan enterprise. Untuk bagian-bagian yang melibatkan sumber daya komputasi yang besar, pengembang dapat menggunakan fungsionalitas dalam bahasa pemrograman lainnya yang bersifat low-level yang telah dikemas ke dalam fungsionalitas Python.

## Program pertama: "Hello World"
Setelah memahami teori-teori fundamental terkait dengan "Apa dan Mengapa Python?", aku diminta membuat sebuah program sederhana dengan Python.Fungsi Python yang akan pertama kali aku pelajari adalah fungsi print(). Dengan fungsi print(), aku dapat menampilkan atau mencetak teks ke layar pengguna.
### Tugas Praktek
Aku diberikan tugas oleh Senja untuk menampilkan pesan "Hello World!" pada layar dengan fungsi print().
```sh
print ('Hello World!;')
```
## Lebih Jauh dengan Print
Keren! Aku baru tahu kalau Python memiliki fungsi print() yang berguna untuk menampilkan pesan ke layar pengguna.

### Tugas Praktek
Sekarang aku diberikan tugas dari Senja untuk menampilkan dua kalimat, yaitu "Halo Dunia" dan "Riset Bahasa Python" menggunakan fungsi print(). Catatan: Untuk membantu aku, di dalam bagian code editor sudah diberikan template code jawaban dimana aku harus mengganti ___ dengan teks yang diminta oleh soal dari tugas praktek di atas. Klik tombol Run untuk menjalankan code tersebut. Dan jika sudah berjalan lancar, tekan Submit untuk mengirim jawaban ke dalam sistem.
```sh
print("Halo Dunia")
print("Riset Bahasa Python")
```

## Struktur Program Python - Part 1
Setelah berhasil membuat program sederhana menggunakan Python, aku diminta Senja untuk belajar struktur dari sebuah program Python.

Dari situ aku paham sebuah program Python pada umumnya terdiri dari:
1. Statements: Instruksi yang diberikan secara baris per baris untuk dijalankan oleh
2. Variables: Lokasi penyimpanan yang dapat digunakan untuk menampung sebuah data atau informasi. Contoh: aku mempunyai variabel yang bernama bilangan1, bilangan2, dan kalimat1
3. Literals: Simbol-simbol yang dapat kita gunakan untuk mengisi suatu variabel. Pada kode yang telah dicontohkan di atas, angka 5 dan 10 serta 'Belajar Bahasa Python' disebut sebagai literal.
4. Operators: Simbol-simbol yang dapat digunakan untuk mengubah nilai dari satu variabel dengan melibatkan satu atau lebih variabel dan literal. Contoh: Tanda + merupakan salah satu contoh operator. Dengan menggunakan tanda +, aku berhasil menambahkan isi dari bilangan1 dan bilangan2!

Adapun operator yang lain selain operator + adalah sebagai berikut.
1. Operator - yang berfungsi sebagai operator pengurangan,
2. Operator * yang berfungsi sebagai operator perkalian, dan
3. Operator ** untuk pemangkatan

 ### Tugas :
Aku diminta untuk mencoba mempraktekkan tutorial yang diajarkan untuk memahami struktur bahasa pemrograman Python.
```sh
# Statement
print("Belajar Python Menyenangkan") 
print("Halo Dunia")
print("Hello World!")
# Variables & Literals
bilangan1 = 5
bilangan2 = 10
kalimat1 = "Belajar Bahasa Python"
# Operators
print(bilangan1 + bilangan2)
```

### Tugas Praktek
Tantangan belum berakhir. Aku diminta Senja untuk membuat program pengurangan sederhana dengan Python.
Tugas:
Deklarasi variable bilangan1 dengan 20, dan bilangan2 dengan 10 dan tampilkan hasil pengurangan bilangan1 & bilangan 2.
```sh
bilangan1 = 20
bilangan2 = 10
print(bilangan1 - bilangan2)
```
## Tugas Praktek
“Saya lihat kamu cepat belajar. Gimana kalau kamu coba buat kalkulator sederhana untuk potongan harga dan pajak, Aksara?” komentar Senja padaku.

Tugas:
Aku diminta menghitung harga_setelah_potongan dan harga_final. harga_final diperoleh dengan mengalikan harga_setelah_potongan dengan angka 1.1 karena PPN sebesar 10% (100% + 10% = 110% atau 1.1)
Aku menggunakan variabel harga_asli dengan nilai 20000 dan variabel potongan dengan nilai 2000.
```sh
harga_asli = 20000 
potongan = 2000
harga_setelah_potongan = harga_asli - potongan
harga_final = harga_setelah_potongan * 1.1

print(harga_final)
```

Struktur Program Python - Part 2
Setelah mengerjakan tugas yang diberikan Senja, aku kembali lanjut belajar. Berikut adalah hal-hal baru yang aku pelajari mengenai Python:

1. Reserved Words: Kumpulan kata-kata yang memiliki makna khusus dalam bahasa pemrograman Python. Kata False, return, dan for merupakan contoh dari reserved words. Catatan: Ternyata, aku tidak dapat mendeklarasikan variabel dengan menggunakan sebuah reserved word!
2. Whitespace: Pada bahasa Python, spasi dan tab memiliki makna khusus untuk menandai serangkaian blok dalam kode Python. Hal ini akan dijelaskan secara lebih lanjut pada bagian struktur pemilihan dan struktur pengulangan pada bahasa Python.
3. Comments: Comments merupakan sekumpulan teks yang dituliskan di dalam sebuah program yang tidak akan mempengaruhi hasil dari sebuah program. Walaupun tidak mempengaruhi hasil program, comments merupakan salah satu komponen yang penting dalam pengembangan program. Hal tersebut dikarenakan comments dapat diselipkan di antara sekumpulan statements yang telah dituliskan, untuk berkomunikasi dengan rekan programmer lainnya dalam satu tim. 
Terdapat dua jenis comments di dalam Python, yaitu:
a. single line comment (comments dalam satu baris)
```sh
## Variabel xxxxxx
```
b.  multi line comment (comments dalam beberapa baris)
```sh
'''
Variabel xxxxxxx 
xxxxxx
xxxxx
'''
```

## Python Variables & Data Types

### Aturan Penamaan Python Variables
Penamaan suatu variabel pada python dapat dikatakan valid selama memenuhi aturan-aturan berikut:
1. Nama dari sebuah variabel harus dimulai dengan huruf (a-z, A-Z) atau karakter garis bawah underscore (_) dan tidak dapat dimulai dengan angka (0-9).
2. Variabel hanya boleh mengandung karakter alfabet, bilangan dan underscore (a-z, A-Z, 0-9, _)
3. Variabel bersifat case-sensitive yang mengartikan bahwa variabel TINGGI, tinggi, dan Tinggi merujuk pada tiga variabel berbeda.

Selain dapat mendeklarasikan nilai dari suatu variabel secara baris per baris, aku juga dapat mendeklarasikan beberapa variabel dalam satu baris dengan menggunakan ekspresi seperti:
```sh
Var1, Var2 = x, y
provinsi = "Jambi", kabupaten "Bungo"
```
### Tipe Data Dasar: Null, Boolean, Numeric dan Text
1. Null Type: Tipe data null dalam Python digunakan untuk menyimpan nilai kosong atau tidak ada yang dinyatakan dengan None.
2. Boolean Type: Tipe data boolean atau bool digunakan untuk menyimpan nilai kebenaran (True, False) dari suatu ekspresi logika.
3. Numeric Type: Tipe data yang digunakan untuk menyimpan data berupa angka. Terdapat dua macam tipe data numeric, yaitu int untuk menyimpan bilangan bulat (e.g.: 0, 1, 2, 404, -500, -1000) dan float untuk menyimpan bilangan riil (e.g.: 0.5, 1.01, 2.05, 4.04)
4. Text Type: Pada Python, tipe data string (str) digunakan untuk menyimpan data teks. Tipe data string dimulai dengan tanda kutip (baik kutip satu/ dua) dan diakhir dengan tanda kutip. Contoh: "Teks", "Contoh teks menggunakan Python", dan 'Teks pada Python'.

### Sequence Type – Part 1
Tipe data ini digunakan untuk menampung sekumpulan data secara terorganisir.
Bentuk dari tipe data sequence ini adalah List dan Tuple.
Pada part 1 ini, aku akan mempelajari tipe data list terlebih dahulu.
Tipe data list diawali dengan tanda kurung siku buka ( [ ), memisahkan setiap elemen di dalamnya dengan tanda koma ( , ) dan ditutup dengan kurung siku tutup ( ] ).

### Tugas:
Aku diberikan tugas untuk menerapkan variasi tipe data list dengan mengikuti petunjuk yang diberikan Senja. Berikut petunjuknya:
Petunjuk 1: Input data 1, 'dua', 3, 4.0, 5 ke dalam contoh_list
Petunjuk 2: Ambil Elemen pertama dari contoh_list untuk menampilkan output 1 menggunakan print statement
Petunjuk 3: Ambil Elemen ke empat dari contoh_list untuk menampilkan output 4.0 menggunakan print statement
Petunjuk 4: Input data 1, 'dua', 3, 4.0, 5 ke dalam contoh_list
Petunjuk 5: Ubah Elemen keempat dalam contoh_list menjadi 'empat'
Petunjuk 6: Tampilkan output elemen keempat yang telah diubah tersebut menggunakan print statement


```sh
contoh_list = [1, 'dua', 3, 4.0, 5]
print(contoh_list[0])
print(contoh_list[3])
contoh_list = [1, 'dua', 3, 4.0, 5]
contoh_list[3] = 'empat'
print(contoh_list[3])
```

### Sequence Type – Part 2
Setelah mempelajari tipe data list, aku mempelajari tipe data tuple. Tipe data tuple juga berfungsi untuk menampung sekumpulan data. Tipe data ini diawali dengan tanda kurung buka ( ( ), memisahkan setiap elemen di dalamnya dengan tanda koma ( , ) dan ditutup dengan tanda kurung tutup ( ) ).

### Tugas:
Sekarang aku diberikan tugas untuk menerapkan variasi tipe data tuple dengan mengikuti petunjuk yang diberikan Senja:
Petunjuk 1: Input data Januari sampai dengan April ke dalam contoh_tuple
Petunjuk 2: Ambil Elemen pertama dari contoh_tuple untuk menampilkan output 1 menggunakan print statement
Petunjuk 3: Input kembali data Januari sampai dengan April ke dalam contoh_tuple
Petunjuk 4: Ubah Elemen pertama dalam contoh_tuple menjadi 'Desember'
Ketika dijlankan ini akan menghasilkan error yaitu TypeError, silakan kamu submit dengan adanya error dari output pada Petunjuk 4 tersebut. 

```sh
contoh_tuple = ('Januari', 'Februari', 'Maret', 'April')
print(contoh_tuple[0])
contoh_tuple = ('Januari', 'Februari', 'Maret', 'April')
contoh_tuple[0] = 'Desember'
```

### Set Type
Serupa dengan tipe data sequence, tipe data set digunakan untuk menampung sekumpulan data dengan tipe lainnya. Terdapat dua jenis dari tipe data set yaitu, set dan frozenset.
Tipe data set diawali dengan tanda kurung buka kurawal ( { ), memisahkan setiap elemen di dalamnya dengan tanda koma ( , ) dan ditutup dengan tanda kurung tutup ( } ). Namun berbeda dengan tipe data sequence, seperti list, tipe data objek tidak mengizinkan adanya elemen dengan nilai yang sama dan tidak mempedulikan urutan dari elemen.
### Tugas:
Sekarang aku diberikan tugas untuk menerapkan variasi set dan frozenset oleh Senja:
Tugas 1:Input data Dewi, Budi, Cici, Linda, Cici kedalam tipe data list dan tampilkan hasilnya
Tugas 2: Input data Dewi, Budi, Cici, Linda, Cici kedalam tipe data set dan tampilkan hasilnya
Tugas 3: Input data Dewi, Budi, Cici, Linda, Cici kedalam tipe data frozenset dan tampilkan hasilnya

```sh
contoh_list = ['Dewi', 'Budi', 'Cici', 'Linda', 'Cici']
print(contoh_list)
contoh_set = {'Dewi', 'Budi', 'Cici', 'Linda', 'Cici'}
print(contoh_set)
contoh_frozen_set = ({'Dewi', 'Budi', 'Cici', 'Linda', 'Cici'})
print(contoh_frozen_set)
```
### Mapping Type
Tipe data mapping dapat digunakan untuk memetakan sebuah nilai ke nilai lainnya. Dalam Python, tipe data mapping disebut dengan istilah dictionary. Tipe data dictionary dapat dideklarasikan dengan diawali oleh tanda kurung buka kurawal ( { ), memisahkan setiap elemen di dalamnya dengan tanda koma ( , ) dan ditutup dengan tanda kurung kurawal ( } ). Setiap elemen pada tipe data dictionary dideklarasikan dengan format:
"kunci" : "nilai"

### Tugas:
Menggunakan tipe data mapping, aku diminta Senja untuk menampilkan nama & pekerjaan John Doe, seorang Programmer.
```sh
person = {'nama': 'John Doe', 'pekerjaan' : 'Programmer'}
print(person['nama'])
print(person['pekerjaan'])
```

### Tugas Praktek
Ternyata seru juga! Aku jadi berniat mengembangkan program kalkulator potongan harga ini untuk beberapa barang sekaligus agar lebih fungsional. Kalau begitu, aku perlu rapikan dulu informasi setiap barang di tabel ini.
“Lalu, aku tinggal merepresentasikan semuanya ke tipe data dictionary, dengan begitu akan lebih mudah mengolahnya,” gumamku.
Aku pun mulai mendeklarasikan variabel sepatu, baju, dan celana untuk menampung informasi barang ke dalam live code editor.
Nama Barang : Sepatu Niko, Baju Unikloh, Celana Lepis
Harga : 150000, 80000, 200000
Diskon :30000, 8000, 60000

```sh
sepatu = {"nama": 'Sepatu Niko', "harga": 150000, "diskon": 30000}
baju = {"nama": 'Baju Unikloh', "harga": 80000, "diskon": 8000}
celana = {"nama": 'Celana Lepis', "harga": 200000, "diskon": 60000}
```
### Tugas Praktek
Setelah berhasil merepresentasikan setiap barang ke dalam tipe data dictionary dengan variabel nama, harga, dan diskon, langkahku selanjutnya adalah: mendeklarasikan list dengan nama daftar_belanja yang berisi data sepatu, baju, dan celana.

```sh
sepatu = {"nama": "Sepatu Niko", "harga": 150000, "diskon": 30000} 
baju = {"nama": "Baju Unikloh", "harga": 80000, "diskon": 8000} 
celana = {"nama": "Celana Lepis", "harga": 200000, "diskon": 60000} 
daftar_belanja = ['sepatu', 'baju', 'celana']
```

### Tugas Praktek
Dengan data yang aku miliki, aku bisa menghitung total harga jual dengan potongan harga beserta pajak sebesar 10% dari nilai jual.
Untungnya Senja memberikan beberapa tips untuk menyelesaikan tugas ini:
Tips 1. # Data yang dinyatakan ke dalam dictionary
Tips 2. # Hitung harga masing-masing data setelah dikurangi diskon
Tips 3. # Hitung harga total
Tips 4. # Hitung harga kena pajak
Tips 5. # Cetak total_harga + total_pajak

```sh
# Data yang dinyatakan ke dalam dictionary
sepatu = {"nama": "Sepatu Niko", "harga": 150000, "diskon": 30000} 
baju = {"nama": "Baju Unikloh", "harga": 80000, "diskon": 8000} 
celana = {"nama": "Celana Lepis", "harga": 200000, "diskon": 60000}
# Hitunglah harga masing-masing data setelah dikurangi diskon
harga_sepatu = sepatu["harga"] - sepatu["diskon"] 
harga_baju = baju["harga"] - baju["diskon"]
harga_celana = celana["harga"] - celana["diskon"]
# Hitung harga total
total_harga = harga_sepatu + harga_baju + harga_celana
# Hitung harga kena pajak
total_pajak = total_harga * 0.1
# Cetak total_harga + total_pajak
print(total_harga + total_pajak)
```

## Python Operators

### Pendahuluan
Setelah aku berhasil mempelajari detail terkait dengan variables dan data type, sekarang aku akan mempelajari operator-operator yang tersedia di dalam Python. Di dalam Python, operator terbagi ke dalam 6 kelompok:
1. Arithmetic operators
2. Assignment operators
3. Comparison operators
4. Logical operators
5. Identity operators
6. Membership operators

| **Operator Type**        | **Operator** | **Description**                                                           | **Example**            | **Result**   |
| ------------------------ | ------------ | ------------------------------------------------------------------------- | ---------------------- | ------------ |
| **Arithmetic Operators** | `+`          | Addition (penjumlahan)                                                    | `5 + 3`                | `8`          |
|                          | `-`          | Subtraction (pengurangan)                                                 | `10 - 4`               | `6`          |
|                          | `*`          | Multiplication (perkalian)                                                | `6 * 2`                | `12`         |
|                          | `/`          | Division (pembagian)                                                      | `9 / 2`                | `4.5`        |
|                          | `//`         | Floor Division (pembagian bulat)                                          | `9 // 2`               | `4`          |
|                          | `%`          | Modulus (sisa bagi)                                                       | `9 % 2`                | `1`          |
|                          | `**`         | Exponentiation (pangkat)                                                  | `2 ** 3`               | `8`          |
| **Assignment Operators** | `=`          | Assign value (memberi nilai)                                              | `x = 5`                | `x = 5`      |
|                          | `+=`         | Add and assign                                                            | `x += 3` (jika `x=5`)  | `x = 8`      |
|                          | `-=`         | Subtract and assign                                                       | `x -= 2` (jika `x=5`)  | `x = 3`      |
|                          | `*=`         | Multiply and assign                                                       | `x *= 4` (jika `x=3`)  | `x = 12`     |
|                          | `/=`         | Divide and assign                                                         | `x /= 2` (jika `x=6`)  | `x = 3.0`    |
|                          | `//=`        | Floor divide and assign                                                   | `x //= 2` (jika `x=5`) | `x = 2`      |
|                          | `%=`         | Modulus and assign                                                        | `x %= 2` (jika `x=5`)  | `x = 1`      |
|                          | `**=`        | Power and assign                                                          | `x **= 3` (jika `x=2`) | `x = 8`      |
| **Comparison Operators** | `==`         | Equal to                                                                  | `5 == 5`               | `True`       |
|                          | `!=`         | Not equal to                                                              | `5 != 3`               | `True`       |
|                          | `>`          | Greater than                                                              | `7 > 3`                | `True`       |
|                          | `<`          | Less than                                                                 | `2 < 5`                | `True`       |
|                          | `>=`         | Greater than or equal                                                     | `5 >= 5`               | `True`       |
|                          | `<=`         | Less than or equal                                                        | `4 <= 6`               | `True`       |
| **Logical Operators**    | `and`        | Returns `True` if both are true                                           | `(5 > 3) and (2 < 4)`  | `True`       |
|                          | `or`         | Returns `True` if at least one is true                                    | `(5 > 3) or (2 > 10)`  | `True`       |
|                          | `not`        | Negates result                                                            | `not (5 > 3)`          | `False`      |
| **Identity Operators**   | `is`         | Returns `True` if two variables are the same object (same memory address) | `x is y`               | `True/False` |
|                          | `is not`     | Returns `True` if two variables are not the same object                   | `x is not y`           | `True/False` |
| **Membership Operators** | `in`         | Returns `True` if value is in sequence                                    | `'a' in 'apple'`       | `True`       |
|                          | `not in`     | Returns `True` if value is not in sequence                                | `'b' not in 'apple'`   | `True`       |


### Nilai Prioritas Operator dalam Python – Part 1
Info: materi telah diperbarui pada tanggal 29 Januari 2022, pastikan kembali kode yang telah ditulis disesuaikan dengan bagian Lesson.
Setelah mempelajari berbagai operator dalam bahasa pemrograman Python, tentunya aku juga ingin bisa menuliskan operasi-operasi variabel yang bersifat ekspresif dan ringkas.

### Tugas:
Aku diminta Senja untuk menghitung harga yang harus dibayarkan menggunakan barang senilai 150,000, dengan diskon 30% dan pajak 10%, menggunakan cara yang aku gunakan awal dan cara lebih singkat yang diajarkan Senja. 
```sh
# Kode awal
total_harga = 150000
potongan_harga = 0.3
pajak = 0.1 # pajak dalam persen ~ 10%
harga_bayar = 1 - potongan_harga  # baris pertama
harga_bayar *= total_harga # baris kedua
pajak_bayar = pajak * harga_bayar # baris ketiga
harga_bayar += pajak_bayar # baris ke-4
print("Kode awal - harga_bayar=", harga_bayar)
# Penyederhanaan baris kode dengan menerapkan prioritas operator
total_harga = 150000
potongan_harga = 0.3
pajak = 0.1 # pajak dalam persen ~ 10%
harga_bayar = (1 - potongan_harga) * total_harga #baris pertama 
harga_bayar += harga_bayar * pajak # baris kedua
print("Penyederhanaan kode - harga_bayar=", harga_bayar)
```

### Tugas Praktek
Senja memang hebat! 
Aku baru sadar, dengan struktur penulisan yang tepat maka penulisan syntax dapat dipersingkat untuk menjadi lebih simpel. 
Kenapa tidak terpikirkan olehku, ya? Harusnya aku tidak perlu mendeklarasikan variabel total_pajak dan aku bisa langsung menampung hasil perhitungan akhir saat mendeklarasikan variabel total_harga. Jadi, kodeku akan berjalan jika aku menambahkan setiap harga barang yang telah dipotong diskon sebelum menghitung pajak.

### Tugas:
Dengan cara yang diajarkan Senja, aku akan membuat potongan kode diatas menjadi lebih simpel. Jangan lupa ada pajak 10%.
```sh
sepatu = { "nama" : "Sepatu Niko", "harga": 150000, "diskon": 30000 }
baju = { "nama" : "Baju Unikloh", "harga": 80000, "diskon": 8000 }
celana = { "nama" : "Celana Lepis", "harga": 200000, "diskon": 60000 }
harga_sepatu = sepatu["harga"] - sepatu["diskon"]
harga_baju = baju["harga"] - baju["diskon"]
harga_celana = celana["harga"] - celana["diskon"]
total_harga = (harga_sepatu + harga_baju + harga_celana) * 1.1 
print(total_harga)
```

## Python Control Flow

### Python Conditioning for Decision – Part 1
Layaknya bahasa pemrograman lainnya, bahasa pemrograman Python menyediakan flow control statement untuk berinteraksi dengan variabel bertipe boolean dan operator logika. Flow control statement dalam Python dapat dituliskan dengan menggunakan format berikut:
```sh
if conditions:
    do_action_1
    ...
    do_action_n
```
Dengan <conditions> berisikan operator yang mengembalikan nilai kebenaran; ataupun beberapa operator yang mengembalikan nilai kebenaran, yang digabungkan dengan operator logika.  Melalui  sebuah flow control statement (if statement), <do_action_1> sampai dengan <do_action_n> akan dijalankan saat <conditions> bernilai True.
Dalam menuliskan serangkaian aksi (<do_action_1>, ... , <do_action_n>) dalam sebuah statemen if, aku harus mengemas setiap aksi dalam sebuah blok dengan menambahkan indentasi (jorokan) dari pada aksi.

### Python Conditioning for Decision – Part 2
### Tugas:
Praktekkan kode berikut di live code editor pada baris setelah kode sebelumnya yang telah dibuat.
### ps: Aku juga bisa mengubah nilai x sehingga lebih mudah memahami flow control statement mana yang akan dieksekusi oleh potongan kode yang telah aku jalankan.
```sh
# Statement if
x = 4
if x % 2 == 0: # jika sisa bagi x dengan 2 sama dengan 0
    print("x habis dibagi dua") # statemen aksi lebih menjorok ke dalam
# Statement if ... elif ... else
x = 7 
if x % 2 == 0: # jika sisa bagi x dengan 2 sama dengan 0
    print("x habis dibagi dua")
elif x % 3 == 0: # jika sisa bagi x dengan 3 sama dengan 0
    print("x habis dibagi tiga")
elif x % 5 == 0: # jika sisa bagi x dengan 5 sama dengan 0
    print("x habis dibagi lima")
else:
    print("x tidak habis dibagi dua, tiga ataupun lima")
```

### Python Conditioning for Decision – Part 3
Dari yang aku pelajari pada bagian awal dari flow control statement, conditional operator juga dapat digunakan dengan operator logika. 
Sebagai catatan tambahan, aku juga belajar bahwa aksi dalam sebuah flow control statement dapat dituliskan flow control statement tambahan (lainnya) secara bersarang yang dikenal dengan istilah nested if.
```sh
jam = 13
if jam >= 5 and jam < 12: # selama jam di antara 5 s.d. 12
    print("Selamat pagi!")
elif jam >= 12 and jam < 17: # selama jam di antara 12 s.d. 17
    print("Selamat siang!")
elif jam >= 17 and jam < 19: # selama jam di antara 17 s.d. 19
    print("Selamat sore!")
else: # selain kondisi di atas
    print("Selamat malam!")
```
### ugas Praktek
Aku diminta tolong Senja untuk menghitung tagihan pembayaran karena saat ini prosesnya masih manual.
### Tugas:
“Aksara, kantor kita akan merilis penawaran baru terkait jasa pembuatan data warehouse. Bisa tolong kembangkan kalkulatormu untuk menghitung tagihan pembayaran? Soalnya selama ini kita masih manual,” jelas Senja sembari memberikan contoh nota tagihan kantor.
Aku belum mengiyakan karena sedikit ragu. Mengingat sebelumnya aku sempat salah. Tapi dalam hati aku berkata, pasti bisa! Kali ini aku harus mampu membuat kalkulator lebih rumit.
Solusi yang terlintas dalam bayanganku: Kalkulator ini harus dapat menghitung subtotal setiap jasa yang diambil dari kolom harga/ hari dan total hari dari setiap jasa. Ternyata Senja juga memikirkan hal yang sama dengan instruksinya yang sangat membantu.
| **Nama Jasa**       | **Harga per Hari (Rp)** | **Total Hari** | **Subtotal (Rp)** |
| ------------------- | ----------------------- | -------------- | ----------------- |
| Data Warehousing    | 1.000.000               | 15             | 15.000.000        |
| Data Cleansing      | 1.500.000               | 10             | 15.000.000        |
| Data Integration    | 2.000.000               | 15             | 30.000.000        |
| Data Transformation | 2.500.000               | 10             | 25.000.000        |
| **Total**           |                         |                | **85.000.000**    |

```sh
tagihan_ke = 'Mr. Yoyo'
warehousing = { 'harga_harian': 1000000, 'total_hari':15 } 
cleansing = { 'harga_harian': 1500000, 'total_hari':10 } 
integration = { 'harga_harian':2000000, 'total_hari':15 } 
transform = { 'harga_harian':2500000, 'total_hari':10 }
sub_warehousing = warehousing['harga_harian'] * warehousing['total_hari']
sub_cleansing = cleansing['harga_harian'] * cleansing['total_hari'] 
sub_integration = integration['harga_harian'] * integration['total_hari'] 
sub_transform = transform['harga_harian'] * transform['total_hari']
total_harga = sub_warehousing + sub_cleansing + sub_integration + sub_transform
print("Tagihan kepada:") 
print(tagihan_ke)
print("Selamat pagi, anda harus membayar tagihan sebesar:") 
print(total_harga)
```

### Tugas Praktek
Aku menunjukkan potongan kode dan hasil dari kalkulator yang telah aku buat ke Senja yang sudah berhasil menampilkan kalimat:
Selamat pagi, Anda harus membayar tagihan sebesar:
Kulihat kedua alis Senja bertaut, ini pertanda kodeku pasti ada yang keliru.
“Kalau kamu hanya memasukkan perintah ‘selamat pagi’ seakan kalau tagihan ini dikirim hanya saat pagi, padahal bisa kapan saja sesuai kebutuhan,” komentar Senja. Begini, jam pengiriman email kantor kita mulai dari 6 pagi sampai 9 malam.
### Tugas:
Tolong masukkan variabel keterangan waktu tersebut di kodemu. Lalu, diatur dengan detail berikut:
1. Diatas jam 07 malam adalah salam 'selamat malam'
2. Diatas jam 05 sore adalah salam 'selamat sore'
3. Diatas jam 12 siang, adalah 'selamat siang'
4. dan selain itu 'selamat pagi'

“Oh, oke. Paham,” sahutku sembari merevisi. Saran yang bagus, kedepannya aku harus berpikir kritis.
```sh
jam = 17
tagihan_ke = 'Mr. Yoyo'
warehousing = { 'harga_harian': 1000000, 'total_hari':15 } 
cleansing = { 'harga_harian': 1500000, 'total_hari':10 } 
integration = { 'harga_harian':2000000, 'total_hari':15 } 
transform = { 'harga_harian':2500000, 'total_hari':10 }
sub_warehousing = warehousing['harga_harian']*warehousing['total_hari'] 
sub_cleansing = cleansing['harga_harian']*cleansing['total_hari'] 
sub_integration = integration['harga_harian']*integration['total_hari'] 
sub_transform = transform['harga_harian']*transform['total_hari']
total_harga = sub_warehousing+sub_cleansing+sub_integration+sub_transform
print("Tagihan kepada:")
print(tagihan_ke)
if jam > 19:
    print("Selamat malam, anda harus membayar tagihan sebesar:")
elif jam > 17:
    print("Selamat sore, anda harus membayar tagihan sebesar:") 
elif jam > 12:
    print("Selamat siang, anda harus membayar tagihan sebesar:")
else:
    print("Selamat pagi, anda harus membayar tagihan sebesar:") 
print(total_harga)
```

### Python Primitive Loop Control
Loop Control merupakan salah satu fitur yang mengizinkan penggunanya untuk melakukan serangkaian aksi, selama suatu kondisi yang telah ditetapkan bernilai benar. Dalam Python, terdapat dua bentuk primitif dari loop kontrol (struktur pengulangan), yaitu
1. while loops
2. for loops

### Python while loops – Part 1
Pertama-tama aku mempelajari struktur kontrol while loops . 
### Tugas 1:
Hitung total tagihan secara manual dengan menulis potongan kode berikut ke dalam live code editor.
### Tugas 2:
Ubah potongan kode yang telah dibuat dengan arahan Senja dan tuliskan di dalam live code editor.
```sh
# Tagihan
tagihan = [50000, 75000, 125000, 300000, 200000]
# Tanpa menggunakan while loop
total_tagihan = tagihan[0] + tagihan[1] +tagihan[2] +tagihan[3] + tagihan[4]
print(total_tagihan)
# Dengan menggunakan while loop
i = 0 # sebuah variabel untuk mengakses setiap elemen tagihan satu per satu
jumlah_tagihan = len(tagihan) # panjang (jumlah elemen dalam) list tagihan
total_tagihan = 0 # mula-mula, set total_tagihan ke 0
while i < jumlah_tagihan: # selama nilai i kurang dari jumlah_tagihan
    total_tagihan += tagihan[i] # tambahkan tagihan[i] ke total_tagihan
    i += 1 # tambahkan nilai i dengan 1 untuk memproses tagihan selanjutnya.
print(total_tagihan)
```

### Python while loops – Part 2
Dalam sebuah struktur kontrol pengulangan, aku dapat menggunakan perintah break untuk keluar dari struktur pengulangan dan perintah continue untuk melanjutkan proses pengulangan berikutnya. 
### Tugas:
Praktekkan potongan kode berikut pada live code editor.
```sh
tagihan = [50000, 75000, -150000, 125000, 300000, -50000, 200000]
i = 0
jumlah_tagihan = len(tagihan)
total_tagihan = 0
while i < jumlah_tagihan:
    # jika terdapat tagihan ke-i yang bernilai minus (di bawah nol),
    # pengulangan akan dihentikan
    if tagihan[i] < 0:
        total_tagihan = -1
        print("terdapat angka minus dalam tagihan, perhitungan dihentikan!")
        break
    total_tagihan += tagihan[i]
    i += 1
print(total_tagihan)
```

### Python while loops – Part 3
```sh
tagihan = [50000, 75000, -150000, 125000, 300000, -50000, 200000]
i = 0
jumlah_tagihan = len(tagihan)
total_tagihan = 0
while i < jumlah_tagihan:
    # jika terdapat tagihan ke-i yang bernilai minus (di bawah nol),
    # abaikan tagihan ke-i dan lanjutkan ke tagihan berikutnya
    if tagihan[i] < 0:
        i += 1
        continue
    total_tagihan += tagihan[i]
    i += 1
print(total_tagihan)
```

### Python for loops – Part 1
Untuk perintah for loops, aku mencoba potongan kode ini menggunakan live code editor.
Jika dijalankan maka akan mencetak output total tagihan sebesar 550000 (total tagihan positif).
```sh
list_tagihan = [50000, 75000, -150000, 125000, 300000, -50000, 200000]
total_tagihan = 0
for tagihan in list_tagihan: # untuk setiap tagihan dalam list_tagihan
    total_tagihan += tagihan # tambahkan tagihan ke total_tagihan
print(total_tagihan)
```

### Python for loops – Part 2
Serupa dengan struktur pengulangan while, aku juga dapat memanfaatkan statement break dan continue di dalamnya. Aku mencoba potongan kode di bawah menggunakan live code editor untuk penggunaan statement break.
```sh
list_tagihan = [50000, 75000, -150000, 125000, 300000, -50000, 200000]

# For loops with break
print("For loops with break")
total_tagihan_break = 0
for tagihan in list_tagihan :
    if tagihan < 0:
        print("Terdapat angka minus dalam tagihan, perhitungan dihentikan!")
        break
    total_tagihan_break += tagihan
print("Total tagihan %d." % total_tagihan_break)
print()

# For loops with continue
print("For loops with continue")
total_tagihan_continue = 0
for tagihan in list_tagihan:
    if tagihan < 0:
        print("Terdapat angka minus dalam tagihan, tagihan %d dilewati!" % tagihan)
        continue
    total_tagihan_continue += tagihan
print("Total tagihan %d." % total_tagihan_continue)
```

### Python for loops – Part 3
Ternyata, aku belajar bahwa ada istilah nested loops, yaitu pengulangan bersarang. Dengan nested loops, aku dapat mengkombinasikan (menambahkan) struktur pengulangan lain di dalamnya.  Aku mencoba potongan kode di bawah menggunakan live code editor:

```sh
list_daerah = ['Malang', 'Palembang', 'Medan']
list_buah = ['Apel', 'Duku', 'Jeruk']
for nama_daerah in list_daerah:
    for nama_buah in list_buah:
        print(nama_buah+" "+nama_daerah)
```

### Tugas Praktek
Aku diberi informasi oleh Senja bahwa manajemen cukup puas dengan hasil kalkulator potongan harga dan pajak yang aku kembangkan. Setelahnya, aku diberikan kepercayaan lebih untuk membuat program baru.
Dalam program kali ini, aku diminta untuk menghitung total pengeluaran dan pemasukan perusahaan.
Senja pun mengingatkan akan ada penghitungan cash flow.
Melihat Senja dan tim manajemen memberikan kepercayaan yang besar kepadaku, akupun bersemangat!
### Tugas:
Program yang akan aku bangun akan mengolah sebuah list yang bernama list_cash_flow. Setiap elemen dari list_cash_flow berisikan pengeluaran (bilangan negatif) dan pemasukan (bilangan positif) pada perusahaan
Dari list_cash_flow ini, aku akan menghitung total_pengeluaran dan total_pemasukan perusahaan. 
```sh
list_cash_flow = [
2500000, 5000000, -1000000, -2500000, 5000000, 10000000,
-5000000, 7500000, 10000000, -1500000, 25000000, -2500000
]
total_pengeluaran, total_pemasukan = 0, 0
for dana in list_cash_flow:
    if dana > 0:
        total_pemasukan += dana
    else:
        total_pengeluaran += dana
total_pengeluaran *= -1
print(total_pengeluaran) 
print(total_pemasukan)
```

### Quiz
### Pendahuluan
Berkat dua pekerjaan berturut-turut kemarin, aku sekarang diberi waktu senggang untuk beristirahat alias bereksplorasi sendiri. Senangnya!
Selama ini aku ingin sekali membantu usaha paman karena selama ini pamanku selalu kesulitan mencatat laporan pengeluaran bisnisnya. Kali ini aku sudah tahu caranya!
### Ekspedisi Pamanku
Aku menyambar ponsel di meja dan membuka pesan singkat dari paman tempo hari yang menjelaskan jika paman harus mengeluarkan uang sebesar 1,5 juta per mobil dalam sehari. Tapi, beliau selalu kebingungan dengan total pengeluaran per bulan karena adanya aturan ganjil-genap yang membuat pengoperasian mobil yang berbeda.

“Kalau begitu, aku akan masukkan variabel jumlah_hari berisi jumlah hari dalam sebulan dan variabel list_plat_nomor berisi seluruh nomor plat mobil milik paman,” gumamku sendiri. Kalau seperti ini paman hanya perlu mengganti variabel jumlah_hari atau modifikasi variabel list_plat_nomor untuk melacak total pengeluaran paman selama sebulan. Ide Cemerlang!

```sh
# Data
uang_jalan = 1500000
jumlah_hari = 31
list_plat_nomor = [8993, 2198, 2501, 2735, 3772, 4837, 9152]
# Pengecekan kendaraan dengan nomor pelat ganjil atau genap 
# Deklarasikan kendaraan_genap dan kendaraan_ganjil = 0
kendaraan_genap = 0 
kendaraan_ganjil = 0
for plat_nomor in list_plat_nomor:
    if plat_nomor % 2 == 0 :
        kendaraan_genap += 1 
    else:
        kendaraan_ganjil += 1
# Total pengeluaran untuk kendaraan dengan nomor pelat ganjil 
# dan genap dalam 1 bulan
i = 1
total_pengeluaran = 0
while i <= jumlah_hari:
    if i % 2 == 0:
        total_pengeluaran += (kendaraan_genap * uang_jalan)
    else:
        total_pengeluaran += (kendaraan_ganjil * uang_jalan) 
    i += 1
# Cetak total pengeluaran
print(total_pengeluaran)
```

### Hasil Belajarku
Wah senangnya! Aku telah berhasil menyelesaikan pelajaran Python pertamaku, Python for Data Professional Beginner - Part 1.
Selain membabat habis materi dari Senja, aku berhasil menyelesaikan latihan, dan membantu Pamanku.
Dari materi yang telah aku pelajari dan praktekkan, aku telah mempelajari:
Alasan Python secara luas digunakan dalam komputasi saintifik, web, ranah data (data domain).
Konstruksi dari struktur bahasa pemrograman Python.
Teknik mempraktekkan penggunaan tipe data pada Python.
Teknik mempraktekkan penggunaan jenis-jenis operator pada Python.
Teknik mempraktekkan penggunaan pengkondisian untuk pengambilan keputusan dan perulangan pada Python.
Program Python untuk penyelesaian kasus bisnis sederhana.
