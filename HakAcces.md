# Jenis-jenis hak akes dalam java

Hak akses terbagi jadi dua

1. Hak akses Modifier

2.  Hak akses non Modifier

## 1. Hak akses modifier

Hak akses ini punya 4 jenis 

1. Public 
Public bisa di akses dari mana saja baik dari luar paket maupun dari dalam class

2. Proteced 
Protected Bisa di akses dari dalam class, dari paket yang sama, dan dari luar paket, akan tetapi jika kita ingin mengakes dari luar paket syaratnya class yang ada didalam paket tersebut harus merupakan class child dari class yang di proctected.

3. Default 
Default sama seperti Protected akan tetapi tidak bisa di akses dari luar class.

4.Private
Private hanya bisa diakses oleh class nya sendiri.

========================================  
Hak Akses|Class|Paket|Class Child|World|
========================================
Public   |Yes  |Yes  |Yes        |Yes  |
=========|=====|=====|===========|=====|
Protected|Yes  |Yes  |Yes        |No   |
=========|=====|=====|===========|=====|
Default  |Yes  |Yes  |No         |No   |
=========|=====|=====|===========|=====|
Private  |Yes  |No   |No         |No   |
========================================

## 2. Hak akses non modifier

1. static
Static adalah hak akses yang digunakan untuk mendefinisikan suatu variable atau yang method.
Jadi jika menggunakan static maka kita tidak harus membuat instance cukup langsung memanggil nama methodnya.

2. final
final adalah hak akses yang sudah tidak dapat di rubah lagi,final punya tiga macam hak akses

- hak akses pada variable = variable tidak dapat di rubah lagi.

- hak akses pada method = method tidak dapat di override atau diturunkan pada class child.

- hak akses pada class = class tidak dapat di jadikan class parent(induk).

3. transient
transient adalah hak akses yang berhubungan dengan proses serialisasi, proses serialisasi digunakan untuk di konversi ke byte agar dapat di tranmusikan.




