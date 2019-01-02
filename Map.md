# Map 
Map adalah class yang berguna untuk membuat list juga sama seperti List dan Set akan tetapi Map tidak menggunakan index untuk mengurutkannya,Map menggunakan *key dan values*.

Kita bisa mengatur sendiri key nya bisa integer atau string, jadi ibarat kita memproduksi suatu barang dan di barang tersebut ada kode produksinya dan nama barangnya.

Map Mempunyai 3 class :

1. HashMap

HashMap menampilkan data secara acak 

contoh 

	import java.util.HashMap;
	import java.util.Map.Entry;

	public class Map {
	
	public static void main(String [] args) {
		//Map punya 3 class ==> HashMap LinkedHashMap TreeMap
		
		//kita buat HashMap
		
		HashMap<String, String> produksi = new HashMap<String, String>();
		
		//untuk memasukkan datanya kita butuh method put
		
		produksi.put("bc001" , "Brownies Coklat");
		produksi.put("bm001", "Brownies Matcha");
		produksi.put("bk001", "Brownies Keju");
		
		//kita akan menampilkannya dengan for
		
		//kita perlu menggunakan rumus
		//tipeData namaBaru : namaMap.entrySet()
		for(Entry<String, String> brownies : produksi.entrySet()) {//tipe data datanya adalah entry lalu entrySet digunakan untuk mengambil data 
			
			System.out.println("Kode Produksi : " + brownies.getKey() +" Nama Barang : " + brownies.getValue());
			
			
			}
		
		
		}
	}

Hasil Output

	Kode Produksi : bm001 Nama Barang : Brownies Matcha
	Kode Produksi : bc001 Nama Barang : Brownies Coklat
	Kode Produksi : bk001 Nama Barang : Brownies Keju

2. LinkedHashMap

LinkedHashMap menampilkan data secar urut sesuai dengan yang kita masukkan

contoh 

	import java.util.*;
	import java.util.Map.Entry;

	public class Map {
	
	public static void main(String [] args) {
		//Map punya 3 class ==> HashMap LinkedHashMap TreeMap
		
		//kita buat HashMap
		
		LinkedHashMap<String, String> produksi = new LinkedHashMap<String, String>();
		
		//untuk memasukkan datanya kita butuh method put
		
		produksi.put("bc001" , "Brownies Coklat");
		produksi.put("bm001", "Brownies Matcha");
		produksi.put("bk001", "Brownies Keju");
		
		//kita akan menampilkannya dengan for
		
		//kita perlu menggunakan rumus
		//tipeData namaBaru : namaMap.entrySet()
		
		for(Entry<String, String> brownies : produksi.entrySet()) {//tipe data datanya adalah entry lalu entrySet digunakan untuk mengambil data 
			
			System.out.println("Kode Produksi : " + brownies.getKey() +" Nama Barang : " + brownies.getValue());
			
			
			}
		
		
		}
	}

Hasil Output 

	Kode Produksi : bc001 Nama Barang : Brownies Coklat
	Kode Produksi : bm001 Nama Barang : Brownies Matcha
	Kode Produksi : bk001 Nama Barang : Brownies Keju

3. TreeMap

TreeMap akan menampilkan data sesuai dengan urutan abjad atau angka dan disini TreeMap akan mengurutkan Key nya bukan values nya.

	import java.util.*;
	import java.util.Map.Entry;

	public class Map {
	
	public static void main(String [] args) {
		//Map punya 3 class ==> HashMap LinkedHashMap TreeMap
		
		
		TreeMap<String, String> produksi = new TreeMap<String, String>();
		
		//untuk memasukkan datanya kita butuh method put
		
		produksi.put("bc001" , "Brownies Coklat");
		produksi.put("bm001", "Brownies Matcha");
		produksi.put("bk001", "Brownies Keju");
		
		//kita akan menampilkannya dengan for
		
		//kita perlu menggunakan rumus
		//tipeData namaBaru : namaMap.entrySet()
		
		for(Entry<String, String> brownies : produksi.entrySet()) {//tipe data datanya adalah entry lalu entrySet digunakan untuk mengambil data 
			
			System.out.println("Kode Produksi : " + brownies.getKey() +" Nama Barang : " + brownies.getValue());
			
			
			}
		
		
		}
	}

Hasil Output

	Kode Produksi : bc001 Nama Barang : Brownies Coklat
	Kode Produksi : bk001 Nama Barang : Brownies Keju
	Kode Produksi : bm001 Nama Barang : Brownies Matcha




