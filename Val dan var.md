# Val dan var

Val dan Var adalah tempat untuk menyimpan data.

## Val

Semua data yang di simpan di dalam val tidak bisa di rubah karna data tersebut sudah final jadi tidak bisa di rubah lagi

contoh penggunaan Val

	val nama = "Daff"

	print(nama)

Output 

	Daff

jika kita mengubah isi variable yang ada di val maka akan error

	val nama = "Daff"
    
    nama = "dafa"

	print(nama)
Output 

	error: val cannot be reassigned
    nama = "dafa"
    		^

## var 

Data yang di simpan didalam var masih bisa di rubah lagi.

contoh var

	var nama = "Daff"

    nama = "dafa"

	print(nama)

Output

	dafa

data yang ada dalam variable var masih bisa dirubah lagi.