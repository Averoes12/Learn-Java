#Interface 
Interface mirip sebuah class akan tetapi interface tidak memiliki atribut class dan method nya di tulis tanpa ada isinya
interface berfungsi untuk meyimpan method kosong dan atribut yang bersifat final atau sudah tidak bisa diganti, interface juga tidak memilki body 
Untuk memasukkan interface ke dalam class kita harus memberi kata kunci "implement" 
contoh

	public class BukuBagus implement buku {

	}

Di dalam interface variable memiliki atribut final sehingga tidak bisa di rubah lagi

Jika suatu class tidak dapat di extend lebih dari satu class child, interface bisa punya lebih dari turunan.
di dalam interface juga tidak ada instance dan constructornya kosong.

contoh interface

Petama kita buat interface terlebih dahulu di sebuah packet

Klik kanan pada **src** pilih new ==> **package** lalu isi namanya

Setelah itu kita buat interface di dalam packet tersebut 

Klik kanan pada paket yang telah kita buat pilih new ==> **interface** isi nama sesuka hati

lalu kita isikan pada interface method yang ingin kita jalankan

contoh
		package interfaces;

		public interface Learn {	

		 public String id();
		}
	package executor;
	import interfaces.Learn;

Setelah itu kita buat class baru untuk menjalankan method yang telah kita buat 

lalu kita isi method yang telah di buat pada interface ke dalam class tersebut

agar interface bisa kita panggil kita harus menngunakan kata *implements* 

kita juga butuh method overriding agar method yang ada di interface dapat di turunkan pada class

	public class executor implements Learn{
	
		@Override
		public String id() {
			String name = "Daff";
			int code = 1705;
			System.out.print(name + " your code is "+ code);
			return "";

		}//Setelah kita mengisi method kita harus membuat method main agar bisa dijalankan
			
			public static void main(String[] args) {
				
				executor Learn = new executor();//Kata Learn Bisa diganti karna itu adalah nama variable
				
				System.out.print(Learn.id());
			}
}

