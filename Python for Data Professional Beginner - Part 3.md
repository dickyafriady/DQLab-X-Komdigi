### DQLab x Komdigi
## Python for Data Professional Beginner - Part 3
# _Guide to Learn Python with AI at DQLab_

## Pengantar Object Oriented Programming
Pengantar Object Oriented Programming
Aku sudah sampai di modul ketiga pembelajaran Python. Kalau modul pertama aku masih bisa bilang lancar-lancar saja dan modul dua kian menantang, di modul ketiga ini aku masih belum punya gambaran.

Kuintip judul pertama pembelajaran modul ketiga berisi “Pengantar Object Oriented Programming”, “Classes & Objects”, “Encapsulation”, hingga “Polymorphism”. Waduh! Nama makhluk apa semua itu?

“Kok diintip aja? Lanjut dong,” celetuk Senja di sebelahku.

“Hehehe, siap. Kalau enggak paham, nanya-nanya boleh dong?”

“Silakan.”

Nah, kalau ada yang siap membimbing bakal semangat nih. Aku mulai membuka isi modul ketiga ini.

### Apa itu Object Oriented Programming?
Pemrograman Berbasis Objek (Object Oriented Programming - OOP) merupakan salah satu paradigma pemrograman yang cukup populer di antara paradigma-paradigma lainnya.
Pada paradigma OOP, struktur dari sebuah program dikemas ke dalam sebuah objek yang memiliki serangkaian properti (properties) dan fungsi (behaviours). Sebagai contoh, aku dapat merepresentasikan seorang karyawan ke dalam sebuah program melalui konsep OOP.
Seorang karyawan dapat memiliki serangkaian properti seperti nama, usia, keahlian, dll. Kemudian, seorang karyawan juga dapat memiliki fungsi-fungsi seperti hadir ke kantor, absen, lembur, tugas dinas, dll.

### Konsep dalam Object Oriented Programming
Sebagai salah satu bahasa pemrograman yang bersifat multi-purposive, Python juga mendukung paradigma Object Oriented (OO).

Konsep OO pada Python memiliki tujuan untuk menciptakan potongan-potongan kode yang bersifat reusable dan tidak redundan. Konsep ini dikenal dengan istilah konsep DRY - Don’t Repeat Yourself (berlawanan dengan konsep WET - Write Everything Twice).

Dalam bahasa pemrograman Python, terdapat 3 konsep utama OO yaitu.

1. Encapsulation: Menyembunyikan sebagian detail yang dimiliki oleh sebuah objek terhadap objek-objek lainnya.
2. Inheritance: Menurunkan serangkaian fungsi-fungsi yang dimiliki oleh sebuah objek ke sebuah objek baru tanpa mengubah makna dari objek acuan yang digunakan.
3. Polymorphism: Konsep untuk menggunakan fungsi-fungsi dengan nama/tujuan yang sama dengan cara yang berbeda.

### Classes & Objects
### Class dan Objek dalam Python - Part 1
Setiap objek yang aku representasikan dalam program berbasis OOP merupakan instansi/ bentuk nyata dari sebuah konsep yang disebut dengan class. Oleh karena itu, class dapat juga aku sebutkan sebagai kerangka utama (blueprint) dari objek. Untuk mempermudah pemahaman konsep OO, aku menggunakan contoh berikut:

Asumsikan aku ingin merepresentasikan Diriku dan Senja sebagai karyawan di suatu perusahaan X. Untuk merepresentasikan Diriku dan Senja, aku dapat membuat sebuah class yang nantinya akan mencakup properti-properti yang umumnya dimiliki oleh sebuah karyawan.

### Class dan Objek dalam Python - Part 2
Pada bagian pertama, aku telah berhasil membuat sebuah class dan objek-objek sebagai bentuk realisasi dari sebuah class. Akan tetapi, class yang telah aku definisikan belum memiliki atribut ataupun fungsi-fungsi yang dapat merepresentasikan objek Karyawan dengan baik.

Agar dapat membuat class Karyawan dengan baik, pertama, aku akan mempelajari cara merepresentasikan atribut/properti dalam sebuah class.  Dalam sebuah class, aku dapat mendefinisikan dua jenis atribut yaitu.

Class Attribute adalah properti/atribut yang bernilai sama untuk oleh seluruh objek 
Instance Attribute adalah properti/atribut yang nilainya berbeda-beda untuk setiap objek dari sebuah class.

### Class dan Objek dalam Python - Part 3
Berkaitan dengan kedua jenis atribut yang telah aku pelajari, aku menggunakan contoh berikut untuk memperkuat pemahamanku terkait dengan konsep class attribute.

Class Karyawan pada umumnya memiliki beberapa atribut seperti nama, usia, pendapatan serta nama perusahaan di mana karyawan tersebut bekerja. Untuk merepresentasikan diriku dan Senja sebagai karyawan yang bekerja di sebuah perusahaan yang sama (anggap saja perusahan ABC), aku dapat merepresentasikan dengan menggunakan konsep class attribute
### Tugas:
Aku di minta untuk mengerjakan tutorial sederhana untuk membantu memahami konsep OOP:

1. Definisikan Class Karyawan
2. Inisiasi object yang dinyatakan dalam variabel Aksara dan Senja
3. Cetak Nama Perusahaan melalui penggunaan keyword __class__
4. Ubah Nama Perusahaan menjadi 'DEF' 

```sh
# Definisikan class Karyawan
class Karyawan:
    nama_perusahaan = 'ABC'
# Inisiasi object yang dinyatakan dalam variabel aksara dan senja
aksara = Karyawan()
senja = Karyawan()
# Cetak nama perusahaan melalui penggunaan keyword __class__
# pada class attribute nama_perusahaan
print(aksara.__class__.nama_perusahaan)
# Ubah nama_perusahaan menjadi 'DEF'
aksara.__class__.nama_perusahaan = 'DEF'
# Cetak nama_perusahaan objek aksara dan senja
print(aksara.__class__.nama_perusahaan)
print(senja.__class__.nama_perusahaan)
```

### Class dan Objek dalam Python - Part 4
Pada bagian sebelumnya aku telah mempelajari contoh deklarasi class Karyawan; nama, usia dan pendapatan karyawan adalah contoh dari konsep instance attribute. Hal ini dikarenakan setiap karyawan tentunya dapat memiliki nama, usia dan pendapatan yang berbeda.
### Tugas
```sh
# Definisikan class Karyawan
class Karyawan:
    nama_perusahaan = 'ABC'
    def __init__(self, nama, usia, pendapatan):
        self.nama = nama
        self.usia = usia
        self.pendapatan = pendapatan
# Buat object bernama aksara dan senja
aksara = Karyawan('Aksara', 25, 8500000)
senja = Karyawan('Senja', 28, 12500000)
# Cetak objek bernama aksara
print(aksara.nama + ', Usia: ' + str(aksara.usia) + ', Pendapatan ' + str(aksara.pendapatan))
# Cetak objek bernama senja
print(senja.nama + ', Usia: ' + str(senja.usia) + ', Pendapatan ' + str(senja.pendapatan))
```

### Behavior pada Class
Selain dapat mendefinisikan atribut, dalam sebuah class, aku diperbolehkan untuk mendefinisikan fungsi-fungsi (behavior) dari sebuah class.

Dari potongan kode yang telah aku gunakan, aku dapat menambahkan fungsi-fungsi berkaitan dengan class Karyawan. Sebagai contoh, seorang karyawan tentunya mungkin saja memiliki pendapatan tambahan berdasarkan banyaknya kerja lembur dan jumlah proyek yang telah diselesaikan.

Tugas:
Untuk menghitung pendapatan tambahan dari jumlah kerja lembur  dan jumlah proyek yang diselesaikan oleh seorang karyawan dan mengakses pendapatan total dari seorang karyawan, aku dapat menuliskan potongan kode berikut.
```sh
#Definisikan class Karyawan berikut dengan attribut dan fungsinya
class Karyawan:
    nama_perusahaan = 'ABC'
    insentif_lembur = 250000
    def __init__(self, nama, usia, pendapatan):
        self.nama = nama
        self.usia = usia
        self.pendapatan = pendapatan
        self.pendapatan_tambahan = 0
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur
    def tambahan_proyek(self, insentif_proyek):
    	self.pendapatan_tambahan += insentif_proyek
    def total_pendapatan(self):
    	return self.pendapatan + self.pendapatan_tambahan
#Buat object dari karwayan bernama Aksara dan Senja
aksara = Karyawan('Aksara', 25, 8500000)
senja = Karyawan('Senja', 28, 12500000)
#Aksara melaksanakan lembur
aksara.lembur()
#Senja memiliki proyek tambahan
senja.tambahan_proyek(2500000)
# Cetak pendapatan total Aksara dan Senja
print('Pendapatan Total Aksara: ' + str(aksara.total_pendapatan()))
print('Pendapatan Total Senja: ' +str(senja.total_pendapatan()))
``` 

### Tugas Praktek
Seperti biasa, aku selalu pusing setiap usai membaca teori data. “Gimana, Aksara?” tanya Senja tanpa memalingkan perhatian dari laptop.

“Kayaknya butuh praktik deh,” sahutku.

“Oke, ini coba kamu bikin sistem manajemen perusahaan sederhana pakai Object Oriented (OO) ya. Artinya dalam program ini kamu harus mampu memuat informasi nama, alamat, nomor telepon, dan daftar karyawan yang bekerja. Satu lagi, jangan lupa masukkan fungsi untuk mengaktifkan dan menonaktifkan karyawan.”

“Siap. Ini aku masukkan informasi class karyawan juga kali yah?” tanyaku sembari bersiap-siap memasukkan kode dan mendaftar informasi karyawan secara lebih rapi, mulai dari nama, usia, pendapatan tetap, tambahan, dan insentif lembur.

“Bagus juga itu. Bikin saja pendapatan mula-mula karyawannya bernilai 0, lalu bisa bertambah oleh fungsi lembur dan fungsi tambahan proyek sebagai parameter dan variabel pendapatan tambahan karyawan.”

Aku mengangguk dan siap bertempur. Terakhir aku menyelipkan fungsi untuk menghitung total pendapatan. Ini paling penting, hehehe.

Tugas:
Lengkapi class Karyawan dan class Perusahaan menggunakan potongan kode pada Live Code Editor.
```sh
#Definisikan class Karyawan
class Karyawan:
    def __init__(self, nama, usia, pendapatan, insentif_lembur): 
        self.nama = nama
        self.usia = usia
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
        self.insentif_lembur = insentif_lembur
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, jumlah_tambahan):
        self.pendapatan_tambahan += jumlah_tambahan 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
#Definisikan class Perusahaan
class Perusahaan:
    def __init__(self, nama, alamat, nomor_telepon): 
        self.nama = nama
        self.alamat = alamat 
        self.nomor_telepon = nomor_telepon
        self.list_karyawan = []
    def aktifkan_karyawan(self, karyawan): 
        self.list_karyawan.append(karyawan)
    def nonaktifkan_karyawan(self, nama_karyawan): 
        karyawan_nonaktif = None
        for karyawan in self.list_karyawan:
            if karyawan.nama == nama_karyawan: 
                karyawan_nonaktif = karyawan 
                break
        if karyawan_nonaktif is not None: 
            self.list_karyawan.remove(karyawan_nonaktif)
```

### Tugas Praktek
Sekitar satu jam lebih berkutat depan laptop, kode aku kelar juga! Tapi, sebelum kutunjukkan pada Senja, lebih baik aku coba simulasikan dulu. Kuambil post-it kuning di ujung meja dan kugambar tabel berisi daftar perusahaan dan karyawan sebagai contoh, lengkap dengan pendapatan tetap dan tambahan yang diterima.

Nama Perusahaan: ABC
Alamat                  : Jl. Jendral Sudirman, Blok 11
No. Telp                : (021) 95205XX

| Nama Pekerja | Usia | Pendapatan (Rp) | Insentif Lembur (Rp) |
| ------------ | ---- | --------------- | -------------------- |
| Ani          | 25   | 8.500.000       | 100.000              |
| Budi         | 28   | 12.000.000      | 150.000              |
| Cici         | 30   | 15.000.000      | 200.000              |

Kalau sudah seperti ini, tinggal dimasukkan saja ke variabel list_karyawan, lalu operasikan. “Programnya berhasil!” batinku.

Tanpa kusadari ada tepukan halus di pundakku, itu dari Senja yang ternyata sedari tadi diam-diam memerhatikan hasil kerjaku.

“Nice try, Aksara.” Aku memandang puas dengan hasil kodeku kali ini.
```sh
class Karyawan:
    def __init__(self, nama, usia, pendapatan, insentif_lembur): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
        self.insentif_lembur = insentif_lembur 
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, jumlah_tambahan):
        self.pendapatan_tambahan += jumlah_tambahan 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan 

class Perusahaan:
    def __init__(self, nama, alamat, nomor_telepon): 
        self.nama = nama
        self.alamat = alamat 
        self.nomor_telepon = nomor_telepon
        self.list_karyawan = []
    def aktifkan_karyawan(self, karyawan): 
        self.list_karyawan.append(karyawan)
    def nonaktifkan_karyawan(self, nama_karyawan): 
        karyawan_nonaktif = None
        for karyawan in self.list_karyawan:
            if karyawan.nama == nama_karyawan: 
                karyawan_nonaktif = karyawan 
                break
        if karyawan_nonaktif is not None: 
            self.list_karyawan.remove(karyawan_nonaktif)

# Definisikan perusahaan
perusahaan = Perusahaan('ABC', 'Jl. Jendral Sudirman, Blok 11', '(021) 95205XX')
#Definisikan nama-nama karyawan
karyawan_1 = Karyawan('Ani', 25, 8500000, 100000)
karyawan_2 = Karyawan('Budi', 28, 12000000, 150000)
karyawan_3 = Karyawan('Cici', 30, 15000000, 200000)
#Aktifkan karyawan di perusahaan ABC
perusahaan.aktifkan_karyawan(karyawan_1)
perusahaan.aktifkan_karyawan(karyawan_2)
perusahaan.aktifkan_karyawan(karyawan_3)
```

### Encapsulation & Inheritance
### Encapsulation pada Python - Part 1
Praktik tadi yang dibantu Senja, membuatku lebih percaya diri untuk lanjut ke materi selanjutnya mengenai “Encapsulation & Inheritance”. Ini apa lagi yah? Aku membolak-balik halaman modul materi ini. Aku bersemangat untuk memulai!
Enkapsulasi (Encapsulation) adalah sebuah teknik dalam OOP yang mengizinkan aku untuk menyembunyikan detil dari sebuah atribut dalam sebuah class. Pada contoh-contoh sebelumnya, setiap atribut dan fungsi yang telah aku definisikan belum menggunakan konsep enkapsulasi, yang mengartikan bahwa setiap atribut dan fungsi dapat diakses di luar class.

### Encapsulation pada Python – Part 2
Pada contoh di atas, terlihat bahwa atribut nama pada setiap objek dapat diakses secara bebas di luar scope dari sebuah class. Agar suatu properti ataupun fungsi dari sebuah class tidak dapat diakses secara bebas di luar scope milik suatu class, aku dapat mendefinisikan access modifier (level akses) saat sebuah atribut/fungsi didefinisikan.

Terdapat 2 macam access modifier dalam Python, yakni.

1. Public access: dapat aku definisikan dengan secara langsung menuliskan nama dari atribut/ fungsi. Dalam sebuah objek, atribut/fungsi yang bersifat public access dapat diakses di luar scope sebuah class
2. Private access: dapat aku definisikan dengan menambahkan double underscore (__) sebelum menuliskan nama dari atribut/fungsi. Dalam sebuah objek, atribut/fungsi yang bersifat private access hanya dapat diakses di dalam scope sebuah class.

Tugas:
Untuk memperkuat pemahamanku terkait konsep enkapsulasi dalam paradigma OO, aku menggunakan contoh syntax dan mengetiknya pada live code editor:
```sh
#Definisikan class Karyawan
class Karyawan: 
    nama_perusahaan = 'ABC' 
    __insentif_lembur = 250000
    def __init__(self, nama, usia, pendapatan): 
        self.__nama = nama
        self.__usia = usia 
        self.__pendapatan = pendapatan 
        self.__pendapatan_tambahan = 0
    def lembur(self):
        self.__pendapatan_tambahan += self.__insentif_lembur 
    def tambahan_proyek(self, insentif_proyek):
        self.__pendapatan_tambahan +=insentif_proyek 
    def total_pendapatan(self):
        return self.__pendapatan + self.__pendapatan_tambahan
#Buat objek karyawan bernama Aksara
aksara = Karyawan('Aksara', 25, 8500000)
#Akses ke attribute class Karyawan
print(aksara.__class__.Karyawan)
#Akan menimbulkan error ketika di run
print(aksara.nama)
```
### Inheritance pada Python – Part 1
Inheritance adalah salah satu mekanisme di konsep OO yang mengizinkan aku untuk mendefinisikan sebuah class baru berdasarkan class yang sebelumnya telah dideklarasikan.

Melalui konsep inheritance, sebuah class baru dapat memiliki atribut dan fungsi pada class yang sebelumnya telah didefinisikan. Pada konsep inheritance, atribut/fungsi yang akan diwariskan hanyalah atribut/fungsi dengan access modifier public, atribut/fungsi dengan access modifier private tidak akan diturunkan.
```sh
#Definisikan class Karyawan (sebagai base class)
class Karyawan: 
    nama_perusahaan = 'ABC' 
    insentif_lembur = 250000
    def __init__(self, nama, usia, pendapatan): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, insentif_proyek):
        self.pendapatan_tambahan += insentif_proyek 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
#Buat class turunan (sebagai inherit class) dari class karyawan, 
#yaitu class AnalisData
class AnalisData(Karyawan):
    def __init__(self, nama, usia, pendapatan):
    #melakukan pemanggilan konstruktur class Karyawan 
        super().__init__(nama, usia, pendapatan)
#Buat kembali class turunan (sebagai inherit class) dari class karyawan,  
#yaitu class IlmuwanData
class IlmuwanData(Karyawan):
    def __init__(self, nama, usia, pendapatan):
        #melakukan pemanggilan konstruktur class Karyawan 
        super().__init__(nama, usia, pendapatan)
#Buat objek karyawan yang bekerja sebagai AnalisData
aksara = AnalisData('Aksara', 25, 8500000)
aksara.lembur()
print(aksara.total_pendapatan())
#Buat objek karyawan yang bekerja sebagai IlmuwanData
senja = IlmuwanData('Senja', 28, 13000000)
senja.tambahan_proyek(2000000)
print(senja.total_pendapatan())
```

### Inheritance pada Python – Part 2
Pada bagian pertama aku telah mempelajari bagaimana child class mewarisi fungsi/atribut dari parent class dengan menggunakan fungsi super(). Melalui konsep inheritance, child class dapat memodifikasi atribut/ fungsi yang diwarisi oleh sebuah parent class dengan mendefinisikan ulang atribut/ fungsi menggunakan nama yang sama. 

```sh
#Definisikan class Karyawan (sebagai base class)
class Karyawan: 
    nama_perusahaan = 'ABC' 
    insentif_lembur = 250000
    def __init__(self, nama, usia, pendapatan): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, insentif_proyek):
        self.pendapatan_tambahan += insentif_proyek 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
#Buat class turunan (sebagai inherit class) dari class karyawan, 
#yaitu class AnalisData
class AnalisData(Karyawan):
    def __init__(self, nama, usia, pendapatan):
    #melakukan pemanggilan konstruktur class Karyawan 
        super().__init__(nama, usia, pendapatan)
#Buat kembali class turunan (sebagai inherit class) dari class karyawan,  
#yaitu class IlmuwanData
class IlmuwanData(Karyawan):
    # mengubah atribut insentif_lembur yang digunakan pada fungsi lembur()
    insentif_lembur = 500000
    def __init__(self, nama, usia, pendapatan):
        super().__init__(nama, usia, pendapatan)
#Buat objek karyawan yang bekerja sebagai AnalisData
aksara = AnalisData('Aksara', 25, 8500000)
aksara.lembur()
print(aksara.total_pendapatan())
#Buat objek karyawan yang bekerja sebagai IlmuwanData
senja = IlmuwanData('Senja', 28, 13000000)
senja.lembur()
print(senja.total_pendapatan())
```

### Polymorphism & Overloading
### Polymorphism pada Python - Part 1
Selain dapat mendefinisikan ulang nilai dari atribut yang diwarisi oleh parent class seperti pada contoh di atas, aku juga dapat juga dapat mendefinisikan ulang fungsi yang telah diwarisi oleh parent class.

Saat aku mendefinisikan kembali fungsi yang telah diwarisi oleh parent class, secara tidak langsung aku telah menerapkan salah satu mekanisme yang secara khusus pada paradigma OO disebut dengan istilah polymorphism.
```sh
#Definisikan class Karyawan (sebagai base class)
class Karyawan: 
    nama_perusahaan = 'ABC' 
    insentif_lembur = 250000
    def __init__(self, nama, usia, pendapatan): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, insentif_proyek):
        self.pendapatan_tambahan += insentif_proyek 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
#Buat class turunan (sebagai inherit class) dari class karyawan, 
#yaitu class AnalisData
class AnalisData(Karyawan):
    def __init__(self, nama, usia, pendapatan):
    #melakukan pemanggilan konstruktur class Karyawan 
        super().__init__(nama, usia, pendapatan)
    #menerapkan polymorphism dengan mendefinisikan kembali fungsi 
    #lembur() pada class AnalisData 
    def lembur(self):
        #pendapatan tambahan pada class AnalisData sebesar
        #10 % dari pendapatannya.
        self.pendapatan_tambahan += int(self.pendapatan * 0.1)
#Buat objek karyawan yang bekerja sebagai AnalisData
aksara = AnalisData('Aksara', 25, 8500000)
aksara.lembur()
print(aksara.total_pendapatan())
```

### Polymorphism pada Python - Part 2
Pada konsep inheritance, melalui fungsi super(), selain dapat mengakses constructor milik parent class, child class juga dapat mengakses atribut/fungsi yang dimiliki oleh parent class.

```sh
#Definisikan class Karyawan (sebagai base class)
class Karyawan: 
    nama_perusahaan = 'ABC' 
    insentif_lembur = 250000
    def __init__(self, nama, usia, pendapatan): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, insentif_proyek):
        self.pendapatan_tambahan += insentif_proyek 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
#Buat class turunan (sebagai inherit class) dari class karyawan, 
#yaitu class AnalisData
class AnalisData(Karyawan):
    def __init__(self, nama, usia, pendapatan): 
        super().__init__ (nama, usia, pendapatan)
    #mendefinisikan kembali fungsi lembur() pada class AnalisData 
    def lembur(self):
        #memanggil fungsi lembur pada class Karyawan 
        super().lembur()
        #pendapatan tambahan pada class AnalisData sebesar
        #5 % dari pendapatannya.
        self.pendapatan_tambahan += int(self.pendapatan * 0.05)
#Buat objek karyawan yang bekerja sebagai AnalisData
aksara = AnalisData('Aksara', 25, 8500000)
aksara.lembur()
print(aksara.total_pendapatan())
```

### Tugas Praktek
Aku tak pernah membayangkan diriku benar-benar mengerjakan program untuk kebutuhan perusahaan. Seperti sekarang, aku sedang mengerjakan rikues untuk memenuhi penghitungan pembayaran fee karyawan lepas. 

Tapi tak apa. Sejak program yang terakhir berhasil, aku sedikit lebih percaya diri untuk menjawab tantangan baru.

Sembari menyeruput kopi hangat, aku mulai memasukkan informasi yang cukup untuk membuat class Tenaga Lepas berisi nama, usia, dan pendapatan selama bergabung di sebuah proyek. Lalu, apa lagi ya?

“Nja, mau nanya. Kalau karyawan lepas, insentif tambahannya dari uang lembur juga?”

“Engga, Aksara. Di kantor kita, karyawan lepas dapat insentif dari proyek yang dikerjakan. Kalau hasilnya sukses bisa dapat 1% dari nilai proyek.”

“Oke,” aku mencatat itu sebagai penghitungan akhir dan mulai menulis kodenya.
```sh
# Definisikan class Karyawan
class Karyawan:
    def __init__(self, nama, usia, pendapatan, insentif_lembur): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
        self.insentif_lembur = insentif_lembur 
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self,jumlah_tambahan):
        self.pendapatan_tambahan += jumlah_tambahan 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
# Definisikan class TenagaLepas sebagai child class dari
# class Karyawan
class TenagaLepas(Karyawan):
    def __init__(self, nama, usia, pendapatan):
        super().__init__(nama, usia, pendapatan, 0)
    def tambahan_proyek(self, nilai_proyek):
        self.pendapatan_tambahan += int(nilai_proyek * 0.01)
```
### Tugas Praktek
Di luar sudah menggelap. Gerobak nasi goreng yang biasanya menunggu di depan kantor tiap pukul tujuh sudah tampak. Aku masih saja larut dalam pekerjaan.

“Masih di sini, Aksara? Belum pulang?” tegur Senja yang baru saja keluar dari ruangan.

“Masih ngurusin proyek Tenaga Lepas. Ini baru dapat rikues lagi untuk nambahin class yang merepresentasikan masing-masing pekerjaan di divisi ini.”

“Hmm, kamu pakai konsep inherintance saja, akan lebih mudah,” saran Senja sebelum pulang. Sejujurnya, aku juga mau pulang. Teringat kasur di rumah yang siap untuk rebahan. Kalau begitu, pekerjaan ini harus cepat diselesaikan.

Di divisiku ada empat bidang pekerjaan, mulai dari analisis data, ilmuwan data, pembersih data, dan dokumenter teknis. Setiap peran punya sistem penerimaan fee yang berbeda. Ini yang bikin rumit. Misalnya, ilmuwan data akan mendapat insentif tambahan sebesar 10% dari proyek yang dikerjakan, dan dokumenter teknis adalah satu-satunya peran yang tidak menerima insentif dari proyek.

Oke, tenang. Ini pasti bisa, tinggal masukkin saja variabelnya satu persatu. Semangat! batinku sembari ditemani suara abang nasi goreng yang menjajakan makanannya.

Aku kembali bekerja dengan data dan kode-kode ini di code editor.

```sh
# Definisikan class Karyawan sebagai parent class
class Karyawan:
    def __init__(self, nama, usia, pendapatan, insentif_lembur): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
        self.insentif_lembur = insentif_lembur 
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self,jumlah_tambahan):
        self.pendapatan_tambahan += jumlah_tambahan 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
# Definisikan class TenagaLepas sebagai child class dari
# class Karyawan
class TenagaLepas(Karyawan):
    def __init__(self, nama, usia, pendapatan):
        super().__init__(nama, usia, pendapatan, 0)
    def tambahan_proyek(self, nilai_proyek):
        self.pendapatan_tambahan += int(nilai_proyek * 0.01)
# Definisikan class AnalisData sebagai child class dari
# class Karyawan
class AnalisData(Karyawan): 
    pass
# Definisikan class IlmuwanData sebagai child class dari
# class Karyawan
class IlmuwanData(Karyawan):
    def tambahan_proyek(self, nilai_proyek): 
        self.pendapatan_tambahan += int(0.1 * nilai_proyek)
# Definisikan class PembersihData sebagai child class dari
# class TenagaLepas
class PembersihData(TenagaLepas): 
    pass
# Definisikan class DokumenterTeknis sebagai child class dari
# class TenagaLepas
class DokumenterTeknis(TenagaLepas):
    def tambahan_proyek(self, jumlah_tambahan): 
        return
```

### Overloading
Pada bahasa pemrograman lain yang mendukung paradigma OO seperti C# ataupun Java, polymorphism juga dapat diterapkan melalui sebuah fitur yang dikenal dengan istilah metode overloading.

Metode overloading mengizinkan sebuah class untuk memiliki sekumpulan fungsi dengan nama yang sama dan parameter yang berbeda. Berkaitan dengan hal ini, Python tidak mengizinkan pendeklarasian fungsi (baik pada class ataupun tidak) dengan nama yang sama.

Untuk mengimplementasikan method overloading pada Python, aku dapat menggunakan sebuah teknik yang dikenal dengan function default parameters.

### Tugas Praktek
Perusahaan ABC memiliki 3 orang karyawan baru seperti yang diberikan dalam tabel berikut:
| Nama | Usia | Pendapatan (Rp) |
| ---- | ---- | --------------- |
| Budi | ?    | ?               |
| Didi | 25   | ?               |
| Hadi | ?    | 8.000.000       |

Aku di minta untuk mengisi tabel dengan detail sebagai berikut:

Budi berusia 21 dan pendapatan = 5000000
Didi berusia 25 dan pendapatan = 5000000
Hadi berusia 21 dan pendapatan = 8000000

```sh
class Karyawan: 
    nama_perusahaan = 'ABC' 
    insentif_lembur = 250000
    #usia akan di-set nilainya menjadi 21 saat tidak
    #dispesifikasikan dan pendapatan akan di-set nilainya
    #menjadi 5000000 saat tidak dispesifikasikan
    def __init__(self, nama, usia=21, pendapatan=5000000): 
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan 
        self.pendapatan_tambahan = 0
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur 
    def tambahan_proyek(self, insentif_proyek):
        self.pendapatan_tambahan += insentif_proyek 
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan
#Karyawan baru pertama yang bernama Budi
karyawan_baru1 = Karyawan('Budi')
print(karyawan_baru1.nama)
print(karyawan_baru1.usia)
print(karyawan_baru1.total_pendapatan())
#Karyawan baru ke-2 yang bernama Didi, umur 25
karyawan_baru2 = Karyawan('Didi', 25)
print(karyawan_baru2.nama)
print(karyawan_baru2.usia)
print(karyawan_baru2.total_pendapatan())
#Karyawan baru ke-3 yang bernama Hadi, pendapatan 8000000
karyawan_baru3 = Karyawan('Hadi', pendapatan=8000000)
print(karyawan_baru3.nama)
print(karyawan_baru3.usia)
print(karyawan_baru3.total_pendapatan())
```

### Pendahuluan
Keesokan harinya, aku menerima kabar mengejutkan sekaligus membahagiakan dari Senja: aku lulus untuk pembelajaran programming dengan Object Oriented (OO). Senyum tak lepas dari bibirku sejak menerima informasi itu.

“Untuk itu, kamu dianggap layak untuk mengerjakan proyek yang lebih besar,” tambah Senja. Aku sampai lupa, di sini kalau dianggap performanya baik, hadiahnya berupa pekerjaan dengan tanggung jawab lebih. Memang benar kata orang bijak, semakin tinggi pohon tumbuh, semakin tinggi angin menerpa.

“Apa, Nja?”

“Praktik uji konsep OOP,” jawab Senja mantap sembari memberikan soal studi kasus padaku.

Studi Kasus dari Senja
Di perusahaan ini, seorang analis data yang masuk umumnya berusia 21, memiliki pendapatan senilai 6.500.000 dan insentif lembur senilai 100.000. Kemudian, untuk seorang ilmuwan data yang masuk umumnya berusia 25, memiliki pendapatan senilai 12.000.000, dan insentif lembur senilai 150.000. Di sisi lain, untuk tenaga lepas, hanya terdapat pendapatan umum senilai 4.000.000 untuk pembersih data dan 2.500.000 untuk dokumenter teknis. 

Berikut adalah data perusahaan beserta detail karyawan yang bekerja.

Nama Perusahaan: ABC
Alamat                  : Jl. Jendral Sudirman, Blok 11
Telepon                 : (021) 95812XX

| Nama | Usia | Pekerjaan         | Pendapatan (Rp) |
| ---- | ---- | ----------------- | --------------- |
| Ani  | 25   | Pembersih Data    | -               |
| Budi | 18   | Dokumenter Teknis | -               |
| Cici | -    | Ilmuwan Data      | -               |
| Didi | 32   | Ilmuwan Data      | 20.000.000      |
| Efi  | -    | Analis Data       | -               |
| Febi | 28   | Analis Data       | 12.000.000      |


Note: saat usia/pendapatan kosong maka usia/pendapatan mengikuti standar perusahaan.

“Dengan kasus ini, berarti di akhir aku harus mencetak total pengeluaran perusahaan untuk menguji kelancaranku dalam menerapkan OOP dengan Python nih,” gumamku sambil berkutat pada baris-baris kode di code editor.

Tugas:
Simulasikan dengan program yang telah dibuat.
Cetak total pengeluaran yang dimiliki perusahaan untuk menguji fungsionalitas konsep dan teknik polymorphism yang diterapkan.
```sh
# Definisikan class Karyawan sebagai parent class
class Karyawan:
    def __init__(self, nama, usia, pendapatan, insentif_lembur):
        self.nama = nama
        self.usia = usia 
        self.pendapatan = pendapatan
        self.pendapatan_tambahan = 0
        self.insentif_lembur = insentif_lembur
    def lembur(self):
        self.pendapatan_tambahan += self.insentif_lembur
    def tambahan_proyek(self,jumlah_tambahan):
        self.pendapatan_tambahan += jumlah_tambahan
    def total_pendapatan(self):
        return self.pendapatan + self.pendapatan_tambahan 

# Definisikan class TenagaLepas sebagai child class dari class Karyawan 
class TenagaLepas(Karyawan):
    def __init__(self, nama, usia, pendapatan): 
        super().__init__(nama, usia, pendapatan, 0)
    def tambahan_proyek(self, nilai_proyek): 
        self.pendapatan_tambahan += nilai_proyek * 0.01

# Definisikan class AnalisData sebagai child class dari class Karyawan 
class AnalisData(Karyawan):
    def __init__(self, nama, usia = 21, pendapatan = 6500000, 
                 insentif_lembur = 100000):
        super().__init__(nama, usia, pendapatan, insentif_lembur) 

# Definisikan class IlmuwanData sebagai child class dari class Karyawan
class IlmuwanData(Karyawan):
    def __init__(self, nama, usia = 25, pendapatan = 12000000, 
                 insentif_lembur = 150000):
        super().__init__(nama, usia, pendapatan, insentif_lembur) 
    def tambahan_proyek(self, nilai_proyek):
        self.pendapatan_tambahan += 0.1 * nilai_proyek

# Definisikan class PembersihData sebagai child class dari class TenagaLepas
class PembersihData(TenagaLepas):
    def __init__(self, nama, usia, pendapatan = 4000000): 
        super().__init__(nama, usia, pendapatan)

# Definisikan class DokumenterTeknis sebagai child class dari class TenagaLepas
class DokumenterTeknis(TenagaLepas):
    def __init__(self, nama, usia, pendapatan = 2500000): 
        super().__init__(nama, usia, pendapatan)

# Definisikan class Perusahaan 
class Perusahaan:
    def __init__(self, nama, alamat, nomor_telepon): 
        self.nama = nama
        self.alamat = alamat 
        self.nomor_telepon = nomor_telepon
        self.list_karyawan = []
    def aktifkan_karyawan(self, karyawan): 
        self.list_karyawan.append(karyawan)
    def nonaktifkan_karyawan(self, nama_karyawan): 
        karyawan_nonaktif = None
        for karyawan in self.list_karyawan:
            if karyawan.nama == nama_karyawan: 
                karyawan_nonaktif = karyawan 
                break
        if karyawan_nonaktif is not None: 
            self.list_karyawan.remove(karyawan_nonaktif)
    def total_pengeluaran(self): 
        pengeluaran = 0
        for karyawan in self.list_karyawan:
            pengeluaran += karyawan.total_pendapatan()
        return pengeluaran
    def cari_karyawan(self, nama_karyawan): 
        for karyawan in self.list_karyawan:
            if karyawan.nama == nama_karyawan: 
                return karyawan
        return None

# Create object karyawan sesuai dengan tugasnya masing-masing
# seperti yang dinyatakan dalam tabel.
ani = PembersihData('Ani',25)
budi = DokumenterTeknis('Budi',18)
cici = IlmuwanData('Cici')
didi = IlmuwanData('Didi',32,20000000)
efi = AnalisData('Efi')
febi = AnalisData('Febi',28,12000000)

# Create object perusahaan
perusahaan = Perusahaan('ABC','Jl. Jendral Sudirman, Blok 11','(021) 95812XX')

# Aktifkan setiap karyawan yang telah didefinisikan
perusahaan.aktifkan_karyawan(ani)
perusahaan.aktifkan_karyawan(budi)
perusahaan.aktifkan_karyawan(cici)
perusahaan.aktifkan_karyawan(didi)
perusahaan.aktifkan_karyawan(efi)
perusahaan.aktifkan_karyawan(febi)

# Cetak keseluruhan total pengeluaran perusahaan
print(perusahaan.total_pengeluaran())
```
### Hasil Belajarku
Wah senangnya! Aku telah berhasil menyelesaikan rangkaian pelajaran Python for Data Professional Beginner.
Dari materi yang telah aku pelajari dan praktekkan, aku telah mempelajari:

Konsep Object Oriented Programming (OOP) pada Python.
Teknik Class dan Objects, serta Class Behavior pada Python.
Teknik Encapsulation dan Inheritance dalam pemograman OOP dengan Python.
Teknik Polymorphism dan teknik Overloading dalam pemograman OOP pada Python.
Teknik membuat program OOP pada Python untuk kasus bisnis sederhana.
