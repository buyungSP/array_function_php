###### Membuat

array()
------
>Membuat sebuah array

Syntax

Syntax untuk array terindeks:
>array(nilai1, nilai2, nilai3, dll.)

Syntax untuk array asosiatif:
>array(kunci=>nilai, kunci=>nilai, kunci=>nilai, dll.)

**kunci**
:Menentukan kunci (numerik atau string)

**nilai**
:Menentukan nilai

array_combine()
------
>Membuat sebuah array dengan menggunakan elemen dari array "keys" dan array "values"

Syntax
>array_combine(kunci, nilai)

**kunci** ___wajib___
:Array kunci

**nilai** ___wajib___
:Array nilai

Key
######

array_change_key_case()
------
>Mengubah semua kunci dalam array menjadi huruf kecil atau besar

Syntax
>array_change_key_case(array, case)

**array** ___wajib___
:Menentukan array yang akan digunakan

**case** ___opsional___
:Nilai yang mungkin
	- **CASE_LOWER** - Nilai default. Mengubah kunci menjadi huruf kecil
	- **CASE_UPPER** - Mengubah kunci menjadi huruf besar

array_key_exists()
------
>Memeriksa apakah kunci yang ditentukan ada dalam array

Syntax
>array_key_exists(kunci, array)

Nilai Parameter
| Parameter | Deskripsi |
| --------- | --------- |
| kunci Diperlukan. | Menentukan kunci |
| array Diperlukan. | Menentukan sebuah array |

array_keys()
------
>Mengembalikan semua kunci dari sebuah array

Syntax
>array_keys(array, value, strict)

Nilai Parameter
| Parameter | Deskripsi |
| --------- | --------- |
| array Wajib. | Menentukan sebuah array |
| value Pilihan. | Anda dapat menentukan nilai, maka hanya kunci dengan nilai ini yang akan dikembalikan |
| strict Pilihan. | Digunakan dengan parameter nilai. Nilai yang mungkin: |
| | <ul><li>**true** - Mengembalikan kunci dengan nilai yang ditentukan, tergantung pada tipe: angka 5 tidak sama dengan string "5".</li><li>**false** - Nilai default. Tidak tergantung pada tipe, angka 5 sama dengan string "5".</li></ul> |




array_chunk()
------
>Memecah sebuah array menjadi beberapa bagian array

Syntax
>array_chunk(array, size, preserve_key)

Parameter Values
| Parameter | Description |
| --------- | --------- |
| array Diperlukan. | Menentukan array yang akan digunakan |
| size Diperlukan. | Sebuah bilangan bulat yang menentukan ukuran setiap potongan |
| preserve_key Pilihan. | Nilai yang mungkin: |
| | <ul><li>**true** - Menjaga kunci</li><li>**false** - Default. Mengindeks ulang potongan secara numerik</li></ul> |

array_column()
------
>Mengembalikan nilai dari sebuah kolom tunggal dalam array input

array_count_values()
------
>Menghitung jumlah nilai dari sebuah array

array_fill()
------
>Mengisi sebuah array dengan nilai tertentu

array_fill_keys()
------
>Mengisi sebuah array dengan nilai tertentu, dengan menentukan kunci

array_filter()
------
>Menyaring nilai-nilai dari sebuah array menggunakan fungsi callback

array_flip()
------
>Membalikkan/menukar semua kunci dengan nilai yang terkait dalam sebuah array

array_map()
------
>Mengirim setiap nilai dari sebuah array ke sebuah fungsi buatan pengguna, yang mengembalikan nilai baru

array_merge()
------
>Menggabungkan satu atau lebih array menjadi sebuah array

array_merge_recursive()
------
>Menggabungkan satu atau lebih array menjadi sebuah array secara rekursif

array_pad()
------
>Menyisipkan sejumlah item yang ditentukan, dengan nilai tertentu, ke dalam sebuah array

array_pop()
------
>Menghapus elemen terakhir dari sebuah array

array_product()
------
>Menghitung hasil kali dari nilai-nilai dalam sebuah array

array_push()
------
>Menyisipkan satu atau lebih elemen ke akhir sebuah array

array_rand()
------
>Mengembalikan satu atau lebih kunci acak dari sebuah array

array_reduce()
------
>Mengembalikan sebuah array sebagai sebuah string, dengan menggunakan fungsi yang ditentukan pengguna

array_replace()
------
>Menggantikan nilai-nilai dari array pertama dengan nilai-nilai dari array yang mengikuti

array_replace_recursive()
------
>Menggantikan nilai-nilai dari array pertama dengan nilai-nilai dari array yang mengikuti secara rekursif

array_reverse()
------
>Mengembalikan sebuah array dalam urutan terbalik

array_search()
------
>Mencari sebuah nilai tertentu dalam sebuah array dan mengembalikan kunci yang terkait

array_shift()
------
>Menghapus elemen pertama dari sebuah array, dan mengembalikan nilai dari elemen yang dihapus

array_unshift()
------
>Menambahkan satu atau lebih elemen ke awal sebuah array

array_slice()
------
>Mengembalikan bagian terpilih dari sebuah array

array_splice()
------
>Menghapus dan mengganti elemen-elemen tertentu dari sebuah array

array_sum()
------
>Mengembalikan jumlah dari nilai-nilai dalam sebuah array

array_unique()
------
>Menghapus nilai-nilai duplikat dari sebuah array

array_values()
------
>Mengembalikan semua nilai dari sebuah array

array_walk()
------
>Menerapkan sebuah fungsi buatan pengguna ke setiap anggota dari sebuah array

array_walk_recursive()
------
>Menerapkan sebuah fungsi buatan pengguna secara rekursif ke setiap anggota dari sebuah array




Membandingkan
######

array_diff()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya nilai)

array_udiff()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

array_diff_assoc()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai)

array_diff_uassoc()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

array_udiff_assoc()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai, menggunakan fungsi bawaan untuk membandingkan kunci dan fungsi pembanding nilai yang ditentukan pengguna)

array_udiff_uassoc()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai, menggunakan dua fungsi pembanding kunci yang ditentukan pengguna)

array_diff_key()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya kunci)

array_diff_ukey()
------
>Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya kunci, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

array_intersect()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya nilai)

array_uintersect()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

array_intersect_assoc()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai)

array_intersect_uassoc()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

array_uintersect_assoc()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai, menggunakan fungsi bawaan untuk membandingkan kunci dan fungsi pembanding nilai yang ditentukan pengguna)

array_uintersect_uassoc()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai, menggunakan dua fungsi pembanding kunci yang ditentukan pengguna)

array_intersect_key()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya kunci)

array_intersect_ukey()
------
>Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya kunci, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Mengurutkan
######

array_multisort()
------
>Mengurutkan beberapa atau multidimensional array

natcasesort()
------
>Mengurutkan sebuah array menggunakan algoritma "natural order" yang tidak memperhatikan huruf besar atau kecil

natsort()
------
>Mengurutkan sebuah array menggunakan algoritma "natural order"

sort()
------
>Mengurutkan sebuah array indeks secara menaik

asort()
------
>Mengurutkan sebuah array asosiatif secara menaik, berdasarkan nilai

rsort()
------
>Mengurutkan sebuah array indeks secara menurun

usort()
------
>Mengurutkan sebuah array berdasarkan nilai menggunakan sebuah fungsi pembanding yang ditentukan pengguna

ksort()
------
>Mengurutkan sebuah array asosiatif secara menaik, berdasarkan kunci

krsort()
------
>Mengurutkan sebuah array asosiatif secara menurun, berdasarkan kunci

uksort()
------
>Mengurutkan sebuah array berdasarkan kunci menggunakan sebuah fungsi pembanding yang ditentukan pengguna

arsort()
------
>Mengurutkan sebuah array asosiatif secara menurun, berdasarkan nilai

uasort()
------
>Mengurutkan sebuah array berdasarkan nilai menggunakan sebuah fungsi pembanding yang ditentukan pengguna dan mempertahankan asosiasi indeks







compact()
------
>Membuat sebuah array yang berisi variabel-variabel dan nilai-nilainya

range()
------
>Membuat sebuah array yang berisi rentang elemen

key()
------
>Mengambil sebuah kunci dari sebuah array

each()
------
>Ditolak dari PHP 7.2. Mengembalikan pasangan kunci dan nilai saat ini dari sebuah array

extract()
------
>Mengimpor variabel-variabel ke dalam tabel simbol saat ini dari sebuah array

in_array()
------
>Memeriksa apakah sebuah nilai tertentu ada dalam sebuah array

list()
------
>Memberikan nilai-nilai variabel seolah-olah mereka adalah sebuah array

count()
------
>Mengembalikan jumlah elemen dalam sebuah array

sizeof()
------
>Alias dari count()

current()
------
>Mengembalikan elemen saat ini dari sebuah array

pos()
------
>Alias dari current()

end()
------
>Mengatur pointer internal dari sebuah array ke elemen terakhirnya

next()
------
>Maju ke elemen berikutnya dari sebuah array

prev()
------
>Mundurkan pointer internal sebuah array

reset()
------
>Mengatur pointer internal dari sebuah array ke elemen pertamanya

shuffle()
------
>Mengacak sebuah array