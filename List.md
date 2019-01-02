# List 
	List fungsinya smaa seperti array,setiap data yang kita masukkan akan mempunyai nilai index berdasarkan urutan objek yang kita masukkan,List adalah sebuah interface dan salah satu bentuk implementasinya adalah ArrayList samasperti array akan tetapi arraylist lebih mudah dari array.

## Array List 

array list memiliki performa yang baik saat digunakan untuk mencari data.

	contoh 

		int [] numb = new int[2];

		numb[0] = 1;
		numb[1] = 2;
		//dalam array jika memasukkan data yang tidak sesuai dengan jumlahnya maka akan menampilkan pesan errorOutOfBounds
		numb[2] = 3;

akan tetapi jika kia memakai arraylist tidak akan terjadi error seperti itu karna lebih flexible,arraylist juga bisa menggabungkan tipe data 

contoh 
	
		List mobil = new ArrayList();

		mobil.add(2);//method add() untuk menambah list 
		mobil.add("Vechile");
		mobil.add(1);
		mobil.add("tier");//kita bisa menambahkan list lagi 

Akan tetapi cara menampilkan arraylist berbeda kita menampilkan nya perlu atribute for
contoh 

		for(int i = 0; i < mobil.size(); i++){method size() untuk mendapatkan banyak index yang kita buat

			System.out.println("Mobil ini butuh " + mobil.get(i));

		}//method get() untuk melihat isi dari list yang kita buat,huruf i disitu adalah nomer indexnya
		

dalam penulisan array list ada dua cara ini cara yang kedua

kita bisa langsung memasukkan semua data ke dalam array list

	//kita gunakan addAll

	List mobil = new ArrayList();

	mobil.addAll(Arrays.asList(2, "Vechile", 1, "tier"));


contoh array list
	//kita perlu meng import class dari collection

	import java.util.ArrayList;
	import java.util.List;

	public class Collection {

    public static void main(String[] args) {
        //kita akan membuat arraylist

        List warna = new ArrayList();

        warna.add("merah");
        warna.add("putih");
        warna.add("briu");
        warna.add("Kuning");


        //kita panggil arraylist yang telah kita buat


        for(Object color : warna){

        	System.out.println(color);
        }	

        //atau kita bisa menggunakan

        for (int i = 0; i < warna.size(); i++) {

            System.out.println("Kita Punya Warna " + warna.get(i));
        }

    }

 Hasil output 

 	Kita Punya Warna merah
	Kita Punya Warna putih
	Kita Punya Warna briu
	Kita Punya Warna Kuning

## Linked List

Linked List memiki performa yang baik saat digunakan untuk meng input data atau menghapus data
Penggunaan Linked List sama dengan array list tidak ada yang membedakan yang beda hanya dari segi performa nya saja.

# Mtehod Pada List

List punya method tersendiri 

`.remove();` untuk menghapus data.
`.set();` untuk merubah data.
`.removeAll();` untuk menghapus semua data.
`.get();` untuk mengamnbil data.


