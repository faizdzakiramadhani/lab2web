faiz dzaki ramadhani
312210223
# lab2web

# 1. Membuat dokumen HTML

![gambar1](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/e2fc0446-438a-455e-a72a-e0e10d7e2e8f)


# 2. Mendeklarasikan CSS Internal

![gambar2](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/a395b075-8f86-4fec-86fe-7ae62e48a6d3)


# 3. Menambahkan Inline CSS

![gambar3](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/35ef131c-1b27-43e3-a41f-a1b4f91ec13b)


# 4. Membuat CSS Eksternal

![gambar4](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/307535cd-e0d6-48dd-b9e7-c8a261a40cb2)



# 5. Menambahkan CSS Selector

![gambar5](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/137a42c0-8d9d-4f0b-b0f5-c8a584e191be)

# 6. validasi dokumen css

![gambar6](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/1ac7f2b0-7b12-46b1-b1ad-0ca289278d02)



# Pertanyaan dan Tugas

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

jawaban: 

![gambar7](https://github.com/faizdzakiramadhani/lab2web/assets/115913915/cf286f12-6855-479c-a1cd-2a3a72741fc8)


2. Apa perbedaan pendeklarasian CSS elemen `h1` `{...}` dengan #intro `h1` `{...}`? berikan
penjelasannya!

jawaban:

Berikut adalah penjelasan perbedaannya:

`h1` `{...}`:

- Pendeklarasian ini akan mempengaruhi semua elemen `<h1>` di seluruh halaman web.
  
- Ini adalah contoh dari pemilihan elemen berdasarkan jenisnya `(tag selector)`. 

- Ini akan mengubah semua elemen `<h1>` di halaman tanpa memandang di mana elemen-elemen tersebut berada dalam struktur dokumen HTML.

Contoh penggunaannya adalah jika Anda ingin mengubah gaya teks semua elemen `<h1>` di seluruh situs web, seperti mengubah warna teks, ukuran font, atau gaya lainnya secara konsisten.

#intro `h1` `{...}`:

- Pendeklarasian ini akan mempengaruhi elemen `<h1>` yang berada dalam elemen dengan id "intro".
  
- Ini adalah contoh dari pemilihan elemen berdasarkan hierarki atau "nested selector".
  
- Ini akan mengubah gaya elemen `<h1>` yang berada dalam elemen dengan id "intro" saja.
  
Contoh penggunaannya adalah jika Anda memiliki elemen `<h1>` yang hanya ingin Anda ubah gayanya ketika elemen tersebut berada dalam konteks elemen dengan id "intro". Ini memungkinkan Anda untuk memberikan gaya khusus pada elemen tersebut dalam konteks tertentu.


3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!

jawaban:

etika Anda memiliki deklarasi CSS yang dideklarasikan secara internal `(di dalam tag `<style>` dalam elemen `<head>`)`, CSS eksternal `(di dalam file eksternal dengan ekstensi .css)`, dan CSS inline `(langsung dalam atribut style elemen HTML yang bersangkutan)` yang mempengaruhi elemen yang sama, prinsip "specificity" dan urutan pengaturan akan mempengaruhi deklarasi mana yang akan ditampilkan oleh browser.

Contoh:

`<p id="paragraf" class="teks-merah" style="color: blue;">`Ini adalah teks paragraf.`</p>`

Dan ada CSS yang terkait:

CSS Internal:

`<style>`
  p `{
    color: green;
  }`
`</style>`

CSS Eksternal `(styles.css)`:

.teks-merah `{
  color: red;
}`


4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! `( `<p id="paragraf-1" class="text-paragraf">` )`

jawaban:

Ketika sebuah elemen HTML memiliki baik ID maupun Class, deklarasi CSS yang akan ditampilkan oleh browser akan dipengaruhi oleh kombinasi dari keduanya. Namun, perlu diingat bahwa ID 

memiliki prioritas yang lebih tinggi daripada Class. Berikut adalah penjelasan lebih lanjut dan contohnya:

`<p id="paragraf-1" class="text-paragraf">`Ini adalah teks paragraf.`</p>`

Jika ada deklarasi CSS sebagai berikut:

#paragraf-1 `{
  color: red;
}`

.text-paragraf `{
  color: blue;
}`

alam kasus ini, deklarasi CSS dengan ID selector `(#paragraf-1)` akan memiliki prioritas tertinggi. Oleh karena itu, warna teks paragraf ini akan menjadi merah, sesuai dengan deklarasi color: red;. Deklarasi CSS dengan class selector `(text-paragraf)` akan diabaikan dalam hal ini karena ID selector memiliki prioritas yang lebih tinggi.

Jadi, pada elemen HTML `<p id="paragraf-1" class="text-paragraf">`, deklarasi CSS yang akan ditampilkan adalah color: red; karena ID selector `(#paragraf-1)` memiliki prioritas yang lebih tinggi daripada class selector `(text-paragraf)`.
