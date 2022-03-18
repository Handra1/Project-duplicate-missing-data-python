# Project-duplicate-missing-data-python
This project about duplicate and missing data in python (In Indonesia)

Salah satu masalah ketika kita ingin melakukan cleaning data adalah duplicate data. Tentu saja hal ini akan berpengaruh untuk melakukan analisis data.
Kita dapat menggunakan method drop_duplicates() jika terjadi duplicate data. Dengan menggunakan method drop_duplicates() maka data atas nama Daniel yang sebelumnya duplicate akan ditampilkan hanya 1 kali saja.
Terdapat kolom total_bill, top, sex, smoker, day / week, day dan size of the party. Dapat kita lihat bahwa terdapat NaN missing values.
Kita dapat menggunakan method info() untuk menghitung NaN missing values.
Untuk data yang kita miliki sekarang, terdapat 5 entries tetapi tidak ada kolom yang memiliki non-null values. Artinya kita memiliki missing value di semua kolom tersebut.
Untuk menghapus missing values pada dataframes, kita dapat menggunakan method dropna().
Sekarang kita hanya  memiliki 2 entries saja setelah menghapus data jika terdapat missing values tersebut. Namun jika kita menggunakan cara ini untuk melakukan analisis, maka kita akan kehilangan 40% data tersebut. Maka kita akan menggunakan method fillna() untuk mengisi nilai yang hilang tersebut.

Fill missing values with .fillna() :
Dengan menggunakan method fillna() maka tidak akan ada lagi output NaN missing values dan akan digantikan dengan string yang kita inputkan pada method fillna().
Contoh yang lain misalnya memberikan nilai 0 untuk kolom total_bill dan size jika disana terdapat NaN missing values.
Dapat kita lihat jika kolom total_bill sekarang sudah tidak memiliki NaN missing values pada index ke-1 nya.
Kelebihan ketika kita sudah memiliki clean data adalah mempermudah kita dalam melakukan perhitungan statistik. Misalnya disini saya ingin menghitung nilai mean dari kolom total_bill.
Maka kita akan langsung mendapatkan hasilnya ketika sudah mempunyai data yang sudah rapi dan tidak ada NaN missing values.
