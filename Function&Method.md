# Method dan Function

Method atau function adalah serangkaian program yang dibuat dalam sebuah block dan dapat di jalankan dengan memanggilnya,Method dan Function memiliki nilai balik.
Nilai balik adalah hasil dari program yang kita buat didalamm sebuah block yang dikembalikan oleh sebuah function 
Jika sebuah Method atau Function tidak memiliki milai balik di sebut dengan procedural, Pada dasarnya sebuah method atau function mempunyai nilai balik atau nilai return.

Method adalah fungsi yang berada dalam sebuah class

# Procedural 
Procedural adalah sebutan untuk fungsi yang tidak memiliki nilai balik,dan biasanya ditandai dengan katak kunci *void*.

# Pembuatan fungsi

	static typeDataHasil namaFungsi(){
		//Isi dari fungsi
	}

- static adalah kata kunci yang digunakan agar sebuah fungsi dapat dipanggil tanapa harus membuat instance dari suatu objek.
- typeDataHasil adalah jenis dari hasil yang dikembalikkan setelah fungsi dijalankan, yaitu *return*.\
- namaFungsi nama dari fungsi yang kita buat,penulisannya biasanya kata pertamanya huruf kecil dan kata kedua diawali dengan huruf besar.

# Memanggil fungsi
Ada dua cara dalam memanggil fungsi

1. Jika kita membuat fungsi dengan kata kunci *static* maka kita bisa langsung memanggilnya, contoh:
		public static void Function(){
		

		luasKubus();//kita bisa memanggil function yang telah kita buat
	}
	
	

	 static void luasKubus() { // contoh function
		
		Scanner s = new Scanner(System.in);
		
		System.out.println("Masukkan nilai");
		
		int luasKubus = s.nextInt();
		
		int total = 6 * luasKubus * luasKubus;
		System.out.print(total);
	}

2. Jika kita membuat fungsi tanpa kata kunci *static* kita harus memasukkan nama objek nya, contoh:
		public static void Function(){

		Kubus luas = new Kubus ();

		luas.luasKubus();//kita bisa memanggil function yang telah kita buat
	}
	
	

	 	void luasKubus() { // contoh function
		
		Scanner s = new Scanner(System.in);
		
		System.out.println("Masukkan nilai");
		
		int luasKubus = s.nextInt();
		
		int total = 6 * luasKubus * luasKubus;
		System.out.print(total);
	}

# Fungsi yang punya nilai balik
Agar sebuah fungsi memiliki suatu nilai balik maka kita harus menggunakan kata *return*.
cara penulisannya 

static tipedata namaFungsi(tipeData namaVariable){
	//isi fungsi
	return;
}

contoh

	static int luasKubus(int sisi){
		int luas = 6 * sisi * sisi;
		return luas;
	}

Fungsi diatas menggunakan parameter
Parameter adalah sebuah variable yang menampung nilai untuk diproses dalam sebuah fungsi, parameter berperan sebagai fungsi.

# Methode Overloading

Kita bisa membuat method dengan nama yang sama dalam satu kelas akan tetapi parameternya harus berbeda, konsep ini disebut dengan methode overloading.

