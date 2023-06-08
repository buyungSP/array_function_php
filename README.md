------

# Membuat

array()
------
> Membuat sebuah array

Fungsi array() digunakan untuk membuat array.

Di PHP, ada tiga jenis array:

- Array indeks - Array dengan indeks numerik
- Array asosiatif - Array dengan kunci bernama
- Array multidimensi - Array yang berisi satu atau lebih array.

Syntax
Syntax untuk array terindeks:
> array(nilai1, nilai2, nilai3, dll.)

Syntax untuk array asosiatif:
> array(kunci=>nilai, kunci=>nilai, kunci=>nilai, dll.)
> 
> **kunci**
> - Menentukan kunci (numerik atau string)
> 
> **nilai**
> - Menentukan nilai

array_combine()
------
> Membuat sebuah array dengan menggunakan elemen dari array "keys" dan array "values"

Fungsi array_combine () membuat array dengan menggunakan elemen dari satu array "keys" dan satu array "values".

Catatan: Kedua array harus memiliki jumlah elemen yang sama!

Syntax
> array_combine(kunci, nilai)
> 
> **kunci** ___wajib___
> - Array kunci
> 
> **nilai** ___wajib___
> - Array nilai

------

# Key

array_change_key_case()
------
> Mengubah semua kunci dalam array menjadi huruf kecil atau besar

Fungsi array_change_key_case () mengubah semua kunci dalam sebuah array menjadi huruf kecil atau huruf besar.

Syntax
> array_change_key_case(array, case)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan
> 
> **case** ___opsional___
> - Nilai yang mungkin
> 	- **CASE_LOWER** - Nilai **Default**. Mengubah kunci menjadi huruf kecil
> 	- **CASE_UPPER** - Mengubah kunci menjadi huruf besar

array_key_exists()
------
> Memeriksa apakah kunci yang ditentukan ada dalam array

Fungsi array_key_exists() memeriksa apakah terdapat kunci tertentu pada sebuah array, dan mengembalikan nilai true jika kunci tersebut ada dan false jika kunci tersebut tidak ada.

Tips: Ingatlah bahwa jika Anda tidak menentukan kunci pada saat menentukan sebuah array, maka kunci integer akan dihasilkan, dimulai dari 0 dan meningkat sebanyak 1 untuk setiap nilai. (Lihat contoh di bawah ini)

Syntax
> array_key_exists(kunci, array)
> 
> **kunci** ___wajib___
> - Menentukan kunci
> 
> **array** ___wajib___
> - Menentukan kunci

array_keys()
------
> Mengembalikan semua kunci dari sebuah array

Fungsi array_keys() mengembalikan sebuah array yang berisi kunci-kunci.

Syntax
> array_keys(array, value, strict)
> 
> **array** ___wajib___
> - Menentukan sebuah array
> 
> **value** ___opsional___
> - Anda dapat menentukan nilai, maka hanya kunci dengan nilai ini yang akan dikembalikan
> 
> **strict** ___opsional___
> - Digunakan dengan parameter nilai. Nilai yang mungkin
> 	- **true** - Mengembalikan kunci dengan nilai yang ditentukan, tergantung pada tipe: angka 5 tidak sama dengan string "5".
> 	- **false** - Nilai **Default**. Tidak tergantung pada tipe, angka 5 sama dengan string "5".

array_chunk()
------
> Memecah sebuah array menjadi beberapa bagian array

Fungsi array_chunk() membagi sebuah array menjadi beberapa bagian array yang baru.

Syntax
> array_chunk(array, size, preserve_key)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan
> 
> **size** ___wajib___
> - Sebuah bilangan bulat yang menentukan ukuran setiap potongan
> 
> **preserve_key** ___opsional___
> - Nilai yang mungkin
> 	- **true** - Menjaga kunci
> 	- **false** - **Default**. Mengindeks ulang potongan secara numerik

array_column()
------
> Mengembalikan nilai dari sebuah kolom tunggal dalam array input

Fungsi array_column () mengembalikan nilai dari satu kolom dalam array masukan.

Syntax
> array_column(array, column_key, index_key)
> 
> **array** ___wajib___
> - Menentukan array multi-dimensi (record-set) yang akan digunakan. Mulai PHP 7.0, ini juga dapat berupa array objek.
> 
> **column_key** ___wajib___
> - Kunci integer atau nama kunci string dari kolom nilai yang akan dikembalikan. Parameter ini juga dapat berupa NULL untuk mengembalikan array lengkap (berguna bersama dengan index_key untuk mengindeks ulang array)
> 
> **index_key** ___opsional___
> - Kolom yang akan digunakan sebagai indeks/kunci untuk array yang dikembalikan

array_count_values()
------
> Menghitung jumlah nilai dari sebuah array

Fungsi array_count_values () menghitung semua nilai dari sebuah array.

Syntax
> array_count_values(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan dihitung nilai-nilainya.

array_fill()
------
> Mengisi sebuah array dengan nilai tertentu

Fungsi array_fill() mengisi sebuah array dengan nilai-nilai.

Syntax
> array_fill(index, jumlah, nilai)
> 
> **index** ___Wajib___
> - Indeks pertama dari array yang akan dikembalikan
> **jumlah** ___Wajib___
> - Menentukan jumlah elemen yang akan dimasukkan
> **nilai** ___Wajib___
> - Menentukan nilai yang akan digunakan untuk mengisi array

array_fill_keys()
------
> Mengisi sebuah array dengan nilai tertentu, dengan menentukan kunci

Fungsi array_fill_keys () mengisi sebuah array dengan nilai, dengan menentukan kunci.

Syntax
> array_fill_keys(kunci, nilai)
> 
> **kunci** ___Wajib___
> - Array dari nilai-nilai yang akan digunakan sebagai kunci
> **nilai** ___Wajib___
> - Menentukan nilai yang akan digunakan untuk mengisi array

array_filter()
------
> Menyaring nilai-nilai dari sebuah array menggunakan fungsi callback

Fungsi array_filter() digunakan untuk menyaring nilai-nilai dalam sebuah array menggunakan fungsi callback.

Fungsi ini akan memasukkan setiap nilai dari array input ke dalam fungsi callback. Jika fungsi callback mengembalikan nilai true, maka nilai saat ini dari input akan dimasukkan ke dalam array hasil. Kunci array akan dipertahankan.

Syntax
> array_filter(array, callbackfunction, flag)
> 
> **array** ___Wajib___
> - Menentukan array yang akan difilter
> **callbackfunction** ___Opsional___
> - Menentukan fungsi callback yang akan digunakan
> **flag** ___Opsional___
> - Menentukan argumen apa yang akan dikirim ke callback:
> 	- **ARRAY_FILTER_USE_KEY** - kirim kunci sebagai satu-satunya argumen ke callback (bukan nilai)
> 	- **ARRAY_FILTER_USE_BOTH** - kirim baik nilai maupun kunci sebagai argumen ke callback (bukan nilai)

array_flip()
------
> Membalikkan/menukar semua kunci dengan nilai yang terkait dalam sebuah array

Fungsi array_flip() membalikkan/menukar semua kunci dengan nilai yang terkait dalam sebuah array.

Syntax
> array_flip(array)
> 
> **array** ___Diperlukan___
> - Menentukan sebuah array pasangan kunci/nilai yang akan dibalikkan.

array_map()
------
> Mengirim setiap nilai dari sebuah array ke sebuah fungsi buatan pengguna, yang mengembalikan nilai baru

Fungsi array_map () mengirimkan setiap nilai dari sebuah array ke fungsi yang dibuat pengguna, dan mengembalikan array dengan nilai baru, yang diberikan oleh fungsi yang dibuat pengguna.

Tip: Anda dapat menetapkan satu array ke fungsi, atau sebanyak yang Anda inginkan.

Syntax
> array_map(myfunction, array1, array2, array3, ...)
> 
> **myfunction** ___Wajib___
> - Nama fungsi buatan pengguna, atau null
> **array1** ___Wajib___
> - Menentukan sebuah array
> **array2** ___Pilihan___
> - Menentukan sebuah array
> **array3** ___Pilihan___
> - Menentukan sebuah array

array_merge()
------
> Menggabungkan satu atau lebih array menjadi sebuah array

Fungsi array_merge () menggabungkan satu atau lebih array menjadi satu array.

Tips: Anda dapat menetapkan satu array ke fungsi, atau sebanyak yang Anda inginkan.

Catatan: Jika dua atau lebih elemen array memiliki kunci yang sama, yang terakhir akan menggantikan yang lain.

Catatan: Jika Anda hanya menetapkan satu array ke fungsi array_merge () dan kuncinya adalah bilangan bulat, fungsi tersebut mengembalikan array baru dengan kunci bilangan bulat yang dimulai dari 0 dan meningkat sebesar 1 untuk setiap nilai (lihat contoh di bawah).

Tips: Perbedaan antara fungsi ini dan fungsi array_merge_recursive () adalah ketika dua atau lebih elemen array memiliki kunci yang sama. Alih-alih mengganti kunci, fungsi array_merge_recursive () membuat nilai sebagai array.

Syntax
> array_merge(array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Menentukan sebuah array
> **array2** ___Pilihan___
> - Menentukan sebuah array
> **array3,...** ___Pilihan___
> - Menentukan sebuah array lainnya

array_merge_recursive()
------
> Menggabungkan satu atau lebih array menjadi sebuah array secara rekursif

Fungsi array_merge_recursive() menggabungkan satu atau lebih array menjadi satu array.

Perbedaan antara fungsi ini dan fungsi array_merge() adalah ketika dua atau lebih elemen array memiliki kunci yang sama. Alih-alih menimpa kunci-kunci tersebut, fungsi array_merge_recursive() membuat nilai sebagai array.

Catatan: Jika Anda hanya memberikan satu array ke fungsi array_merge_recursive(), maka fungsi tersebut akan berperilaku sama persis dengan fungsi array_merge().

Syntax
> array_merge_recursive(array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Menentukan sebuah array
> **array2** ___Pilihan___
> - Menentukan sebuah array
> **array3,...** ___Pilihan___
> - Menentukan sebuah array lainnya

array_pad()
------
> Menyisipkan sejumlah item yang ditentukan, dengan nilai tertentu, ke dalam sebuah array

Fungsi array_pad() menyisipkan sejumlah elemen yang ditentukan, dengan nilai tertentu, ke dalam sebuah array.

Tip: Jika Anda memberikan parameter ukuran yang negatif, fungsi ini akan menyisipkan elemen-elemen baru SEBELUM elemen-elemen asli (lihat contoh di bawah).

Catatan: Fungsi ini tidak akan menghapus elemen-elemen apapun jika parameter ukuran lebih kecil dari ukuran array asli.

Syntax
> array_pad(array, size, value)
> 
> **array** ___Diperlukan___
> - Menentukan sebuah array
> **size** ___Diperlukan___
> - Menentukan jumlah elemen dalam array yang dihasilkan dari fungsi
> **value** ___Diperlukan___
> - Menentukan nilai elemen-elemen baru dalam array yang dihasilkan dari fungsi

array_pop()
------
> Menghapus elemen terakhir dari sebuah array

Fungsi array_pop() menghapus elemen terakhir dari sebuah array.

Syntax
> array_count_values(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan dihitung nilai-nilainya.

array_product()
------
> Menghitung hasil kali dari nilai-nilai dalam sebuah array

Fungsi array_product() menghitung dan mengembalikan hasil kali dari elemen-elemen dalam sebuah array.

Syntax
> array_count_values(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan dihitung nilai-nilainya.

array_push()
------
> Menyisipkan satu atau lebih elemen ke akhir sebuah array

Fungsi array_push() memasukkan satu atau lebih elemen ke akhir dari sebuah array.

Tips: Anda dapat menambahkan satu nilai atau sebanyak yang Anda inginkan.

Catatan: Meskipun array Anda memiliki kunci string, elemen yang ditambahkan selalu memiliki kunci numerik (lihat contoh di bawah).

Syntax
> array_push(array, value1, value2, ...)
> 
> **array** ___Diperlukan___
> - Menentukan array
> **value1** ___Tidak wajib___
> - Menentukan nilai yang akan ditambahkan (Diperlukan pada versi PHP sebelum 7.3)
> **value2** ___Tidak wajib___
> - Menentukan nilai yang akan ditambahkan.

array_rand()
------
> Mengembalikan satu atau lebih kunci acak dari sebuah array

Fungsi array_rand() mengembalikan kunci acak dari sebuah array, atau mengembalikan array dari kunci acak jika Anda menentukan bahwa fungsi harus mengembalikan lebih dari satu kunci.

Syntax
> array_rand(array, number)
> 
> **array** ___Diperlukan___
> - Menentukan array
> **number** ___Pilihan___
> - Menentukan berapa banyak kunci acak yang akan dikembalikan

array_reduce()
------
> Mengembalikan sebuah array sebagai sebuah string, dengan menggunakan fungsi yang ditentukan pengguna

Fungsi array_reduce() mengirimkan nilai-nilai dalam sebuah array ke dalam fungsi yang telah ditentukan oleh pengguna, dan mengembalikan sebuah string.

Catatan: Jika array kosong dan nilai awal tidak diberikan, fungsi ini akan mengembalikan NULL.

Syntax
> array_reduce(array, myfunction, initial)
> 
> **array** ___Wajib___
> - Menentukan array
> **myfunction** ___Wajib___
> - Menentukan nama fungsi
> **initial** ___Opsional___
> - Menentukan nilai awal yang akan dikirimkan ke fungsi

array_replace()
------
> Menggantikan nilai-nilai dari array pertama dengan nilai-nilai dari array yang mengikuti

Fungsi array_replace() menggantikan nilai-nilai dari array pertama dengan nilai-nilai dari array yang mengikuti.

Tip: Anda dapat menetapkan satu array ke fungsi, atau sebanyak yang Anda inginkan.

Jika kunci dari array1 ada di array2, nilai dari array1 akan digantikan oleh nilai dari array2. Jika kunci hanya ada di array1, maka akan tetap seperti itu (lihat Contoh 1 di bawah).

Jika kunci ada di array2 dan tidak di array1, maka akan dibuat di array1 (lihat Contoh 2 di bawah).

Jika beberapa array digunakan, nilai dari array yang lebih akhir akan menimpa yang sebelumnya (lihat Contoh 3 di bawah).

Tip: Gunakan array_replace_recursive() untuk menggantikan nilai dari array1 dengan nilai dari array yang mengikuti secara rekursif.

Syntax
> array_replace(array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Menentukan sebuah array
> **array2** ___Opsional___
> - Menentukan sebuah array yang akan menggantikan nilai dari array1
> **array3,...** ___Opsional___
> - Menentukan beberapa array untuk menggantikan nilai dari array1 dan array2, dll. Nilai dari array yang lebih akhir akan menimpa yang sebelumnya.

array_replace_recursive()
------
> Menggantikan nilai-nilai dari array pertama dengan nilai-nilai dari array yang mengikuti secara rekursif

Fungsi array_replace_recursive () menggantikan nilai-nilai dari array pertama dengan nilai dari array berikutnya secara rekursif.

Tip: Anda dapat menetapkan satu array ke fungsi, atau sebanyak yang Anda inginkan.

Jika kunci dari array1 ada di array2, nilai dari array1 akan digantikan oleh nilai dari array2. Jika kunci hanya ada di array1, maka akan dibiarkan seperti itu. Jika kunci ada di array2 dan tidak di array1, maka akan dibuat di array1. Jika beberapa array digunakan, nilai dari array yang lebih baru akan menimpa yang sebelumnya.

Catatan: Jika Anda tidak menentukan kunci untuk setiap array, fungsi ini akan berperilaku sama persis dengan fungsi array_replace ().

Syntax
> array_replace_recursive (array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Menentukan sebuah array
> **array2** ___Opsional___
> - Menentukan sebuah array yang akan menggantikan nilai dari array1
> **array3,...** ___Opsional___
> - Menentukan beberapa array untuk menggantikan nilai dari array1 dan array2, dll. Nilai dari array yang lebih akhir akan menimpa yang sebelumnya.

array_reverse()
------
> Mengembalikan sebuah array dalam urutan terbalik

Fungsi array_reverse () mengembalikan array dalam urutan terbalik.

Syntax
> array_reverse(array, preserve)
> 
> **array** ___Wajib___Menentukan array
> **preserve** ___Opsional___
> - Menentukan apakah fungsi harus mempertahankan kunci array atau tidak. Nilai yang mungkin:
> 	- **benar**
> 	- **salah**

array_search()
------
> Mencari sebuah nilai tertentu dalam sebuah array dan mengembalikan kunci yang terkait

Fungsi array_search () mencari nilai dalam sebuah array dan mengembalikan kunci.

Syntax
> array_search (nilai, array, strict)
> 
> **nilai** ___Diperlukan___
> - Menentukan nilai yang dicari
> **array** ___Diperlukan___
> - Menentukan array yang akan dicari
> **strict** ___Pilihan___
> - Jika parameter ini diatur ke TRUE, maka fungsi ini akan mencari elemen yang identik dalam array. Nilai yang mungkin:
> 	- **benar**
> 	- **salah** - **Default**
> 		Ketika diatur ke benar, angka 5 tidak sama dengan string 5

array_shift()
------
> Menghapus elemen pertama dari sebuah array, dan mengembalikan nilai dari elemen yang dihapus

Fungsi array_shift() menghapus elemen pertama dari sebuah array, dan mengembalikan nilai dari elemen yang dihapus.

Catatan: Jika kunci pada array adalah numerik, semua elemen akan mendapatkan kunci baru, dimulai dari 0 dan bertambah satu (lihat contoh di bawah).

Syntax
> array_shift(array)
> 
> **array** ___Wajib___
> - Menentukan sebuah array.



array_unshift()
------
> Menambahkan satu atau lebih elemen ke awal sebuah array

Fungsi array_unshift () memasukkan elemen-elemen baru ke dalam array. Nilai-nilai array baru akan dimasukkan di awal array.

Tip: Anda dapat menambahkan satu nilai, atau sebanyak yang Anda inginkan.

Catatan: Kunci numerik akan dimulai dari 0 dan meningkat sebanyak 1. Kunci string akan tetap sama.

Syntax
> array_unshift (array, value1, value2, value3, ...)
> 
> **array** ___Diperlukan___
> - Menentukan array
> **value1** ___Opsional___
> - Menentukan nilai yang akan dimasukkan (Diperlukan pada versi PHP sebelum 7.3)
> **value2** ___Opsional___
> - Menentukan nilai yang akan dimasukkan
> **value3** ___Opsional___
> - Menentukan nilai yang akan dimasukkan

array_slice()
------
> Mengembalikan bagian terpilih dari sebuah array

Fungsi array_slice() mengembalikan bagian-bagian tertentu dari sebuah array.

Catatan: Jika array memiliki kunci string, array yang dikembalikan akan selalu mempertahankan kunci-kunci tersebut (lihat contoh 4).

Syntax
> array_slice(array, start, length, preserve)
> 
> **array** ___Wajib___
> - Menentukan array
> **start** ___Wajib___
> - Nilai numerik. Menentukan dari mana fungsi akan memulai slice. 0 = elemen pertama. Jika nilai ini diatur ke angka negatif, fungsi akan mulai memotong sejauh itu dari elemen terakhir. -2 berarti mulai pada elemen kedua terakhir dari array.
> **length** ___Opsional___
> - Nilai numerik. Menentukan panjang array yang dikembalikan. Jika nilai ini diatur ke angka negatif, fungsi akan berhenti memotong sejauh itu dari elemen terakhir. Jika nilai ini tidak diatur, fungsi akan mengembalikan semua elemen, dimulai dari posisi yang ditetapkan oleh parameter start.
> **preserve** ___Opsional___
> - Menentukan apakah fungsi harus mempertahankan atau mengatur ulang kunci-kunci. Nilai yang mungkin:
> 	- **true** - Mempertahankan kunci
> 	- **false** - **Default**. Mengatur ulang kunci.

array_splice()
------
> Menghapus dan mengganti elemen-elemen tertentu dari sebuah array

Fungsi array_splice () menghapus elemen yang dipilih dari sebuah array dan menggantinya dengan elemen baru. Fungsi ini juga mengembalikan sebuah array dengan elemen-elemen yang dihapus.

Tip: Jika fungsi tidak menghapus elemen apa pun (length=0), array yang diganti akan dimasukkan dari posisi parameter start (Lihat Contoh 2).

Catatan: Kunci dalam array yang diganti tidak dipertahankan.

Syntax
> array_splice(array, start, length, array)
> 
> **array** ___Wajib___
> - Menentukan sebuah array
> **start** ___Wajib___
> - Nilai numerik. Menentukan dari mana fungsi akan mulai menghapus elemen. 0 = elemen pertama. Jika nilai ini diatur menjadi nomor negatif, fungsi akan mulai dari sejauh itu dari elemen terakhir. -2 berarti mulai dari elemen kedua terakhir dari array.
> **length** ___Opsional___
> - Nilai numerik. Menentukan berapa banyak elemen yang akan dihapus, dan juga panjang array yang dikembalikan. Jika nilai ini diatur menjadi nomor negatif, fungsi akan berhenti sejauh itu dari elemen terakhir. Jika nilai ini tidak diatur, fungsi akan menghapus semua elemen, mulai dari posisi yang ditetapkan oleh parameter start.
> **array** ___Opsional___
> - Menentukan sebuah array dengan elemen-elemen yang akan dimasukkan ke dalam array asli. Jika hanya satu elemen, itu bisa berupa string, dan tidak perlu menjadi array.

array_sum()
------
> Mengembalikan jumlah dari nilai-nilai dalam sebuah array

Fungsi array_sum() mengembalikan jumlah dari semua nilai dalam sebuah array.

Syntax
> array_sum(array)
> 
> **array** ___Wajib___
> - Menentukan array yang akan dijumlahkan.

array_unique()
------
> Menghapus nilai-nilai duplikat dari sebuah array

Fungsi array_unique () menghapus nilai duplikat dari sebuah array. Jika dua atau lebih nilai array sama, penampilan pertama akan tetap dan yang lainnya akan dihapus.

Catatan: Array yang dikembalikan akan menjaga jenis kunci item array pertama.

Syntax
> array_unique(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan sebuah array
> **sorttype** ___Opsional___
> - Menentukan bagaimana cara membandingkan elemen / item array. Nilai yang mungkin:
> 	- **SORT_STRING** - **Default**. Membandingkan item sebagai string
> 	- **SORT_REGULAR** - Membandingkan item secara normal (tidak mengubah tipe)
> 	- **SORT_NUMERIC** - Membandingkan item secara numerik
> 	- **SORT_LOCALE_STRING** - Membandingkan item sebagai string, berdasarkan lokalisasi saat ini

array_values()
------
> Mengembalikan semua nilai dari sebuah array

Fungsi array_values () mengembalikan sebuah array yang berisi semua nilai dari sebuah array.

Tips: Array yang dikembalikan akan memiliki kunci numerik, dimulai dari 0 dan meningkat sebesar 1.

Syntax
> array_values (array)
> 
> **array** ___Diperlukan___
> - Menentukan sebuah array.

array_walk()
------
> Menerapkan sebuah fungsi buatan pengguna ke setiap anggota dari sebuah array

Fungsi array_walk () menjalankan setiap elemen array dalam fungsi yang ditentukan pengguna. Kunci dan nilai array adalah parameter dalam fungsi tersebut.

Catatan: Anda dapat mengubah nilai elemen array dalam fungsi yang ditentukan pengguna dengan menentukan parameter pertama sebagai referensi: &$value (Lihat Contoh 2).

Tip: Untuk bekerja dengan array yang lebih dalam (array di dalam array), gunakan fungsi array_walk_recursive ().

Syntax
> array_walk (array, myfunction, parameter...)
> 
> **array** ___Wajib___
> - Menentukan sebuah array
> **myfunction** ___Wajib___
> - Nama fungsi yang ditentukan pengguna
> **parameter,...** ___Optional___
> - Menentukan parameter untuk fungsi yang ditentukan pengguna. Anda dapat menugaskan satu parameter ke fungsi, atau sebanyak yang Anda inginkan.

array_walk_recursive()
------
> Menerapkan sebuah fungsi buatan pengguna secara rekursif ke setiap anggota dari sebuah array

Fungsi array_walk_recursive() menjalankan setiap elemen array dalam sebuah fungsi yang ditentukan oleh pengguna. Kunci dan nilai array adalah parameter dalam fungsi tersebut. Perbedaan antara fungsi ini dan fungsi array_walk() adalah bahwa dengan fungsi ini Anda bisa bekerja dengan array yang lebih dalam (array di dalam array).

Syntax
> array_walk_recursive(array, myfunction, parameter...)
> 
> **array** ___Wajib___
> - Menentukan array
> **myfunction** ___Wajib___
> - Nama fungsi yang ditentukan oleh pengguna
> **parameter,...** ___Opsional___
> - Menentukan parameter untuk fungsi yang ditentukan oleh pengguna. Anda dapat menetapkan satu parameter ke fungsi, atau sebanyak yang Anda inginkan.




# Membandingkan

array_diff()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya nilai)

Fungsi array_diff() membandingkan nilai dari dua (atau lebih) array, dan mengembalikan perbedaannya.

Fungsi ini membandingkan nilai dari dua (atau lebih) array, dan mengembalikan sebuah array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Syntax
> array_diff(array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Opsional___
> - Array lain untuk dibandingkan

array_udiff()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_udiff () membandingkan nilai dari dua atau lebih array, dan mengembalikan perbedaannya.

Catatan: Fungsi ini menggunakan fungsi yang ditentukan pengguna untuk membandingkan nilai!

Fungsi ini membandingkan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Syntax
> array_udiff(array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Opsional___
> - Array lain untuk dibandingkan
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi pembanding yang dapat dipanggil. Fungsi pembanding harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

array_diff_assoc()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai)

Fungsi array_diff_assoc () membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan perbedaan.

Fungsi ini membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Syntax
> array_diff_assoc (array1, array2, array3...)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.

array_diff_uassoc()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_diff_uassoc () membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan perbedaan.

Catatan: Fungsi ini menggunakan fungsi yang didefinisikan pengguna untuk membandingkan kunci!

Fungsi ini membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dst.

Syntax
> array_diff_uassoc (array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi pembanding yang dapat dipanggil. Fungsi pembanding harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

array_udiff_assoc()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai, menggunakan fungsi bawaan untuk membandingkan kunci dan fungsi pembanding nilai yang ditentukan pengguna)

Fungsi array_udiff_assoc () membandingkan kunci dan nilai dari dua atau lebih array, dan mengembalikan perbedaan.

Catatan: Fungsi ini menggunakan fungsi bawaan untuk membandingkan kunci, dan fungsi yang ditentukan pengguna untuk membandingkan nilai!

Fungsi ini membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Sintaks
> array_udiff_assoc (array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi perbandingan yang dapat dipanggil. Fungsi perbandingan harus mengembalikan bilangan bulat <, =, atau> dari 0 jika argumen pertama <, =, atau> dari argumen kedua.

array_udiff_uassoc()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan kunci dan nilai, menggunakan dua fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_udiff_uassoc() membandingkan kunci dan nilai dari dua atau lebih array, dan mengembalikan perbedaan.

Catatan: Fungsi ini menggunakan dua fungsi yang ditentukan oleh pengguna untuk perbandingan; kunci digunakan dalam fungsi pertama dan nilai digunakan dalam fungsi kedua!

Fungsi ini membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Syntax
> array_udiff_uassoc(array1, array2, array3, ..., myfunc_key, myfunc_value)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.
> **myfunc_key** ___Wajib___
> - Nama fungsi yang ditentukan oleh pengguna untuk membandingkan kunci array.
> 	Sebuah string yang mendefinisikan fungsi perbandingan yang dapat dipanggil. Fungsi perbandingan harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua
> **myfunc_value** ___Wajib___
> - Nama fungsi yang ditentukan oleh pengguna untuk membandingkan nilai array.
> 	Sebuah string yang mendefinisikan fungsi perbandingan yang dapat dipanggil. Fungsi perbandingan harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

array_diff_key()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya kunci)

Fungsi array_diff_key () membandingkan kunci dari dua (atau lebih) array, dan mengembalikan perbedaan.

Fungsi ini membandingkan kunci dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Syntax
> array_diff_key (array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.

array_diff_ukey()
------
> Membandingkan dua array, dan mengembalikan perbedaan (membandingkan hanya kunci, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_diff_ukey() membandingkan kunci dari dua (atau lebih) array, dan mengembalikan perbedaan.

Catatan: Fungsi ini menggunakan fungsi yang ditentukan pengguna untuk membandingkan kunci!

Fungsi ini membandingkan kunci dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang tidak ada di array2 atau array3, dll.

Syntax
> array_diff_ukey(array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi pembanding yang dapat dipanggil. Fungsi pembanding harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

array_intersect()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya nilai)

Fungsi array_intersect() membandingkan nilai dari dua (atau lebih) array, dan mengembalikan pasangan yang cocok.

Fungsi ini membandingkan nilai dari dua atau lebih array, dan mengembalikan array yang berisi entri dari array1 yang ada di array2, array3, dll.

Syntax
> array_intersect(array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Tidak wajib___
> - Array tambahan untuk dibandingkan

array_uintersect()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_uintersect () membandingkan nilai dari dua atau lebih array, dan mengembalikan nilai-nilai yang cocok.

Catatan: Fungsi ini menggunakan fungsi yang ditentukan pengguna untuk membandingkan nilai!

Fungsi ini membandingkan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang hadir di array2, array3, dll.

Syntax
> array_uintersect (array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array untuk dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array lain untuk dibandingkan.
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi pembanding yang dapat dipanggil. Fungsi pembanding harus mengembalikan integer <, =, atau> dari 0 jika argumen pertama <, =, atau> dari argumen kedua.

array_intersect_assoc()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai)

Fungsi array_intersect_assoc() membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan hasil yang cocok.

Fungsi ini membandingkan kunci dan nilai dari dua atau lebih array, dan mengembalikan array yang berisi entri dari array1 yang ada di array2, array3, dan seterusnya.

Syntax
> array_intersect_assoc(array1,array2,array3, ...)
> 
> **array1** ___Wajib___
> - Array pertama yang akan dibandingkan dengan yang lainnya
> **array2** ___Wajib___
> - Array yang akan dibandingkan dengan array pertama
> **array3,...** ___Opsional___
> - Array yang akan dibandingkan dengan array pertama

array_intersect_uassoc()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_intersect_uassoc () membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan kecocokan.

Catatan: Fungsi ini menggunakan fungsi yang ditentukan pengguna untuk membandingkan kunci!

Fungsi ini membandingkan kunci dan nilai dari dua atau lebih array, dan mengembalikan array yang berisi entri dari array1 yang ada di array2, array3, dll.

Syntax
> array_intersect_uassoc (array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array pertama yang akan dibandingkan dengan yang lainnya
> **array2** ___Wajib___
> - Array yang akan dibandingkan dengan array pertama
> **array3,...** ___Opsional___
> - Array yang akan dibandingkan dengan array pertama
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi perbandingan yang dapat dipanggil. Fungsi perbandingan harus mengembalikan bilangan bulat <, =, atau> dari 0 jika argumen pertama <, =, atau> dari argumen kedua.

array_uintersect_assoc()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai, menggunakan fungsi bawaan untuk membandingkan kunci dan fungsi pembanding nilai yang ditentukan pengguna)

Fungsi array_uintersect_assoc() membandingkan kunci dan nilai dari dua atau lebih array, dan mengembalikan hasil yang sama.

Catatan: Fungsi ini menggunakan fungsi bawaan untuk membandingkan kunci, dan fungsi yang ditentukan pengguna untuk membandingkan nilai!

Fungsi ini membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan array yang berisi entri dari array1 yang ada di array2, array3, dst.

Syntax
> array_uintersect_assoc(array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array yang akan dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Optional___
> - Array tambahan untuk dibandingkan
> **myfunction** ___Wajib___
> - String yang mendefinisikan fungsi pembanding yang dapat dipanggil. Fungsi pembanding harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

array_uintersect_uassoc()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan kunci dan nilai, menggunakan dua fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_uintersect_uassoc() membandingkan kunci dan nilai dari dua atau lebih array, dan mengembalikan hasil yang cocok.

Catatan: Fungsi ini menggunakan dua fungsi yang ditentukan oleh pengguna untuk perbandingan; kunci digunakan dalam fungsi pertama dan nilai digunakan dalam fungsi kedua!

Fungsi ini membandingkan kunci dan nilai dari dua (atau lebih) array, dan mengembalikan sebuah array yang berisi entri dari array1 yang ada di array2, array3, dan sebagainya.

Syntax
> array_uintersect_uassoc(array1, array2, array3, ..., myfunc_key, myfunc_value)
> 
> **array1** ___Wajib___
> - Array yang akan dibandingkan
> **array2** ___Wajib___
> - Array yang akan dibandingkan
> **array3,...** ___Opsional___
> - Array lain untuk dibandingkan
> **myfunc_key** ___Wajib___
> - Nama fungsi yang ditentukan oleh pengguna untuk membandingkan kunci array.
> 	Sebuah string yang mendefinisikan fungsi pemanggil perbandingan. Fungsi perbandingan harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua
> **myfunc_value** ___Wajib___
> - Nama fungsi yang ditentukan oleh pengguna untuk membandingkan nilai array.
> 	Sebuah string yang mendefinisikan fungsi pemanggil perbandingan. Fungsi perbandingan harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.


array_intersect_key()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya kunci)

Fungsi array_intersect_key () membandingkan kunci dari dua (atau lebih) array, dan mengembalikan hasil yang cocok.

Fungsi ini membandingkan kunci dari dua atau lebih array, dan mengembalikan array yang berisi entri dari array1 yang ada di array2, array3, dan seterusnya.

Syntax
> array_intersect_key(array1, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Array pertama yang akan dibandingkan dengan yang lainnya
> **array2** ___Wajib___
> - Array yang akan dibandingkan dengan array pertama
> **array3,...** ___Opsional___
> - Array yang akan dibandingkan dengan array pertama

array_intersect_ukey()
------
> Membandingkan dua array, dan mengembalikan kesamaan (membandingkan hanya kunci, menggunakan fungsi pembanding kunci yang ditentukan pengguna)

Fungsi array_intersect_ukey() membandingkan kunci dari dua (atau lebih) array, dan mengembalikan hasil yang sama.

Catatan: Fungsi ini menggunakan fungsi yang ditentukan pengguna untuk membandingkan kunci!

Fungsi ini membandingkan kunci dari dua atau lebih array, dan mengembalikan sebuah array yang berisi entri dari array1 yang hadir di array2, array3, dan seterusnya.

Syntax
> array_intersect_ukey(array1, array2, array3, ..., myfunction)
> 
> **array1** ___Wajib___
> - Array pertama yang akan dibandingkan dengan yang lainnya
> **array2** ___Wajib___
> - Array yang akan dibandingkan dengan array pertama
> **array3,...** ___Opsional___
> - Array yang akan dibandingkan dengan array pertama
> **myfunction** ___Wajib___
> - Sebuah string yang mendefinisikan fungsi pembanding yang dapat dipanggil. Fungsi pembanding harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

------

# Mengurutkan

array_multisort()
------
> Mengurutkan beberapa atau multidimensional array

Fungsi array_multisort() mengembalikan sebuah array yang telah diurutkan. Anda dapat menetapkan satu atau beberapa array. Fungsi tersebut mengurutkan array pertama, dan array lainnya mengikuti urutan tersebut, kemudian jika dua atau lebih nilai sama, fungsi tersebut mengurutkan array berikutnya, dan seterusnya.

Catatan: Kunci string akan dipertahankan, tetapi kunci numerik akan diindeks ulang, dimulai dari 0 dan meningkat sebesar 1.

Catatan: Anda dapat menetapkan parameter sortorder dan sorttype setelah setiap array. Jika tidak ditentukan, setiap parameter array menggunakan nilai **Default**.

Syntax
> array_multisort(array1, sortorder, sorttype, array2, array3, ...)
> 
> **array1** ___Wajib___
> - Menentukan sebuah array
> **sortorder** ___Opsional___
> - Menentukan urutan pengurutan. Nilai yang mungkin:
> 	- **SORT_ASC** - **Default**. Urutkan secara menaik (A-Z)
> 	- **SORT_DESC** - Urutkan secara menurun (Z-A)
> **sorttype** ___Opsional___
> - Menentukan tipe yang digunakan saat membandingkan elemen. Nilai yang mungkin:
> 	- **SORT_REGULAR** - **Default**. Bandingkan elemen secara normal (ASCII Standar)
> 	- **SORT_NUMERIC** - Bandingkan elemen sebagai nilai numerik
> 	- **SORT_STRING** - Bandingkan elemen sebagai nilai string
> 	- **SORT_LOCALE_STRING** - Bandingkan elemen sebagai string, berdasarkan konfigurasi wilayah saat ini (dapat diubah menggunakan setlocale())
> 	- **SORT_NATURAL** - Bandingkan elemen sebagai string menggunakan "urutan natural" seperti natsort()
> 	- **SORT_FLAG_CASE** - Dapat digabungkan (bitwise OR) dengan SORT_STRING atau SORT_NATURAL untuk mengurutkan string secara tidak peka terhadap huruf besar-kecil
> **array2** ___Opsional___
> - Menentukan sebuah array
> **array3** ___Opsional___
> - Menentukan sebuah array

natcasesort()
------
> Mengurutkan sebuah array menggunakan algoritma "natural order" yang tidak memperhatikan huruf besar atau kecil

Fungsi natcasesort() mengurutkan sebuah array dengan menggunakan algoritma "urutan alami". Nilai-nilai tetap mempertahankan kunci aslinya.

Dalam algoritma alami, angka 2 lebih kecil dari angka 10. Dalam pengurutan komputer, 10 lebih kecil dari 2, karena angka pertama dalam "10" lebih kecil dari 2.

Fungsi ini tidak bersifat case-sensitive.

Syntax
natcasesort(array)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan.

natsort()
------
> Mengurutkan sebuah array menggunakan algoritma "natural order"

Fungsi natsort () mengurutkan sebuah array dengan menggunakan algoritma "urutan alami". Nilai-nilai tetap mempertahankan kunci mereka yang asli.

Dalam algoritma alami, angka 2 lebih kecil dari angka 10. Dalam pengurutan komputer, 10 lebih kecil dari 2, karena angka pertama dalam "10" lebih kecil dari 2.

Syntax
> natsort(array)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan.

sort()
------
> Mengurutkan sebuah array indeks secara menaik

Fungsi sort() digunakan untuk mengurutkan array yang terindeks secara ascending (dari yang terkecil hingga terbesar).

Tips: Gunakan fungsi rsort() untuk mengurutkan array secara descending (dari yang terbesar hingga terkecil).

Syntax
> sort(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **sorttype** ___Opsional___
> - Menentukan cara untuk membandingkan elemen/item array. Nilai yang mungkin:
> 	- **0** = **SORT_REGULAR** - **Default**. Membandingkan item secara normal (tidak mengubah tipe data)
> 	- **1** = **SORT_NUMERIC** - Membandingkan item secara numerik
>  	- **2** = **SORT_STRING** - Membandingkan item sebagai string
> 	- **3** = **SORT_LOCALE_STRING** - Membandingkan item sebagai string, berdasarkan lokal saat ini
> 	- **4** = **SORT_NATURAL** - Membandingkan item sebagai string menggunakan urutan alami
> 	- **5** = **SORT_FLAG_CASE** - Membandingkan item sebagai string dengan memperhatikan huruf besar-kecil

asort()
------
> Mengurutkan sebuah array asosiatif secara menaik, berdasarkan nilai

Fungsi asort() mengurutkan array asosiatif secara menaik (ascending) berdasarkan nilai (value) dari elemen (item) array tersebut.

Tips: Gunakan fungsi arsort() untuk mengurutkan array asosiatif secara menurun (descending) berdasarkan nilai (value) dari elemen (item) array.

Tips: Gunakan fungsi ksort() untuk mengurutkan array asosiatif secara menaik (ascending) berdasarkan kunci (key) dari elemen (item) array.

Syntax
> asort(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **sorttype** ___Opsional___
> - Menentukan cara untuk membandingkan elemen/item array. Nilai yang mungkin:
> 	- **0** = **SORT_REGULAR** - **Default**. Membandingkan item secara normal (tidak mengubah tipe data)
> 	- **1** = **SORT_NUMERIC** - Membandingkan item secara numerik
>  	- **2** = **SORT_STRING** - Membandingkan item sebagai string
> 	- **3** = **SORT_LOCALE_STRING** - Membandingkan item sebagai string, berdasarkan lokal saat ini
> 	- **4** = **SORT_NATURAL** - Membandingkan item sebagai string menggunakan urutan alami
> 	- **5** = **SORT_FLAG_CASE** - Membandingkan item sebagai string dengan memperhatikan huruf besar-kecil

rsort()
------
> Mengurutkan sebuah array indeks secara menurun

Fungsi rsort() mengurutkan array yang diindeks secara menurun.

Tips: Gunakan fungsi sort() untuk mengurutkan array yang diindeks secara menaik.

Syntax
> rsort(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **sorttype** ___Opsional___
> - Menentukan cara untuk membandingkan elemen/item array. Nilai yang mungkin:
> 	- **0** = **SORT_REGULAR** - **Default**. Membandingkan item secara normal (tidak mengubah tipe data)
> 	- **1** = **SORT_NUMERIC** - Membandingkan item secara numerik
>  	- **2** = **SORT_STRING** - Membandingkan item sebagai string
> 	- **3** = **SORT_LOCALE_STRING** - Membandingkan item sebagai string, berdasarkan lokal saat ini
> 	- **4** = **SORT_NATURAL** - Membandingkan item sebagai string menggunakan urutan alami
> 	- **5** = **SORT_FLAG_CASE** - Membandingkan item sebagai string dengan memperhatikan huruf besar-kecil

usort()
------
> Mengurutkan sebuah array berdasarkan nilai menggunakan sebuah fungsi pembanding yang ditentukan pengguna

Fungsi usort() mengurutkan sebuah array berdasarkan nilai dengan menggunakan fungsi perbandingan yang ditentukan oleh pengguna.

Tips: Gunakan fungsi uksort() untuk mengurutkan array berdasarkan kunci dengan menggunakan fungsi perbandingan yang ditentukan pengguna.

Tips: Gunakan fungsi uasort() untuk mengurutkan array berdasarkan nilai (dan mempertahankan asosiasi indeks) dengan menggunakan fungsi perbandingan yang ditentukan pengguna.

Syntax
> usort(array, callback)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **callback** ___Wajib___
> - Fungsi perbandingan. Harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

ksort()
------
> Mengurutkan sebuah array asosiatif secara menaik, berdasarkan kunci

Fungsi ksort() digunakan untuk mengurutkan sebuah array asosiatif secara ascending (menaik), berdasarkan kunci (key) dari setiap elemen pada array.

Tips: Gunakan fungsi krsort() untuk mengurutkan array asosiatif secara descending (menurun), berdasarkan kunci (key).

Tips: Gunakan fungsi asort() untuk mengurutkan array asosiatif secara ascending (menaik), berdasarkan nilai (value) dari setiap elemen pada array.

Syntax
> ksort(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **sorttype** ___Opsional___
> - Menentukan cara untuk membandingkan elemen/item array. Nilai yang mungkin:
> 	- **0** = **SORT_REGULAR** - **Default**. Membandingkan item secara normal (tidak mengubah tipe data)
> 	- **1** = **SORT_NUMERIC** - Membandingkan item secara numerik
>  	- **2** = **SORT_STRING** - Membandingkan item sebagai string
> 	- **3** = **SORT_LOCALE_STRING** - Membandingkan item sebagai string, berdasarkan lokal saat ini
> 	- **4** = **SORT_NATURAL** - Membandingkan item sebagai string menggunakan urutan alami
> 	- **5** = **SORT_FLAG_CASE** - Membandingkan item sebagai string dengan memperhatikan huruf besar-kecil

krsort()
------
> Mengurutkan sebuah array asosiatif secara menurun, berdasarkan kunci

Fungsi krsort() mengurutkan sebuah array asosiatif secara menurun, berdasarkan kunci.

Tips: Gunakan fungsi ksort() untuk mengurutkan sebuah array asosiatif secara menaik, berdasarkan kunci.

Tips: Gunakan fungsi arsort() untuk mengurutkan sebuah array asosiatif secara menurun, berdasarkan nilai.

Syntax
> krsort(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **sorttype** ___Opsional___
> - Menentukan cara untuk membandingkan elemen/item array. Nilai yang mungkin:
> 	- **0** = **SORT_REGULAR** - **Default**. Membandingkan item secara normal (tidak mengubah tipe data)
> 	- **1** = **SORT_NUMERIC** - Membandingkan item secara numerik
>  	- **2** = **SORT_STRING** - Membandingkan item sebagai string
> 	- **3** = **SORT_LOCALE_STRING** - Membandingkan item sebagai string, berdasarkan lokal saat ini
> 	- **4** = **SORT_NATURAL** - Membandingkan item sebagai string menggunakan urutan alami
> 	- **5** = **SORT_FLAG_CASE** - Membandingkan item sebagai string dengan memperhatikan huruf besar-kecil

uksort()
------
> Mengurutkan sebuah array berdasarkan kunci menggunakan sebuah fungsi pembanding yang ditentukan pengguna

Fungsi uksort() mengurutkan sebuah array berdasarkan kunci menggunakan sebuah fungsi perbandingan yang ditentukan oleh pengguna.

Tips: Gunakan fungsi uasort() untuk mengurutkan sebuah array berdasarkan nilai (dan mempertahankan asosiasi indeks) dengan menggunakan sebuah fungsi perbandingan yang ditentukan oleh pengguna.

Tips: Gunakan fungsi usort() untuk mengurutkan sebuah array berdasarkan nilai menggunakan sebuah fungsi perbandingan yang ditentukan oleh pengguna.

Syntax
> uksort(array, callback)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan.
> **callback** ___Wajib___
> - Sebuah fungsi perbandingan. Harus mengembalikan nilai integer <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.

arsort()
------
> Mengurutkan sebuah array asosiatif secara menurun, berdasarkan nilai

Fungsi arsort () mengurutkan array asosiatif secara menurun, sesuai dengan nilai.

Tip: Gunakan fungsi asort () untuk mengurutkan array asosiatif secara menaik, sesuai dengan nilai.

Tip: Gunakan fungsi krsort () untuk mengurutkan array asosiatif secara menurun, sesuai dengan kunci.

Syntax
> arsort(array, sorttype)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **sorttype** ___Opsional___
> - Menentukan cara membandingkan elemen / item array. Nilai yang mungkin:
> 	- **0** = **SORT_REGULAR** - **Default**. Bandingkan item secara normal (tidak mengubah tipe)
> 	- **1** = **SORT_NUMERIC** - Bandingkan item secara numerik
> 	- **2** = **SORT_STRING** - Bandingkan item sebagai string
> 	- **3** = **SORT_LOCALE_STRING** - Bandingkan item sebagai string, berdasarkan bahasa lokal saat ini
> 	- **4** = **SORT_NATURAL** - Bandingkan item sebagai string menggunakan pengurutan alami
> 	- **5** = **SORT_FLAG_CASE** - Bandingkan item sebagai string dengan memperhatikan huruf besar atau kecil.

uasort()
------
> Mengurutkan sebuah array berdasarkan nilai menggunakan sebuah fungsi pembanding yang ditentukan pengguna dan mempertahankan asosiasi indeks

Definisi dan Penggunaan
Fungsi uasort() mengurutkan sebuah array berdasarkan nilai menggunakan fungsi perbandingan yang ditentukan oleh pengguna dan menjaga asosiasi indeks.

Tip: Gunakan fungsi uksort() untuk mengurutkan sebuah array berdasarkan kunci menggunakan fungsi perbandingan yang ditentukan oleh pengguna.

Tip: Gunakan fungsi usort() untuk mengurutkan sebuah array berdasarkan nilai menggunakan fungsi perbandingan yang ditentukan oleh pengguna.

Syntax
> uasort(array, callback)
> 
> **array** ___Wajib___
> - Menentukan array yang akan diurutkan
> **callback** ___Wajib___
> - Fungsi perbandingan. Harus mengembalikan bilangan bulat <, =, atau > dari 0 jika argumen pertama <, =, atau > dari argumen kedua.







compact()
------
> Membuat sebuah array yang berisi variabel-variabel dan nilai-nilainya

Definisi dan Penggunaan
Fungsi compact() membuat sebuah array dari variabel dan nilainya.

Catatan: Semua string yang tidak cocok dengan nama variabel akan dilewati.

Syntax
> compact(var1, var2...)
> 
> **var1** ___Wajib___
> - Bisa berupa string dengan nama variabel, atau array dari variabel
> **var2,...** ___Opsional___
> - Bisa berupa string dengan nama variabel, atau array dari variabel. Beberapa parameter diizinkan.

range()
------
> Membuat sebuah array yang berisi rentang elemen

Definisi dan Penggunaan
Fungsi range() menciptakan sebuah array yang berisi rentang elemen.

Fungsi ini mengembalikan sebuah array dari elemen-elemen dari yang terendah hingga yang tertinggi.

Catatan: Jika parameter low lebih tinggi dari parameter high, array rentang akan dari yang tertinggi ke yang terendah.

Sintaks
> range(low, high, step)
> 
> **low** ___Wajib___
> - Menentukan nilai terendah dari array
> **high** ___Wajib___
> - Menentukan nilai tertinggi dari array
> **step** ___Opsional___
> - Menentukan penambahan yang digunakan dalam rentang. **Default** adalah 1.

key()
------
> Mengambil sebuah kunci dari sebuah array

Fungsi key() mengembalikan kunci elemen dari posisi penunjuk internal saat ini.

Fungsi ini mengembalikan FALSE jika terjadi kesalahan.

Sintaks
> key(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

each()
------
> Ditolak dari PHP 7.2. Mengembalikan pasangan kunci dan nilai saat ini dari sebuah array

Fungsi each() mengembalikan kunci dan nilai elemen saat ini, dan menggerakkan penunjuk internal maju.

Catatan: Fungsi each() sudah tidak digunakan lagi pada PHP 7.2.

Kunci dan nilai elemen ini dikembalikan dalam bentuk array dengan empat elemen. Dua elemen (1 dan Nilai) untuk nilai elemen, dan dua elemen (0 dan Kunci) untuk kunci elemen.

Syntax
> each(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

extract()
------
> Mengimpor variabel-variabel ke dalam tabel simbol saat ini dari sebuah array

Fungsi extract() mengimpor variabel ke dalam tabel simbol lokal dari sebuah array.

Fungsi ini menggunakan kunci array sebagai nama variabel dan nilai sebagai nilai variabel. Untuk setiap elemen, fungsi ini akan membuat variabel di tabel simbol saat ini.

Fungsi ini mengembalikan jumlah variabel yang diekstrak pada saat berhasil.

Syntax
> extract(array, extract_rules, prefix)
> 
> **array** ___Wajib___
> - Menentukan array yang akan digunakan
> **extract_rules** ___Opsional___
> - Fungsi extract() memeriksa untuk nama variabel yang tidak valid dan tabrakan dengan nama variabel yang sudah ada. Parameter ini menentukan bagaimana nama yang tidak valid dan tabrakan diperlakukan.
> 	- Nilai yang mungkin:
> 	- **EXTR_OVERWRITE** - **Default**. Pada tabrakan, variabel yang sudah ada akan ditimpa
> 	- **EXTR_SKIP** - Pada tabrakan, variabel yang sudah ada tidak akan ditimpa
> 	- **EXTR_PREFIX_SAME** - Pada tabrakan, nama variabel akan diberi awalan
> 	- **EXTR_PREFIX_ALL** - Semua nama variabel akan diberi awalan
> 	- **EXTR_PREFIX_INVALID** - Hanya nama variabel yang tidak valid atau numerik yang akan diberi awalan
> 	- **EXTR_IF_EXISTS** - Hanya menimpa variabel yang sudah ada di tabel simbol saat ini, jika tidak, tidak melakukan apa-apa
> 	- **EXTR_PREFIX_IF_EXISTS** - Hanya menambahkan awalan pada variabel jika variabel yang sama sudah ada di tabel simbol saat ini
> 	- **EXTR_REFS** - Mengekstrak variabel sebagai referensi. Variabel yang diimpor masih merujuk pada nilai parameter array
> **prefix** ___Opsional___
> - Jika **EXTR_PREFIX_SAME**, **EXTR_PREFIX_ALL**, **EXTR_PREFIX_INVALID** atau **EXTR_PREFIX_IF_EXISTS** digunakan pada parameter **extract_rules**, awalan tertentu diperlukan.
> 	- Parameter ini menentukan awalan. Awalan secara otomatis dipisahkan dari kunci array oleh karakter garis bawah.

in_array()
------
> Memeriksa apakah sebuah nilai tertentu ada dalam sebuah array

Definisi dan Penggunaan
Fungsi in_array() mencari nilai tertentu dalam sebuah array.

Catatan: Jika parameter pencarian adalah string dan parameter tipe diatur ke TRUE, pencarian akan mempertimbangkan perbedaan huruf besar dan kecil.

Syntax
> in_array(pencarian, array, tipe)
> 
> **pencarian** ___Wajib___
> - Menentukan nilai yang akan dicari
> **array** ___Wajib___
> - Menentukan array yang akan dicari
> **tipe** ___Opsional___
> - Jika parameter ini diatur ke TRUE, fungsi in_array() akan mencari string pencarian dan tipe yang spesifik dalam array.

list()
------
> Memberikan nilai-nilai variabel seolah-olah mereka adalah sebuah array

Definisi dan Penggunaan
Fungsi list() digunakan untuk menetapkan nilai ke daftar variabel dalam satu operasi.

Catatan: Sebelum PHP 7.1, fungsi ini hanya berfungsi pada array numerik.

Syntax
> list(var1, var2, ...)
> 
> **var1** ___Wajib___
> - Variabel pertama untuk menetapkan nilai
> **var2,...** ___Opsional___
> - Lebih banyak variabel untuk menetapkan nilai

count()
------
> Mengembalikan jumlah elemen dalam sebuah array

Fungsi count() mengembalikan jumlah elemen dalam sebuah array.

Syntax
> count(array, mode)
> 
> **array** ___Wajib___
> - Menentukan array
> ***mode** ___opsional___
>  - Menentukan mode. Nilai yang mungkin:
> 	- **0** - **Default**. Tidak menghitung semua elemen dalam array multidimensi
> 	- **1** - Menghitung array secara rekursif (menghitung semua elemen dalam array multidimensi)

sizeof()
------
> Alias dari count()

Definisi dan Penggunaan
Fungsi sizeof() mengembalikan jumlah elemen dalam sebuah array.

Fungsi sizeof() adalah alias dari fungsi count().

Syntax
> sizeof(array, mode)
> 
> **array** ___Wajib___
> - Menentukan array
> **mode** ___Pilihan___
> - Menentukan mode. Nilai yang mungkin:
> 	- **0** - **Default**. Tidak menghitung semua elemen dari array multidimensi
> 	- **1** - Menghitung array secara rekursif (menghitung semua elemen dari array multidimensi)

current()
------
> Mengembalikan elemen saat ini dari sebuah array

Fungsi current() mengembalikan nilai elemen saat ini dalam sebuah array.

Setiap array memiliki penunjuk internal ke "elemen saat ini", yang diinisialisasi dengan elemen pertama yang dimasukkan ke dalam array.

Tips: Fungsi ini tidak memindahkan penunjuk internal array.

Sintaks
> current(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

pos()
------
> Alias dari current()

Fungsi pos() mengembalikan nilai elemen saat ini dalam sebuah array.

Fungsi ini merupakan alias dari fungsi current().

Setiap array memiliki penunjuk internal ke elemen "saat ini", yang diinisialisasi ke elemen pertama yang dimasukkan ke dalam array.

Tips: Fungsi ini tidak memindahkan penunjuk internal array.

Sintaks
> pos(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

end()
------
> Mengatur pointer internal dari sebuah array ke elemen terakhirnya

Fungsi end() memindahkan penunjuk internal ke, dan mengeluarkan, elemen terakhir dalam array.

Sintaks
> end(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

next()
------
> Maju ke elemen berikutnya dari sebuah array

Fungsi next() memindahkan penunjuk internal ke, dan mengeluarkan, elemen berikutnya dalam array.

Sintaks
> next(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

prev()
------
> Mundurkan pointer internal sebuah array

Fungsi prev() memindahkan pointer internal ke elemen sebelumnya dalam array dan mengeluarkan nilainya.

Syntax
> prev(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

reset()
------
> Mengatur pointer internal dari sebuah array ke elemen pertamanya

Fungsi reset() digunakan untuk memindahkan penunjuk internal pada elemen pertama dalam sebuah array.

Syntax
> reset(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan

shuffle()
------
> Mengacak sebuah array

Fungsi shuffle() mengacak urutan elemen dalam sebuah array.

Fungsi ini memberikan kunci baru untuk setiap elemen dalam array. Kunci yang sudah ada akan dihapus.

Syntax
> shuffle(array)
> 
> **array** ___wajib___
> - Menentukan array yang akan digunakan