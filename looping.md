# Perulangan 
Perulangan juga disebut sebgagai looping,berguna ketika ingin menulis suatu kode secara berulang tanpa harus menulis nya berulang kali
## for
kita bisa menggunakan metode for untuk melakukan looping
contoh
	int i = 0;
	for (iint i= 0; i < 3; i++){
		System.out.print("Repeat me");
}

`i = 0` kita memberi tahu bahwa kita mulai nya dari angak nol.

`i < 3` kita memberi batasan dari suatu looping

`i++` kita menentukan aksi terhadap perulangan,disini kita menambahkan satu point daru setiap perulangan.

## for bersarang 
for bersarang atau for nested adalah dimana ketika ada for didalam for, jadi for bisa melakukan pengulangan terhadap dirinya sendiri.

contoh 

	int l = 10;
	for (int i = 0; i < l; i++){
		for (int j = 0; j < i; j++){
			System.out.print("*");
		}
		System.out.print("");
	}

## while
Selain for ada juga metode looping yang lain yaitu while

contoh

	int no = 0;

		while(no <= 6){
			System.out.println(no);
			no++;
		}

## do while 
do while sama seperti while,akan tetapi pengecekan kondisi nya dilakukan terakhir,jadi metode ini akan menjalankan perintah tersebut satu kali

contoh

		int no = 0;

		do{
			System.out.println(no);
			no++;
		}while(no <= 6);

