# Inner Class

Inner Clas adalah class yang ada di dalam class,dan sebuah inner class tidak bisa di akses langsung oleh class yang ada di luarnya,akan tetapi inner class dapat mengakses private acces modifier.

kita buat inner class

	package innerClass;

	class luar {

		//kita buat objek di class luar

			Private String brand = "SevenCloth";

			
			}
		class dalam{

			//lalu kita buat methode di dalam class dalam untuk mengakses objek yang ada di class luar

			void brand() {

				System.out.println("Brand Baju : " + brand);
		}
	}

	//lalu kita buat main class untuk menampilkan yang telah kita buat
	class main{
		
		public static void main (String [] args){

			/*kita tidak bisa membuat objek langsung dari class dalam, maka dari itu kita harus menambahkan objek pada class luar agar bisa di akses di class main*/ 
		}

	}

Menambahkan objek pada class luar 

	class luar {

		//kita buat objek di class luar

			Private String brand = "SevenCloth";

			
			}
		class dalam{

			//lalu kita buat methode di dalam class dalam untuk mengakses objek yang ada di class luar

			void brand() {

				System.out.println("Brand Baju : " + brand);
		}

		void show(){

		dalam show = new dalam();

		show.dalam();

		}
	}

jika sudah buat maka kita bisa mengakses inner class

		class main{
		
		public static void main (String [] args){

			luar brand = new luar();

			show.luar();
		}

	}

