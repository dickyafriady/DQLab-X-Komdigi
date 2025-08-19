### DQLab x Komdigi
## Python for Data Professional Beginner - Part 2
# _Guide to Learn Python with AI at DQLab_

## Collection Manipulation dengan Python
Memulai dengan Collection Manipulation
Hari pertama aku mempelajari Python bersama Senja, aku masih belum mendapat kesulitan yang berarti. Sebaliknya, aku merasa mendapatkan duniaku. Di sinilah aku dapat menjadi diriku sendiri: mengerjakan yang sejak dulu aku sukai.
Meja sebelahku masih kosong, sepertinya Senja belum datang. Aku membuka laptopku dulu dan segera melanjutkan pembelajaran modul kedua Python. Total modul yang Senja berikan padaku kemarin ada tiga!
Harus kucicil belajar dari sekarang. Aku membuka bab pertama isi modul kedua. Materi mengenai “Collection Manipulation”, “List dan Tuple” hingga “Set Manipulation” langsung menyapaku.
Apa itu Collection Manipulation?
Collections manipulation adalah salah satu teknik yang penting untuk dikuasai setiap programmer. Melalui penguasaan materi collections  manipulation, aku dapat mengolah berbagai tipe data collections dalam Python yang meliputi:

1. list,
2. tuple,
3. set, dan
4. Dictionary.


### Mengakses List dan Tuple – Part 1
Seperti yang telah aku pelajari pada modul Python for Data Professional Beginner - Part 1: Bab “Sequence Type”, aku dapat mengakses elemen pada suatu list ataupun tuple dengan menggunakan indeks atau semacam nomor urut dari list atau tuple tersebut. Indeks pada suatu tipe data list atau tuple dimulai dari angka 0.

### Tugas 1:
Aku mencoba mempraktekkan potongan kode di bawah dengan live code editor:
### Tugas 2:
Untuk menampilkan output Desember dan November, yang aku lakukan adalah mengetikkan syntax sederhana 
```sh
bulan_pembelian = ('Januari', 'Februari', 'Maret', 'April', 'Mei', 'Juni', 'Juli', 'Agustus', 'September', 'Oktober', 'November', 'Desember')
print(bulan_pembelian[0])
print(bulan_pembelian[5])
print(bulan_pembelian[-1])
print(bulan_pembelian[-2])
```
### Mengakses List dan Tuple – Part 2
Cara collections manipulation pertama yang akan aku pelajari adalah memotong (slicing) list/tuple dengan menggunakan rentangan nilai indeks (range of index).

### Tugas 1:
Aku mencoba mempraktekkan potongan kode di bawah dengan live code editor:
### Tugas 2:
Untuk menampilkan output bulan_pembelian Januari, Februari, Maret, April, Mei aku dapat menggunakan syntax di bawah untuk mengambil index 0 - 4.
### Tugas 3:
Untuk menampilkan output September, Oktober, November, Desember. Aku dapat menggunakan syntax di bawah untuk mengambil index 8 - elemen terakhir.
### Tugas 4:
Aku juga dapat memotong suatu list/tuple dengan menggunakan indeks negatif. Sebagai contoh untuk mendapatkan output September, Oktober, November.

```sh
bulan_pembelian = ('Januari', 'Februari', 'Maret', 'April', 'Mei', 'Juni', 'Juli', 'Agustus', 'September', 'Oktober', 'November', 'Desember')
pertengahan_tahun = bulan_pembelian [4:8]
print(pertengahan_tahun)
awal_tahun = bulan_pembelian [:5]
print(awal_tahun)
akhir_tahun = bulan_pembelian [:8]
print(akhir_tahun)
print(bulan_pembelian[-4 : -1])
```

### Penggabungan Dua atau Lebih List atau Tuple
Selain dapat melakukan pemotongan terhadap tipe data list/tuple, aku juga dapat menggabungkan isi dari suatu list (ataupun tuple) dengan list lainnya (atau dengan tuple lainnya) dengan menggunakan operator penambahan (+). 

```sh
list_makanan = ['Gado -gado', 'Ayam Goreng', 'Rendang']
list_minuman = ['Es Teh', 'Es Jeruk', 'Es Campur']
list_menu = list_makanan + list_minuman
print(list_menu)
```

### List Manipulation – Part 1
Untuk memanipulasi tipe data list, aku dapat menggunakan sekumpulan fitur yang telah tersedia dalam bahasa pemrograman Python. Merujuk pada tabel di bawah, aku dapat memahami fitur-fitur untuk melakukan manipulasi data yang terdiri atas append(), clear(), copy(), count() dan extend()
```sh
# Fitur .append()
print(">>> Fitur .append()")
list_makanan = ['Gado-gado', 'Ayam Goreng', 'Rendang']
list_makanan.append('Ketoprak')
print(list_makanan)
# Fitur .clear()
print(">>> Fitur .clear()")
list_makanan = ['Gado-gado', 'Ayam Goreng', 'Rendang']
list_makanan.clear
print(list_makanan)
# Fitur .copy()
print(">>> Fitur .copy()")
list_makanan1 = ['Gado-gado', 'Ayam Goreng', 'Rendang']
list_makanan2 = list_makanan1.copy()
list_makanan3 = list_makanan1
list_makanan2.append('Opor')
list_makanan3.append('Ketoprak')
print(list_makanan1)
print(list_makanan2)
# Fitur .count()
print(">>> Fitur .count()")
list_score = ['Budi', 'Sud', 'Budi', 'Budi', 'Budi', 'Sud', 'Sud']
score_budi = list_score.count ('Budi')
score_sud = list_score.count ('Sud')
print(score_budi) # akan menampilkan output 4
print(score_sud) # akan menampilkan output 3
# Fitur .extend()
print(">>> Fitur .extend()")
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang']
list_minuman = ['Es Teh', 'Es Jeruk', 'Es Campur']
list_menu.extend(list_minuman)
print(list_menu)
```

### List Manipulation – Part 2
Selanjutnya aku akan mempelajari fitur index(), insert(), pop(), remove(), reverse(), dan sort() untuk melakukan manipulasi.

```sh
# Fitur .index()
print(">>> Fitur .index()")
list_score = ['Budi','Sud','Budi','Budi','Budi','Sud','Sud']
score_pertama_sud = list_score.index('Sud') + 1
print(score_pertama_sud) # akan menampilkan output 2
# Fitur .insert()
print(">>> Fitur .insert()")
list_score = ['Budi','Sud','Budi','Budi','Sud']
list_score.insert(3, 'Sud')
print(list_score)
# Fitur .pop()
print(">>> Fitur .pop()")
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang']
list_menu.pop(1)
print(list_menu)
# Fitur .remove()
print(">>> Fitur .remove()")
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']
list_menu.remove('Rendang')
print(list_menu)
# Fitur .reverse()
print(">>> Fitur .reverse()")
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']
list_menu.reverse()
print(list_menu)
# Fitur .sort()
print(">>> Fitur .sort()")
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']
list_menu.sort() # Default: Ascending
print(list_menu) 
list_menu.sort(reverse = True )# Descending
print(list_menu) 
```
## Tuple Manipulation
Aku juga mempelajari fitur yang dapat digunakan untuk melakukan manipulasi data dengan tipe data tuple. 
```sh
# Fitur .count()
print(">>> Fitur .count()")
tuple_score = ('Budi', 'Sud', 'Budi', 'Budi', 'Budi', 'Sud', 'Sud')
score_budi = tuple_score.count('Budi')
score_sud = tuple_score.count('Sud')
print(score_budi) # akan menampilkan output 4
print(score_sud) # akan menampilkan output 3
# Fitur .index()
print(">>> Fitur .index()")
tuple_score = ('Budi','Sud','Budi','Budi','Budi','Sud','Sud')
score_pertama_sud = tuple_score.index('Sud')+1
print(score_pertama_sud) # akan menampilkan output 2
```
### Set Manipulation – Part 1
Sedikit berbeda dengan tipe data list dan tuple, pada tipe data set terdapat cukup banyak fitur yang disediakan oleh bahasa Python
```sh
# Fitur .add()
print(">>> Fitur .add()")
set_buah = {'Jeruk','Apel','Anggur'}
set_buah.add('Melon')
print(set_buah)
# Fitur .clear()
print(">>> Fitur .clear()")
set_buah = {'Jeruk','Apel','Anggur'}
set_buah.clear()
print(set_buah)
# Fitur .copy()
print(">>> Fitur .copy()")
set_buah1 = {'Jeruk','Apel','Anggur'}
set_buah2 = set_buah1
set_buah3 = set_buah1.copy()
set_buah2.add('Melon')
set_buah3.add('Kiwi')
print(set_buah1)
print(set_buah2)
# Fitur .update()
print(">>> Fitur .update()")
parcel1 = {'Anggur','Apel','Jeruk'}
parcel2 = {'Apel','Kiwi','Melon'}
parcel1.update(parcel2)
print(parcel1)
# Fitur .pop()
print(">>> Fitur .pop()")
parcel = {'Anggur','Apel','Jeruk'}
buah = parcel.pop()
print(buah)
print(parcel)
# Fitur .remove()
print(">>> Fitur .remove()")
parcel = {'Anggur','Apel','Jeruk'}
parcel.remove('Apel')
print(parcel)
```

### Set Manipulation – Part 2
Sedikit berbeda dengan tipe data list dan tuple, pada tipe data set terdapat cukup banyak fitur manipulasi yang bisa aku gunakan.

```sh
# Fitur .union()
print(">>> Fitur .union()")
parcel1 = {'Anggur','Apel','Jeruk'}
parcel2 = {'Apel','Kiwi','Melon'}
parcel3 = parcel1.union(parcel2)
print(parcel1)
print(parcel3)
# Fitur .isdisjoint()
print(">>> Fitur .isdisjoint()")
parcel1 = {'Anggur','Apel','Jeruk'}
parcel2 = {'Kiwi','Melon','Pisang'}
parcel3 = {'Apel','Srikaya','Semangka'}
parcel1_parcel2_disjoint = parcel1.isdisjoint(parcel2)
print(parcel1_parcel2_disjoint)
parcel1_parcel3_disjoint = parcel1.isdisjoint(parcel3)
print(parcel1_parcel3_disjoint)
# Fitur .issubset()
print(">>> Fitur .issubset()")
parcel_A = {'Anggur', 'Apel'}
parcel_B = {'Durian','Semangka','Apel'}
parcel_C = {'Anggur', 'Kiwi', 'Apel', 'Jeruk', 'Melon'}
parcel_A_dalam_C = parcel_A.issubset(parcel_C)
parcel_B_dalam_C = parcel_B.issubset(parcel_C)
print(parcel_A_dalam_C)
print(parcel_B_dalam_C)
# Fitur .issuperset()
print(">>> Fitur .issuperset()")
parcel_C_mengandung_A = parcel_C.issuperset(parcel_A)
parcel_C_mengandung_B = parcel_C.issuperset(parcel_B)
print(parcel_C_mengandung_A)
print(parcel_C_mengandung_B)
# Fitur .intersection()
print(">>> Fitur .intersection()")
parcel_A = {'Anggur', 'Kiwi', 'Apel', 'Jeruk', 'Melon'}
parcel_B = {'Apel', 'Jeruk', 'Semangka', 'Durian', 'Tomat'}
parcel_C = parcel_A.intersection(parcel_B)
print(parcel_C)
# Fitur .difference()
print(">>> Fitur .difference()")
parcel_C = parcel_A.difference(parcel_B)
print(parcel_C)
# Fitur .symmetric_difference()
print(">>> Fitur .symmetric_difference()")
parcel_A = {'Anggur', 'Apel', 'Jeruk', 'Melon'}
parcel_B = {'Apel','Jeruk','Semangka','Leci'}
parcel_C = parcel_A.symmetric_difference(parcel_B)
print(parcel_C)
```
### Dictionary Manipulation
Aku baru saja selesai mengerjakan beberapa kuis latihan ketika Senja mengejutkanku dengan tepukannya di belakang pundakku.
“Lagi apa kamu, Aksara?”
“Ngagetin aja, Nja.”
“Soalnya serius banget. Padahal saya belum kasih intruksi apa-apa buat lanjut hari ini.”
“Hehehe, iya biar cepet selesai dan bisa praktik lagi,” kataku sembari mengacungkan jari telunjuk dan tengah membentuk ‘peace’.
“Kita bakal banyak praktik kok. Sekarang sudah belajar sampai mana?”
Aku menunjukkan subjudul yang sedang kupelajari saat ini: “Dictionary Manipulation” pada Senja.“Oke, pas banget. Bab ini ada praktiknya, nanti kupandu ya. Bagian string manipulation juga.”
Sembari menunggu Senja membuka laptopnya, aku kembali melanjutkan membaca:
Terakhir, untuk memanipulasi tipe data dictionary.
```sh
# Fitur .clear()
print(">>> Fitur .clear()")
info_karyawan = {'nama' : 'Aksara',
                 'nik' : '1211011',
                 'pekerjaan' : 'Data Analyst'}
info_karyawan.clear()
print(info_karyawan)
# Fitur .copy()
print(">>> Fitur .copy()")
info_karyawan1 = {'nama' : 'Aksara',
                  'nik' : '1211011',
                  'pekerjaan' : 'Data Analyst'}
info_karyawan2 = info_karyawan1.copy()
info_karyawan2['nama'] = 'Senja'
info_karyawan2['nik'] = '1211056'
print(info_karyawan1)
print(info_karyawan2)
# Fitur .keys()
print(">>> Fitur .keys()")
info_karyawan = {'nama' : 'Aksara',
                 'nik' : '1211011',
                 'pekerjaan' : 'Data Analyst'}
kunci_akses = list(info_karyawan.keys())
print(kunci_akses)
# Fitur .values()
print(">>> Fitur .values()")
value_dict = list(info_karyawan.values())
print(value_dict)
# Fitur .update()
print(">>> Fitur .update()")
info_karyawan.update({'skillset':['Python', 'R']})
print(info_karyawan)
```

### Useful Tips and Tricks
Untuk menentukan berapa jumlah data yang tersimpan di setiap elemen pada tuple/list, aku dapat menggunakan fungsi buit-in len(). 
```sh
# Tuple
print(">>> Tuple")
tuple_menu = ('Gado-gado','Ayam Goreng','Rendang','Ketoprak')
jumlah_menu = len(tuple_menu)
print(jumlah_menu)
# List
print(">>> List")
list_menu = ['Gado-gado','Ayam Goreng','Rendang','Ketoprak']
jumlah_menu = len(list_menu)
print(jumlah_menu)
# Konversi tipe data
print(">>> Konversi tipe data")
list_buah = ['Apel', 'Apel', 'Jeruk', 'Markisa', 'Jeruk', 'Markisa', 'Apel']
set_buah = set(list_buah)
print(set_buah)
list_buah = list(set_buah)
list_buah.sort()
print(list_buah)
```

### Tugas Praktek 
Tugas Praktek
“Aksara, untuk praktik kali ini, saya membebaskan kamu memilih case yang akan digunakan,” ujar Senja padaku.

Aku pun mulai berpikir. Selama ini aku bikin program hitung-menghitung untuk kantor dan keluarga, kok enggak bikin buat diri sendiri juga yah? Apalagi belakangan aku suka nge-boba, kayaknya memang harus dilacak deh pengeluaran dan pemasukanku minimal 9 bulan terakhir. Kalau begitu, aku pakai case pengalamanku sendiri ini saja untuk dianalisis!

Buat menganalisisnya, berarti aku harus merapikan struktur data yang kumiliki terlebih dulu dengan dictionary dan kuberi nama keuangan untuk merepresentasikan pengeluaran dan pemasukan. “Pakai format juta, lalu masukkan variabel keuangan,” ujarku sembari mengetik
### Tugas:
Dari variabel keuangan, aku akan menghitung rata-rata pengeluaran dan pemasukanku selama 9 bulan terakhir. Semoga keuanganku sehat-sehat saja. 

```sh
# Data keuangan
keuangan = {
'pengeluaran': [2, 2.5, 2.25, 2.5, 3.2, 2.5, 3.5, 4, 3],
'pemasukan': [7.8, 7.5, 9, 7.6, 7.2, 7.5, 7, 10, 7.5]
}
# Perhitungan rata-rata pemasukan dan rata-rata pengeluaran
total_pengeluaran = 0
total_pemasukan = 0
for biaya in keuangan['pengeluaran']: 
    total_pengeluaran += biaya
for biaya in keuangan['pemasukan']: 
    total_pemasukan += biaya
rata_rata_pengeluaran = total_pengeluaran/len(keuangan['pengeluaran'])
rata_rata_pemasukan = total_pemasukan/len(keuangan['pemasukan']) 
print(rata_rata_pengeluaran) 
print(rata_rata_pemasukan)
```

### String Manipulation dengan Python
### Apa itu String Manipulation?
Aku belajar bahwa String Manipulation adalah teknik yang digunakan dalam memanipulasi data yang disimpan dalam tipe data str. Pada bahasa Python, untuk mempermudah proses pengolahan data, tipe data string dapat diperlakukan layaknya seperti tipe data list.

### Tugas:
Aku mengikuti contoh yang diberikan dengan mengetik syntax pada live code editor untuk memahami bagaimana String Manipulation bekerja pada Python.

```sh
nama_produk = "Sepatu Niko"
nama_produk = nama_produk[:2] + "P" + nama_produk[3:9] + "K" +nama_produk[-1]
print(nama_produk)
print(nama_produk[:7])
print(nama_produk[7:])
print(len(nama_produk))
```

### Operator “+” untuk Tipe Data String
Setelah aku mempelajari String Manipulation, sekarang aku beralih ke Operator +. Operator + pada dua string akan secara otomatis menggabungkan kedua string tersebut. Operator + juga dapat digunakan untuk menambahkan beberapa string secara bersamaan.
Aku mengikuti contoh yang diberikan dengan mengetik syntax pada live code editor untuk memahami bagaimana Operation + bekerja pada Python.

```sh
nama_depan = 'Jhon'
nama_belakang = 'Doee'
nama_lengkap = nama_depan + ' ' + nama_belakang
print(nama_lengkap)
umur = '27 tahun'
alamat = 'Jl. Anggrek No. 100'
nama_umur_alamat = 'Hi, saya ' + nama_lengkap + ' umur ' + umur + ', tinggal di ' + alamat + '.'
print(nama_umur_alamat)
```
### Menghilangkan Spasi di Awal dan/atau di Akhir
Sekarang aku akan mempelajari bagaimana menghilangkan kelebihan spasi yang dimiliki di awal dan/atau di akhir variabel string. Pertama, aku melihat fitur yang diberikan pada tabel contoh.

```sh
# Fitur .strip()
print(">>> Fitur .strip()")
kata_sambutan = ' halo, selamat siang! '
kata_sambutan = kata_sambutan.strip()
print(kata_sambutan)
# Fitur .lstrip()
print(">>> Fitur .lstrip()")
kata_sambutan = ' halo, selamat siang! '
kata_sambutan = kata_sambutan.lstrip()
print(kata_sambutan)
# Fitur .rstrip()
print(">>> Fitur .rstrip()")
kata_sambutan = ' halo, selamat siang! '
kata_sambutan = kata_sambutan.rstrip()
print(kata_sambutan)
```

### Merubah Caps pada String
Pada bagian ini, aku akan mempelajari cara merubah caps (penggunaan huruf besar dan kecil). Jika diawal kalimat pada suatu string yang dimiliki belum berupa huruf kapital, maka dengan menggunakan fitur .capitalize() kita dengan mudah mengubah string tersebut menjadi kalimat yang benar secara bahasa.

Tugas:
Aku mengikuti contoh yang diberikan dengan mengetik syntax pada live code editor untuk memahami bagaimana fitur .capitalize(), .lower(), dan .upper() bekerja pada Python.  

```sh
# Fitur .capitalize()
print(">>> Fitur .capitalize()")
judul_buku = 'belajar bahasa Python'
print(judul_buku.capitalize())
# Fitur .lower()
print(">>> Fitur .lower()")
judul_buku = 'Belajar Bahasa PYTHON.'
print(judul_buku.lower())
# Fitur .upper()
print(">>> Fitur .upper()")
judul_buku = 'Belajar Bahasa PYTHON.'
print(judul_buku.upper())
```

### Pemecahan, Penggabungan, dan Penggantian String
Pada bagian ini, aku akan mempelajari bagaimana cara memecah suatu string dengan kondisi tertentu sehingga menghasilkan list of string. Kemudian, akan dipelajari bagaimana cara menggabungkan beberapa list of string menjadi string saja. Akhirnya, aku akan mengganti sub-string tertentu dengan sub-string lainnya sehingga mengubah string awalnya.

### Tugas:
Agar lebih memahami bagaimana penerapannya pada Python, aku akan mengikuti contoh penggunaan yang diberikan dari tabel berikut dengan mengetik syntax pada live code editor.

```sh
# Fitur .split()
print(">>> Fitur .split()")
frasa = "ani dan budi dan wati dan johan"
karakter = frasa.split("dan")
print(karakter)
kata = frasa.split(" ")
print(kata)
# Fitur .join()
print(">>> Fitur .join()")
pemisah = " dan "
karakter = ["Ricky", "Peter", "Jordan"]
frasa = pemisah.join(karakter)
print(frasa)
frasa = " ".join(karakter)
print(frasa)
# Fitur .replace()
print(">>> Fitur .replace()")
frasa = "apel malang apel yang paling segar, apel sehat, apel nikmat"
frasa = frasa.replace("apel", "jeruk")
print(frasa)
```

### Menentukan Posisi dan Jumlah Sub-string pada String
Pada bagian ini, aku akan mempelajari bagaimana cara menentukan posisi awal suatu sub-string dan jumlah kemunculan sub-string tersebut pada suatu string agar lebih memahami bagaimana penerapannya pada Python.
### Tugas:
Aku akan mengikuti contoh penggunaan yang diberikan dari tabel berikut dengan mengetiknya pada live code editor.

```sh
teks = "Apel malang adalah apel termanis dibanding apel-apel lainnya"
# Fitur .find()
print(">>> Fitur .find()")
print(teks.find("Apel"))
print(teks.find("Malang"))
# Fitur .count()
print(">>> Fitur .count()")
kemunculan_kata_apel = teks.count("apel")
print(kemunculan_kata_apel)
```

### Menentukan String Apakah Diawali/Diakhiri oleh Sub-string
Pada bagian ini, aku akan mempelajari bagaimana menentukan apakah suatu string diawali atau diakhiri dengan suatu substring (teks) tertentu.
### Tugas:
Agar lebih memahami bagaimana penerapannya pada Python, aku akan mengikuti contoh penggunaan yang diberikan menggunakan fitur dalam tabel berikut dengan mengetiknya pada live code editor.
```sh
# Fitur .startswith()
print(">>> Fitur .startswith()")
teks = "Apel malang adalah apel termanis dibanding apel-apel lainnya"
print(teks.startswith("Apel"))
print(teks.startswith("apel"))
# Fitur .endswith()
print(">>> Fitur .endswith()")
print(teks.endswith("lainnya"))
print(teks.endswith("apel"))
```

### Tugas Praktek
Tugas Praktek
Aku mengecek ponsel. Sejak kukirimkan progress latihanku terakhir pada Senja, belum ada kabar lagi sampai saat ini. Senja memang tiba-tiba pergi dari mejanya tadi. Sedikit bosan, aku coba membuka-buka dokumen di laptop. Aku menemukan folder “LATIHAN” dan teringat kalau ada satu latihan kecil yang belum kukerjakan. “Mumpung lagi lowong, aku coba deh.”

Aku mengeklik dokumen PENGOLAHAN DATA TEKS. Di dalamnya aku diminta untuk meneliti popularitas antara buah salak dan buah jeruk berdasarkan judul artikel yang muncul di majalah Buah Sehat. Aku mulai menyiapkan susunan kodeku: 
```sh
judul_artikel = [
"Buah Salak Baik untuk Mata", "Buah Salak Kaya Potasium", 
"Buah Jeruk Kaya Vitamin C", "Buah Salak Kaya Manfaat", 
"Salak Baik untuk Jantung", "Jeruk dapat Memperkuat Tulang", 
"Jeruk Mencegah Penyakit Asma", "Jeruk Memperkuat Gigi", 
"Jeruk Mencegah Kolesterol Jahat", "Salak Mencegah Diabetes", 
"Salak Memperkuat Dinding Usus", "Salak Baik untuk Darah",
"Jeruk Kaya Manfaat untuk Jantung", "Salak si Kecil yang Baik", 
"Jeruk dan Salak Buah Kaya Manfaat", "Buah Jeruk Enak",
"Tips Panen Jeruk Ribuan Kilo", "Tips Bertanam Salak", 
"Salak Manis untuk Berbuka", "Jeruk Baik untuk Wajah"
]
 ```
Tugas:
“Kalau mengikuti yang sudah kupelajari, langkah pertama adalah menghitung jumlah kemunculan kata jeruk dan salak di tiap judul artikel,” batinku.

Aku kembali berkutat di depan layar laptop.
```sh
judul_artikel = [
"Buah Salak Baik untuk Mata", "Buah Salak Kaya Potasium", 
"Buah Jeruk Kaya Vitamin C", "Buah Salak Kaya Manfaat", 
"Salak Baik untuk Jantung", "Jeruk dapat Memperkuat Tulang", 
"Jeruk Mencegah Penyakit Asma", "Jeruk Memperkuat Gigi", 
"Jeruk Mencegah Kolesterol Jahat", "Salak Mencegah Diabetes", 
"Salak Memperkuat Dinding Usus", "Salak Baik untuk Darah",
"Jeruk Kaya Manfaat untuk Jantung", "Salak si Kecil yang Baik", 
"Jeruk dan Salak Buah Kaya Manfaat", "Buah Jeruk Enak",
"Tips Panen Jeruk Ribuan Kilo", "Tips Bertanam Salak", 
"Salak Manis untuk Berbuka", "Jeruk Baik untuk Wajah"
]
jumlah_artikel_jeruk = 0
jumlah_artikel_salak = 0
for judul in judul_artikel:
    if judul.count('jeruk') > 0: 
        jumlah_artikel_jeruk += 1
    if judul.count('salak') > 0:
        jumlah_artikel_salak += 1
print(jumlah_artikel_jeruk) 
print(jumlah_artikel_salak)
```

### Tugas Praktek
Setelah selesai menghitung jumlah kemunculan kata, aku mencoba berpikir dari sudut pandang si pemilik majalah. Kalau aku jadi mereka, tentunya aku juga ingin tahu apakah kata yang muncul itu bermuatan positif atau tidak. Nah ini!

### Tugas:
Dengan cepat, aku mendeklarasikan daftar bernama kata_positif yang berisi nuansa kata positif untuk menghitung jumlah kemunculan kata_positif bagi tiap artikel jeruk dan salak, seperti ini:
```sh
judul_artikel = [
"Buah Salak Baik untuk Mata", "Buah Salak Kaya Potasium", 
"Buah Jeruk Kaya Vitamin C", "Buah Salak Kaya Manfaat", 
"Salak Baik untuk Jantung", "Jeruk dapat Memperkuat Tulang", 
"Jeruk Mencegah Penyakit Asma", "Jeruk Memperkuat Gigi", 
"Jeruk Mencegah Kolesterol Jahat", "Salak Mencegah Diabetes", 
"Salak Memperkuat Dinding Usus", "Salak Baik untuk Darah",
"Jeruk Kaya Manfaat untuk Jantung", "Salak si Kecil yang Baik", 
"Jeruk dan Salak Buah Kaya Manfaat", "Buah Jeruk Enak",
"Tips Panen Jeruk Ribuan Kilo", "Tips Bertanam Salak", 
"Salak Manis untuk Berbuka", "Jeruk Baik untuk Wajah"
]
kata_positif = ["Kaya", "Baik", "Mencegah", "Memperkuat"]
kata_positif_jeruk = 0
kata_positif_salak = 0
for judul in judul_artikel: 
    for kata in kata_positif:
        if judul.count("Jeruk") > 0 and judul.count("kata") > 0: 
            kata_positif_jeruk += 1
        if judul.count("Salak") > 0 and judul.count("kata") > 0:
            kata_positif_salak += 1
print(kata_positif_jeruk) 
print(kata_positif_salak)
```

### Apa itu Functions?
Function adalah sebuah blok statemen yang hanya akan dijalankan saat ia dipanggil. Secara tidak sadar, selama proses belajar ini, aku telah mencoba menggunakan fungsi-fungsi dalam bahasa pemrograman Python.

Fungsi len() untuk mengukur jumlah elemen dalam sebuah list dan fungsi print() untuk menampilkan pesan pada layar konsol merupakan contoh dari bentuk fungsi yang telah disediakan oleh bahasa pemrograman Python, atau dengan kata lain built-in functions.

Selain fungsi yang telah disediakan oleh Python, Python mengizinkan aku untuk mendeklarasikan fungsi dalam kode yang aku tuliskan yang dikenal dengan user defined function.
```sh
def nama_fungsi(argument):
    statement_1
    …
    statement_n
    return returned_value
```
Aku menuliskan dalam catatanku:

nama_fungsi adalah nama untuk fungsi yang kita definisikan, memiliki aturan seperti penamaan variabel
argument adalah variabel masukan ke fungsi, bisa tanpa variabel, satu variabel atau lebih
statement_1 … statement_n adalah algoritma yang telah kita transfer dalam bahasa Python. Ini merupakan inti dari fungsi yang kita definisikan. Seluruh statement adalah menjorok (indent) ke dalam seperti yang pernah dipelajari pada conditioning dan looping
return_value adalah variabel output dari fungsi kita. Bisa tanpa variabel, satu variabel, atau lebih.




### Fungsi Pertama
contoh_fungsi merupakan nama dari fungsi yang aku deklarasikan dan statemen-statemen di dalamnya disebut sebagai isi (body) dari fungsi.

Tugas:
Untuk menjalankan fungsi yang telah aku deklarasikan, aku dapat menuliskan potongan kode berikut dengan mengetiknya pada live code editor pada baris berikutnya.


```sh
# Definisikan fungsi
def contoh_fungsi():
    print("Halo Dunia")
    print("Aku sedang belajar bahasa Python")
# Panggil fungsi yang telah didefinisikan
contoh_fungsi()
```

### Fungsi Kedua
Sebuah fungsi dapat menerima serangkaian argumen pada bagian dalam kurung setelah nama fungsi telah aku definisikan.
fungsi_dengan_argumen membutuhkan dua argumen (nama_depan, nama_belakang).
Python akan menjalankan sebuah fungsi hanya ketika aku telah mensuplai jumlah argumen yang sesuai saat fungsi didefinisikan
```sh
# Definsikan fungsi 
def fungsi_dengan_argumen(nama_depan, nama_belakang):
    print(nama_depan+" "+nama_belakang)
# Panggil fungsi dengan memasukkan argumen
# nama_depan yaitu "John" dan nama_belakang "Doe"
fungsi_dengan_argumen("Jhon", "Doe")
```
### Fungsi Ketiga
Saat aku melakukan pemanggilan fungsi dengan jumlah argumen yang tidak sesuai, Python akan mengembalikan pesan error yang menyatakan bahwa terdapat argumen yang belum disuplai agar fungsi dapat dijalankan dengan baik.

Berikut ini adalah contoh pesan error yang akan dikembalikan oleh Python saat aku hanya menyuplai satu argumen saja untuk fungsi_dengan_argumen:
```sh
Type Error: function fungsi_dengan_argumen() missing 1 required positional argument: nama_belakang
 ```
Bahasa Python mengizinkan aku untuk memberikan suatu nilai default terkait dengan sebuah argumen dalam sebuah fungsi. Melalui fitur ini, suatu argumen dalam sebuah fungsi akan bersifat opsional.
```sh
# Definsikan fungsi dengan nilai default argument kedua adalah "".
def fungsi_dengan_argumen(nama_depan, nama_belakang = ""):
	print(nama_depan+" "+nama_belakang)
# Panggil fungsi dengan memasukkan argumen nama_depan "John"
fungsi_dengan_argumen("Jhon")
# Panggil fungsi dengan memasukkan argumen
# nama_depan yaitu "John" dan nama_belakang "Doe"
fungsi_dengan_argumen("John", "Doe")
```

### Tugas Praktek
Tepat ketika aku baru menyelesaikan latihan tadi, aku mendapat pesan masuk di email. Dari Senja.
Tugas: 
Aksara, pekerjaan terakhirmu baru bisa saya review sore nanti. Saat ini, kita sedang butuh bantuanmu untuk menentukan nilai rata-rata untuk data yang sudah saya buatkan dalam bentuk list of numeric bertipe int/float berikut ini. Tolong kirimkan hasilnya sebelum jam 3 siang. Terima kasih.
data1 = [70, 70, 70, 100, 100, 100, 120, 120, 150, 150]
dan
data2 = [50, 60, 60, 50, 70, 70, 100, 80, 100, 90]

Aku pun melirik jam dinding kantor. Masih ada satu setengah jam sebelum deadline. Harus segera dikebut!

```sh
# Dua buah data yang tersimpan dalam tipe list
data1 = [70, 70, 70, 100, 100, 100, 120, 120, 150, 150]
data2 = [50, 60, 60, 50, 70, 70, 100, 80, 100, 90]
# Definisikan fungsi hitng_rata_rata
def hitung_rata_rata(data):
    jumlah = 0
    for item in data:
        jumlah += item
    rata_rata = jumlah/len(data)
    return rata_rata
# Hitung nilai rata-rata dari kedua data yang dimiliki
print('Rata-rata data1:')
print(hitung_rata_rata(data1))
print('Rata-rata data2:')
print(hitung_rata_rata(data2))
```

### Tugas Praktek
Sudah setengah jam sejak kukirimkan hasil susunan kodeku pada Senja, ia segera membalas pesanku. Untungnya bukan revisi! Aku lebih suka dapat tambahan pekerjaan dibanding merevisi pekerjaan lama.
### Tugas:
Aksara, yang kamu buat sudah cukup. Tolong buat satu fungsi untuk menghitung standar deviasi data dari data yang sudah saya berikan tadi (data dalam list of numeric bertipe int atau float).
data1 = [70, 70, 70, 100, 100, 100, 120, 120, 150, 150]
dan
data2 = [50, 60, 60, 50, 70, 70, 100, 80, 100, 90]

σ = sqrt( (1/N) * Σ (xi - x̄)² )

```sh
# Dua buah data yang tersimpan dalam tipe list
data1 = [70, 70, 70, 100, 100, 100, 120, 120, 150, 150]
data2 = [50, 60, 60, 50, 70, 70, 100, 80, 100, 90]
# Fungsi rata-rata data
def hitung_rata_rata(data):
    jumlah = 0
    for item in data:
        jumlah += item
    rata_rata = jumlah/len(data)
    return rata_rata
# Definisikan fungsi hitung_standar_deviasi
def hitung_standar_deviasi(data):
    rata_rata_data = hitung_rata_rata(data)
    varians = 0
    for item in data:
        varians += (item - rata_rata_data)**2
    varians /= len(data)
    standar_deviasi = varians ** (1/2)
    return standar_deviasi
# Hitung nilai standar deviasi dari kedua data yang dimiliki
print('Standar deviasi data1:')
print(hitung_standar_deviasi(data1))
print('Standar deviasi data2:')
print(hitung_standar_deviasi(data2))
```

### Tugas Praktek
“Aksara, hasil kerjamu dapat pujian di rapat tadi. Terima kasih ya sudah membantu!” ujar Senja yang menghampiri mejaku setelah keluar dari ruang rapat.

Aku mengangguk. Mungkin program tadi sederhana saja, tapi bisa bermanfaat bagi yang membutuhkannya sangat membahagiakan buatku.

“Oh ya, Aksara sebelum kamu pulang bisa tolong buatkan fungsi baru lagi? Kali ini untuk menentukan nilai-rata dan standar deviasi dari data di tabel. Nanti aku kasih data di tabelnya ya.” Senja langsung menarik bangku ke sebelahku dan membuka laptop.
| Luas Tanah (m²) | Luas Bangunan (m²) | Jarak ke Pusat Kota (km) | Harga (×100 Juta Rp) |
| --------------- | ------------------ | ------------------------ | -------------------- |
| 70              | 50                 | 15                       | 500                  |
| 70              | 60                 | 30                       | 400                  |
| 70              | 60                 | 55                       | 300                  |
| 100             | 50                 | 30                       | 700                  |
| 100             | 70                 | 25                       | 1000                 |
| 100             | 70                 | 50                       | 650                  |
| 120             | 100                | 20                       | 2000                 |
| 120             | 80                 | 50                       | 1200                 |
| 150             | 100                | 50                       | 1800                 |
| 150             | 90                 | 15                       | 3000                 |


### Tugas:
Dari data ini, berarti aku harus menjalankan fungsi baru dengan nama variabel deksripsi_properti. Aku pun mengangkat jempol pada Senja seakan bilang, "Serahkan padaku!"

Setelah kupelajari kembali, data ini sebenarnya telah direpresentasikan ke dalam dict dengan nama tabel_properti. Kalau begitu, aku bisa mulai kodeku seperti berikut ini.

```sh
# Data properti
tabel_properti = {
'luas_tanah': [70, 70, 70, 100, 100, 100, 120, 120, 150, 150],
'luas_bangunan': [50, 60, 60, 50, 70, 70, 100, 80, 100, 90],
'jarak': [15, 30, 55, 30, 25, 50, 20, 50, 50, 15],
'harga': [500, 400, 300, 700, 1000, 650, 2000, 1200, 1800, 3000]
}
# Fungsi rata-rata data
def hitung_rata_rata(data):
    jumlah = 0
    for item in data:
        jumlah += item
    rata_rata = jumlah/len(data)
    return rata_rata
# Fungsi hitung_standar_deviasi
def hitung_standar_deviasi(data):
    rata_rata_data = hitung_rata_rata(data)
    varians = 0
    for item in data:
        varians += (item - rata_rata_data) ** 2
        varians /= len(data)
    standar_deviasi = varians ** (1/2)
    return standar_deviasi
# Definisikan fungsi untuk menghitung rata-rata dan standar deviasi
# setiap kolom pada tabel_properti yang diberikan oleh key dict.
def deskripsi_properti(tabel):
    for key in tabel.keys():
        print('Rata-rata ' + key + ':')
        print(hitung_rata_rata(tabel[key])) 
        print('Standar deviasi ' + key + ':')
        print(hitung_standar_deviasi(tabel[key]))
        print('')
# Panggil fungsi deskripsi_properti untuk menghitung rata-rata 
# dan standar deviasi setiap kolom pada tabel_properti
deskripsi_properti(tabel_properti)

```

### Manipulasi Berkas Teks dan Library Matematika pada Python
### Manipulasi Berkas Teks

1. Membaca file di local computer
Pengolahan berkas teks pada Python tidak membutuhkan proses import dependencies lainnya seperti pada bahasa-bahasa pemrograman lainnya. Untuk memanipulasi berkas teks pada bahasa pemrograman Python, mula-mula aku harus membuka/membuat berkas teks yang aku inginkan dengan menggunakan fungsi open(). Fungsi open() menerima 2 parameter, di mana parameter pertama merupakan nama dari file yang ingin dibuka/dibuat dan mode yang berkaitan dengan aksi yang ingin dilakukan terhadap file yang telah terbuka. Sebagai contoh:

file = open("hello.txt", "r")
Argumen/parameter "r" mengartikan bahwa file yang akan dibuka berada dalam mode “read” sehingga nantinya aku tidak dapat menambahkan/ menuliskan ulang isi tulisan dari file "hello.txt".

Perintah ini dapat digunakan untuk menutup file yang telah aku buka.

file.close()
 

Aku juga belajar bahwa selain mode "r" yang hanya digunakan untuk membaca file, terdapat juga mode lainnya seperti:

w: write, mode ini dapat aku gunakan untuk menulis ke dalam sebuah berkas teks. Jika berkas tidak tersedia, maka Python akan secara otomatis membuat sebuah berkas baru dengan nama yang telah di spesifikasikan. Saat menulis dengan menggunakan mode ini, jika file semula tidak kosong, maka isi yang sebelumnya terdapat di dalam berkas akan terhapus.
a: append, mode ini dapat aku gunakan untuk menambahkan isi dari sebuah berkas teks. Mode ini juga akan membuat sebuah berkas teks baru dengan nama yang telah kita spesifikasikan jika berkas teks tidak tersedia.
w+: write+, mode ini dapat aku gunakan untuk membaca ataupun menuliskan isi dari sebuah berkas teks.
a+: append+, mode ini dapat aku gunakan untuk membaca ataupun menambahkan isi dari sebuah berkas teks.
 

2. Membaca file dari url
Berkas teks yang berada di suatu alamat di internet dapat dibaca berdasarkan url-nya. Untuk membacanya aku perlu menggunakan library requests. File hello.txt yang aku temui di local komputer ku juga ada di url berikut https://storage.googleapis.com/dqlab-dataset/hello.txt. 

Akhirnya, aku dapat menggunakan kode berikut

import requests
url = "https://storage.googleapis.com/dqlab-dataset/hello.txt"
response = requests.get(url)
Cukup ringkas juga ya, gumamku.

### Membaca Berkas Teks – Part 1
Setelah mempelajari bagaimana membuka/membuat sebuah berkas teks dalam Python, aku akan mempelajari sintaks untuk dapat membaca isi dari sebuah berkas. Untuk membaca isi dari sebuah teks aku dapat menggunakan potongan kode berikut.
Aku akan mengasumsikan baris-baris di bawah comment merupakan isi dari “hello.txt”.
Kita sedang belajar Python
Tepatnya belajar memanipulasi berkas teks
Memanipulasi berkas dengan Python sangatlah mudah!
Note: Karena ada perubahan hosting file hello.txt yang tidak ditempatkan di direktori lokal sistem DQLab kamu dapat mempraktikkan bagian A1 dan A2 pada komputer kamu. Untuk itu file hello.txt dapat kamu unduh melalui https://storage.googleapis.com/dqlab-dataset/hello.txt. 

### Tugas Praktik:
Well, aku sudah mempraktikkan membaca berkas teks secara lokal di komputer ku. Sekarang aku akan mencoba membaca berkas teks yang sama yang berada di url https://storage.googleapis.com/dqlab-dataset/hello.txt. Di code editor akupun mengetikkan perintah berikut
```sh
import requests
url = "https://storage.googleapis.com/dqlab-dataset/hello.txt"
response = requests.get(url)
# Cetak kode status dari response
print(response)
# Cetak isi file hello.txt menggunakan method response.iter_lines()
print("\n>> Cetak isi file hello.txt menggunakan method response.iter_lines():")
for baris in response.iter_lines():
	print(baris)
```

### Membaca Berkas Teks – Part 2
### Tugas Praktik:
Aku menjadi penasaran dengan hasil yang telah aku dapatkan sebelumnya. Apakah ada method/attribut lain gak ya untuk mencetak isi dari berkas hello.txt di https://storage.googleapis.com/dqlab-dataset/hello.txt.

Akupun mencoba mengunakan atribut .text dari variabel response, seperti yang ditampilkan pada baris kedelapan.

```sh
import requests
url = "https://storage.googleapis.com/dqlab-dataset/hello.txt"
response = requests.get(url)
# Cetak kode status dari response
print(response)
# Cetak isi file hello.txt menggunakan atribut response.text
print("\n>> Cetak isi file hello.txt menggunakan atribut response.text:")
print(response.text)
```

### Menulis Berkas Teks – Part 1
Untuk menuliskan isi dari suatu berkas, aku dapat menggunakan fungsi write() atau writelines() yang telah disediakan oleh Python. Sebelum masuk ke dalam contoh penggunaan fungsi write() atau writelines(), penting bagiku untuk mengingat bahwa mode yang aku spesifikasikan pada fungsi open() akan mempengaruhi bagaimana Python menuliskan isi ke dalam berkas teks. Jika aku menggunakan mode w, maka Python akan menghapus seluruh isi dalam berkas sebelum menuliskan konten yang aku spesifikasikan.

Asumsikan baris-baris di bawah comment ini merupakan isi dari “hello.txt”

Kita sedang belajar Python
Tepatnya belajar memanipulasi berkas teks
Memanipulasi berkas dengan Python sangatlah mudah!


### Tugas:
Perintah ini aku gunakan untuk membuka/membuat sebuah berkas teks.
Seusai program selesai dijalankan, baris-baris di bawah comment ini merupakan isi dari "hello.txt"

Sekarang kita belajar menulis dengan menggunakan Python
Menulis konten file dengan mode w (write).
```sh
# Menulis ke file hello.txt
file = open("hello.txt", "w")
file.write("Sekarang kita belajar menulis dengan menggunakan Python")
file.write("Menulis konten file dengan mode w (write).")
file.close()
```

### Menulis Berkas Teks – Part 2
Ketika aku menulis pada berkas teks menggunakan mode a, Python tidak akan menghapus isi dalam berkas dan hanya akan menambahkan konten. Aku mempelajari contoh berikut untuk memahami penggunaan fungsi write() dan writelines()

### Tugas:
Pertama, aku mengasumsikan baris-baris di bawah comment ini merupakan isi dari “hello.txt”

Kita sedang belajar Python
Tepatnya belajar memanipulasi berkas teks
Memanipulasi berkas dengan Python sangatlah mudah! 
Perintah ini aku gunakan untuk membuka/membuat sebuah berkas teks dengan menggunakan mode “a”, untuk menambahkan beberapa baris pada berkas teks setelah isi dari berkas awalnya
```sh

# Menulis ke file dengan mode append
file = open("hello.txt", "a")
file.writelines([
"Sekarang kita belajar menulis dengan menggunakan Python",
"Menulis konten file dengan mode a (append)."
])
file.close
```

### Library Matematika pada Python
Salah satu keunikan Python adalah library yang dimilikinya karena dapat di-extend dengan library yang didefinisikan oleh pengguna Python, selain dari library bawaan (built-in) yang dimilikinya. Untuk membuat library yang didefinisikan oleh pengguna umumnya dilakukan dengan menggunakan teknik pemrograman berorientasi obyek (object oriented programming).

Tentunya secara dasar, Python tidak dapat digunakan untuk pengolahan data, komputasi saintifik, machine learning dan bahkan sistem cerdas. Melalui pengembang library tentunya aku memiliki akses ke keperluan atau bidang tersebut. Library ini dapat diinstal melalui command pip yang bersumber dari web python package index.

Bagi yang pernah menggunakan Matlab pasti tahu ada toolbox tertentu misal untuk optimasi, pengolahan sinyal, dll. Jadi, toolbox di Matlab itu ekuivalen dengan library pada Python. Bahasa pemrograman lain seperti R, PHP, GO, Java, dsb tentu juga memiliki hal yang serupa.

Untuk memanggil library pada python, aku dapat menggunakan syntax:

import 
adalah nama library yang akan diimport untuk dapat digunakan dalam kode program yang disusun, baik library bawaan (built-in), library yang tersedia ada di web python package index atau dikembangkan sendiri.

Python adalah salah satu bahasa yang paling diminati untuk pengolahan data secara matematis. Untuk menggunakan fungsi-fungsi matematis yang telah disediakan oleh bahasa Python, aku dapat melakukan proses import library math seperti pada potongan kode berikut:

import math

### Fungsi dalam Library Matematika – Part 1
Di dalam library math aku mempelajari berbagai fungsi, beberapa diantaranya dapat dilihat pada tabel di bawah ini.
| **Fitur**             | **Keterangan**                                                                                   | **Contoh Penggunaan**                        | **Output**           |
| --------------------- | ------------------------------------------------------------------------------------------------ | -------------------------------------------- | -------------------- |
| `math.ceil(x)`        | Menerima input berupa bilangan dan mengembalikan pembulatan ke atas dari bilangan input.         | `math.ceil(10.3)` <br> `math.ceil(13.1)`     | `11` <br> `14`       |
| `math.floor(x)`       | Menerima input berupa bilangan dan mengembalikan pembulatan ke bawah dari bilangan input.        | `math.floor(10.9)` <br> `math.floor(13.7)`   | `10` <br> `13`       |
| `math.fabs(x)`        | Menerima input berupa bilangan dan mengembalikan nilai absolut dari bilangan input.              | `math.fabs(-10.32)` <br> `math.fabs(-13.87)` | `10.32` <br> `13.87` |
| `math.factorial(x)`   | Menerima input berupa bilangan bulat dan mengembalikan hasil faktorial dari bilangan tersebut.   | `math.factorial(5)`                          | `120`                |
| `math.fsum(iterable)` | Menerima input berupa collection (list, tuple, dll.) dan mengembalikan hasil penjumlahan elemen. | `math.fsum([1,2,3])`                         | `6`                  |


```sh
# Import library math
import math
# Fungsi math.ceil()
print(">>> Fungsi math.ceil()")
x = 10.32
y = 13.87
x_ceil = math.ceil(x)
y_ceil = math.ceil(y)
print(x_ceil)
print(y_ceil)
# Fungsi math.floor()
print(">>> Fungsi math.floor()")
x_floor = math.floor(x)
y_floor = math.floor(y)
print(x_floor)
print(y_floor)
# Fungsi math.fabs()
print(">>> Fungsi math.fabs()")
x = 10.32
y = -13.87
x = math.fabs(x)
y = math.fabs(y)
print(x)
print(y)
# Fungsi math.factorial()
print(">>> Fungsi math.factorial()")
x_factorial = math.factorial(5)
print(x_factorial)
# Fungsi math.fsum()
print(">>> Fungsi math.fsum()")
x = [1, 2, 3, 4, 5, 6, -6, -5, -4]
total = math.fsum(x)
print(total)
```
### Fungsi dalam Library Matematika – Part 2
Aku masih melanjutkan bagian terakhir dari (bulit-in) library matematika pada Python yang dapat digunakan untuk perhitungan matematis.
| **Fitur**             | **Keterangan**                                                                                                                                    | **Contoh Penggunaan**                                                                    | **Output**                        |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | --------------------------------- |
| `math.log(x, y)`      | Menerima input berupa dua bilangan (`x` dan `y`) dan mengembalikan logaritma basis `y` dari `x` (atau dengan kata lain, `x = y^z`, hasilnya `z`). | `math.log(8, 2)` <br> `math.log(81, 3)` <br> `math.log(16, 2)`                           | `3` <br> `4` <br> `4`             |
| `math.sqrt(x)`        | Menerima input berupa sebuah bilangan dan mengembalikan akar pangkat dua dari bilangan tersebut.                                                  | `math.sqrt(100)` <br> `math.sqrt(2)`                                                     | `10` <br> `1.4142135`             |
| `math.copysign(x, y)` | Menerima dua input bilangan dan mengembalikan **nilai pertama (x)** dengan **tanda (sign) dari bilangan kedua (y)**.                              | `math.copysign(10.32, -1)` <br> `math.copysign(13.87, -1)` <br> `math.copysign(15, -20)` | `-10.32` <br> `-13.87` <br> `-15` |


```sh
# Import library math
import math
# Fungsi math.log()
print(">>> Fungsi math.log()")
# x = log basis 2 dari 8
x = math.log(8, 2)
# y = log basis 3 dari 81
y = math.log(81, 3)
# z = log basis 10 dari 10000
z = math.log(10000, 10)
print(x)
print(y)
print(z)
# Fungsi math.sqrt()
print(">>> Fungsi math.sqrt()")
# akar kuadrat dari 100
x = math.sqrt(100)
print(x)
# akar kuadrat dari 2
y = math.sqrt(2)
print(y)
# Fungsi math.copysign()
print(">>> Fungsi math.copysign()")
x = 10.32
y = -13.87
z = -15
x = math.copysign(x, z)
y = math.copysign(y, z)
z = math.copysign(z, 10)
print(x)
print(y)
print(z)
``` 
### Mini Quiz
### Pendahuluan
Pada mini project dalam modul "Basic Python for Data Professional Beginner - Part 2", aku akan diuji oleh Senja cara memprediksi harga rumah di Tangerang berdasarkan luas tanah, luas bangunan, serta kedekatan lokasi dengan pusat kota.
Data yang tersedia dalam format teks harus dibaca terlebih dahulu dan kemudian mengubahnya ke dalam list of dict. Data yang berupa list of dict ini akan digunakan untuk memprediksi harga rumah di Tangerang.

### Harga Rumah di Tangerang
“Terima kasih, Aksara! Akhirnya kelar juga pekerjaan kemarin. Masih semangat, kan? Belum kapok kalau ada proyek baru datang lagi? Hahaha,” goda Senja.

“Asalkan ada bonus, maju terus,” candaku.

“Oke, kali ini serius. Kita diminta untuk mengembangkan model prediksi harga rumah di di Tangerang berdasarkan luas tanah, luas bangunan serta kedekatan lokasi dengan pusat kota. Untuk mengembangkan model prediksi ini, saya telah mengumpulkan beberapa data yang diperlukan. Coba kamu lihat,” jelas Senja.
| Luas Tanah (m²) | Luas Bangunan (m²) | Jarak ke Pusat Kota (km) | Harga (×100 Juta Rp) |
| --------------- | ------------------ | ------------------------ | -------------------- |
| 70              | 50                 | 15                       | 500                  |
| 70              | 60                 | 30                       | 400                  |
| 70              | 60                 | 55                       | 300                  |
| 100             | 50                 | 30                       | 700                  |
| 100             | 70                 | 25                       | 1000                 |
| 100             | 70                 | 50                       | 650                  |
| 120             | 100                | 20                       | 2000                 |
| 120             | 80                 | 50                       | 1200                 |
| 150             | 100                | 50                       | 1800                 |
| 150             | 90                 | 15                       | 3000                 |

“Berarti aku akan memprediksi harga rumah ini berdasarkan kemiripan atribut dari data yang telah ada ini?” tanyaku memastikan. Senja mengangguk.

Tugas 1
Aku pun melanjutkan prosesnya dengan membaca file harga_rumah.txt dan merepresentasikan setiap data ke dalam tipe data dictionary dan menampung keseluruhan data dalam sebuah list bernama harga_rumah. 
Setelah selesai memasukkan data dan menemukan jika nilai dari setiap atribut (tanah, bangunan, jarak_ke_pusat) tidak setara, aku mulai agak bingung. Tapi, harus tenang dan jangan panik!

Aku kembali mengecekanya dan memutuskan utnuk melakukan proses transformasi data. Transformasi data dilakukan dengan mengurangi setiap nilai atribut dalam data dengan nilai atribut minimum dan membaginya dengan nilai atribut maksimum yang dikurangi dengan nilai atribut minimum, seperti ini:

Untuk atribut tanah, nilai maksimum adalah 150 dan nilai minimum adalah 70.
Saat nilai atribut tanah 100, proses transformasi akan mengubah nilai atribut ini menjadi 0,375
nilai_transformasi = 100 - 70 / (150 - 70)
Aku mulai mendapat solusi untuk mempermudah proses transformasi data.

Tugas 2
Mula-mula,  aku akan membuat sebuah fungsi bernama get_all_specified_attribute yang menerima parameter list_of_dictionary (tipe data list yang berisikan sekumpulan tipe data dictionary) dan specified_key (tipe data string). Fungsi akan mengembalikan sebuah list yang berisikan seluruh atribut dengan kunci (key) specified_key.

Tugas 3

Kemudian, setelah berhasil membuat fungsi  tersebut, aku juga membuat fungsi min_value yang menerima parameter list_attributes (berupa tipe data list) dan mengembalikan nilai terkecil dalam list_attributes dan max_value yang menerima parameter list_attributes dan mengembalikan nilai terbesar dalam list_attributes.

Tugas 4
Selanjutnya aku membuat fungsi transform_attribute yang menerima parameter attr (sebuah bilangan), max_attr (sebuah bilangan) dan min_attr (sebuah bilangan) yang mengembalikan nilai transformasi dari sebuah attribute.

Tugas 5
“Sudah cukup, Nja?” tanyaku saat Senja terdiam lama menelusuri hasil kerjaku.

“Menurutku kita masih butuh fungsi baru yaitu fungsi data_transformation yang menerima parameter list_of_dictionary (sebuah list yang berisikan tipe data dictionary) dan list_attribute_names (sebuah list yang berisikan tipe data string) mengembalikan hasil transformasi data dari list_of_dictionary berdasarkan list_attribute_names telah dispesifikasikan.

Tugas 6
Dari data baru dan attr_info ini, Senja menyuruhku membuat fungsi transform_data yang menerima parameter data dan attr_info dan mengembalikan nilai atribut dari data baru yang telah ditransformasikan.

Tugas 7
Setelah itu, Senja memintaku untuk membuat sistem prediksi harga berdasarkan nilai kemiripan atribut.

Tugas 8
Dan aku menggunakan semua fungsi yang telah aku definisikan dari Step 1 s/d Step 7.

Hitung harga rumah yang telah ditransformasikan ke dalam variabel harga_rumah berikut dengan atributnya attr_info
Gunakan variabel data untuk memprediksi harga rumah
data = {'tanah': 110, 'bangunan': 80, 'jarak_ke_pusat': 35}
transformasikan data tersebut dengan dengan menggunakan attr_info yang telah diperoleh yang kembali disimpan ke variabel data.
Hitunglah prediksi harga dari variabel data tersebut. 

```sh
import requests
from contextlib import closing
import csv
# STEP 1: 
# Baca file "harga_rumah.txt"
url = "https://storage.googleapis.com/dqlab-dataset/harga_rumah.txt"
data_harga_rumah = []
with closing(requests.get(url, stream=True)) as r:
    f = (line.decode('utf-8') for line in r.iter_lines())
    data_harga_rumah = [row for row in csv.reader(f)]
# Buat list of dict dengan nama harga rumah
key_harga_rumah = data_harga_rumah[0]
harga_rumah = []
for baris_harga_rumah in data_harga_rumah[1:]:
	dict_harga_rumah = dict()
	for i in range(len(baris_harga_rumah)):
		dict_harga_rumah[key_harga_rumah[i]] = baris_harga_rumah[i]
	harga_rumah.append(dict_harga_rumah)
print(harga_rumah)
# STEP 2:
# Buat fungsi  get_all_specified_attribute yang menerima parameter list_of_dictionary 
# (tipe data list yang berisikan sekumpulan tipe data dictionary) dan specified_key 
# (tipe data string). Fungsi akan mengembalikan sebuah list yang berisikan seluruh 
# atribut dengan kunci (key) specified_key. 
def get_all_specified_attributes(list_of_dictionary, specified_key):
	list_attributes = []
	for data in list_of_dictionary:
		attribute = data[specified_key]
		list_attributes.append(attribute)
	return list_attributes
# STEP 3: 
# Buat fungsi fungsi min_value yang menerima parameter list_attributes (berupa 
# tipe data list) dan mengembalikan nilai terkecil dalam list_attributes 
def min_value(list_attributes):
	min_attribute = 9999
	for attr in list_attributes:
		if int(attr) < min_attribute:
			min_attribute = int(attr)
	return min_attribute
# Buat fungsi dan max_value yang menerima parameter list_attribute dan 
# mengembalikan nilai terbesar dalam list_attributes.	
def max_value(list_attributes):
	max_attribute = -9999
	for attr in list_attributes:
		if int(attr) > max_attribute:
			max_attribute = int(attr)
	return max_attribute
# STEP 4: 
# Buat fungsi transform_attribute yang menerima parameter attr (sebuah 
# bilangan), max_attr (sebuah bilangan) dan min_attr (sebuah bilangan) 
# yang mengembalikan nilai transformasi dari sebuah attribute.
def transform_attribute(attr, max_attr, min_attr):
	nilai_transformasi = (attr - min_attr) / (max_attr - min_attr)
	return nilai_transformasi
# STEP 5:
# Buat fungsi data_transformation yang menerima parameter list_of_dictionary 
# (sebuah list yang berisikan tipe data dictionary) dan list_attribute_names 
# (sebuah list yang berisikan tipe data string) mengembalikan hasil 
# transformasi data dari list_of_dictionary berdasarkan list_attribute_names 
# dan attr_info telah dispesifikasikan.
def data_transformation(list_of_dictionary, list_attribute_names):
	attr_info = {}
	for attr_name in list_attribute_names:
		specified_attributes = get_all_specified_attributes(list_of_dictionary, attr_name)
		max_attr = max_value(specified_attributes)
		min_attr = min_value(specified_attributes)
		attr_info[attr_name] = {'max': max_attr, 'min': min_attr}
		data_idx = 0
		while(data_idx < len(list_of_dictionary)):
			list_of_dictionary[data_idx][attr_name] = transform_attribute(int(list_of_dictionary[data_idx][attr_name]), max_attr, min_attr)
			data_idx += 1
	return list_of_dictionary, attr_info
# STEP 6:
# Berdasarkan data baru dan attr_info ini, buat fungsi transform_data yang
# menerima parameter data dan attr_info dan mengembalikan nilai atribut 
# dari data baru yang telah ditransformasikan.
def transform_data(data, attr_info):
	for key_name in data.keys():
		data[key_name] = (data[key_name] - attr_info[key_name]['min']) / (
		                  attr_info[key_name]['max'] - attr_info[key_name]['min'])
	return data
# STEP 7:
# Buat fungsi yang digunakan untuk sistem prediksi harga berdasarkan 
# nilai kemiripan atribut, yaitu argument input data dan list_of_data!
def abs_value(value):
	if value < 0:
		return -value
	else:
		return value
def price_based_on_similarity(data, list_of_data):
	prediksi_harga = 0
	perbedaan_terkecil = 999
	for data_point in list_of_data:
		perbedaan= abs_value(data['tanah'] - data_point['tanah'])
		perbedaan+= abs_value(data['bangunan'] - data_point['bangunan'])
		perbedaan+= abs_value(data['jarak_ke_pusat'] - data_point['jarak_ke_pusat'])
		if perbedaan < perbedaan_terkecil:
			prediksi_harga = data_point['harga']
			perbedaan_terkecil = perbedaan
	return prediksi_harga
# STEP 8:
# Hitung harga rumah yang telah ditransformasikan ke dalam variabel 
# harga_rumah berikut dengan atributnya attr_info
harga_rumah, attr_info = data_transformation(harga_rumah,
                                             ['tanah','bangunan','jarak_ke_pusat'])
# Gunakan variabel data untuk memprediksi harga rumah
data = {'tanah': 110, 'bangunan': 80, 'jarak_ke_pusat': 35}
# Transformasikan data tersebut dengan dengan menggunakan attr_info yang telah 
# diperoleh yang kembali disimpan ke variabel data.
data = transform_data(data, attr_info)
# Hitunglah prediksi harga dari variabel data tersebut.
harga = price_based_on_similarity(data, harga_rumah)
print("Prediksi harga rumah: ", harga)
```
