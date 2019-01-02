# Inheritance 

Inheritance adalah salah satu bentuk hubungan antar class, didalam java masing class bisa saling berhubungan salah satu bentuknya adalah inherintance yaitu pewarisan.

Class bisa membuat Subclass sendidri dan bisa memasukkan method yang ada di dalam Class ke dalam Subclass, jadi didalam java ada Parent Class dan Child Class, Parent class adalah induknya dan Child Class adalah Subclass nya atau keturunannya.

untuk membuat sebuah Child Class kita perlu menggunakan kata *extends* 

contoh

misal kita punya class yang bernama Child

lalu kita buat class Parent didalam class child tersebut

	class Parent {

		//Isi dari class
	}

agar kita bisa menajankan method yang ada padda class Parent kita harus menemabahkan kata 
*extends*

	public class Child extends Parent{

		public static void main(String[] args){// yag akan dijalankan oleh java adalah yang punya method main

		}
	}

Kita juga bisa memasukkan method yang ada pada class Parent ke dalam class Child dengan menngunakan method overriding
Overriding method adalah method yang digunakan untuk memasukkan method yang ada dalam Parent class ke dalam Child class

Contoh 

	class ParentClass {

		String ayah() {
			System.out.println("Ayah");
		
			return "";
		}
	
	 	String ibu() {
		
			System.out.println("Ibu");
		
			return "";
		}
	
		void nama() {
		
		}
	}

	public class ChildClass extends ParentClass  {
		
		@Override
		public String ayah() {
			System.out.println("Ayah : 'I'm in Child Class'");
			
			return "";
		}
		
		public String ibu() {
			
			System.out.print("Ibu : 'i'm in Child Class'");
			
			return "";
		}
		
	
		public static void main(String[] args) {
				
				ChildClass ayah = new ChildClass();
				ChildClass ibu = new ChildClass();
				
				ayah.ayah();
				ibu.ibu();			}
				
		}


# Rule of Overriding 

Method Overriding tidak bisa dijalankan jika method yang ada pada Parent class bersifat static

Pada method Overriding kita bisa menngunakan Private acces modifier pada method yang di Parent class nya.


# Polimorphism 

Polimorphism adalah perubahan bentuk,kita bisa meubah isi dari suatu method dengan polimorphism

contoh 

		public static void main(String[] args) {
				
				ParentClass ayah = new ParentClass();
				ParentClass ibu = new ChildClass();// ini adalah contoh polimorphism (perubahan bentuk )
				
				ayah.ayah();
				ibu.ibu();			
			}
				
		}

Pada contoh di atas isi dari ParentClass pada saat ouput akan berubah isinya menjadi isi dari Child Class.