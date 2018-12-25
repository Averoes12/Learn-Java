# Array 
Array adalah sebuah tempat untuk menyimpan kumpulan data yang tipenya sama

## Pembuatan array

cara buat array ada dua cara

`tipeData [] namaVariable = new tipeData[jumlahArray];`
`tipeData [] namaVariable = {isi, array};`

contoh

`int [] umur = new int[5];`
`String [] nama = new String {"nama", "saya", "kepo"};`

## Penggunaan array 
jika kita ingin menggunakan array kita harus mengisi array nya dulu

perlu diingat bahwa array dimulai dari nol
	int [] umur = new int[5];
	umur [0] = 12;
	umur [1] = 15;
	umur [2] = 18;
	umur [3] = 20;
	umur [4] = 23;
	umur [5] = 25;

dalam penggunaan array looping sangat berguna untuk pengisian array 

	for(int x = 0; x < 4; x++){
		umur[x] x + 1;
	}

`x < 4` angka 4 disini bisa kita ganti dengan `arr.length`, .length adalah methode untuk menghitung panjang array.

## Akses array
Setelah kita membuat array kita akan mengakses array
kita akan akses array yang kita buat sebelumnya.

contoh

	int [] umur = new int[5];
	umur [0] = 12;
	umur [1] = 15;
	umur [2] = 18;
	umur [3] = 20;
	umur [4] = 23;

	System.out.print(umur[0]);
	System.out.print(umur[1]);
	System.out.print(umur[2]);
	System.out.print(umur[3]);
	System.out.print(umur[4]);

kita juga bisa memanfaatkan looping untuk mengakses array

	for (int x = 0; x < 4; x++){
		System.out.println(umur[x]);
	}


# Array 2D
Array 2 Dimensi adalah ketika ada array di dalam array jadi 
contoh 

`{{12,13,16},{10,19,13}}`

array bisa memiliki lebih dari satu dimensi karna itu array memiki sifat multi dimensional.

## Buat array 2D

	String [][] arr2D = new String [2][2];

	arr2D[0][0] = "Kayu";
	arr2D[0][1] = "Kursi";
	arr2D[1][0] = "Besi";
	arr2D[1][1] = "Sendok";

Pada [] yang pertama adalah baris
Pada [] yang kedua adalah kolom

kita juga bisa membuat array 2D dengan cara yang lain

	String [][] arr2D = new String [][]{{Kayu","Besi"},{"Rumah","Sendok"}};

# Menampilkan array 2D

cara menampilkan array 2D juga berbeda dengan array biasa

	System.out.print(arr2D[0][0]);
	System.out.print(arr2D[0][1]);
	System.out.print(arr2D[1][0]);
	System.out.print(arr2D[1][1]);

# IndexOutOf Bounds
IndexOutOf Bounds adalah pesan error yang disampaikan oleh java saat kita mengakses index array yang tidak ada pada array tersebut,Maka dari itu saat kita mengakses index array kita harus lebih berhati-hati.

