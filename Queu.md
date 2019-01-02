# Queue
Queue adalah sebuah class yang sama seperti Array List untuk mengurutkan data akan tetapi di queue tidak ada method set dan get, di class queue punya prinsip First In First Out jadi siapa yang pertama kali masuk adalah yang pertama kali keluar sama seperti antrian tidak bisa menyelak.

misal kita buat list warna dengan queue

	import java.util.Iterator;
	import java.util.PriorityQueue;

	public class Queu {
	 
	public static void main(String[] args) {
		
		PriorityQueue<String> warna = new PriorityQueue<String>();
		
		warna.add("coral blue");
		warna.add("gold sand");
		warna.add("Rose gold");
		warna.add("Navy Blue");
		
		//System.out.println("peek " + warna.peek());//peek mengambil data yang pertama kali dioutpun kan
		System.out.println("Pooling " + warna.poll());//berguna untuk mengambil dan menghapus data
		//kita tampilkan menggunakan iterator
		
		Iterator<String> it = warna.iterator();
		
		System.out.println("Choose your color :");
		
		while(it.hasNext()) {
			System.out.println(it.next());
			}
		
		
		}
	}


 Di Dalam Queue terdapat beberapa method 

 - `.contains(data)` berguana untuk mengecek sebuah data
 		
 		if(data.contains("ada")){

 		System.out.print("ada");

 	}

 - `.peek(data)` berguna untuk mengambil data tapi tidak menghapus dari antrian

 		System.out.println("Peek " + warna.peek());

Hasil output

		peek Navy Blue
		Choose your color :
		Navy Blue
		Rose gold
		coral blue
		gold sand

 		//peek mengambil data yang pertama di outpun kan

 - `.poll(data)` berguna untuk mengambil dan menghapus data yang di antrian 

 		System.out.println("Pooling " + warna.poll());

Maka Hasil output nya

	Pooling Navy Blue
	Choose your color :
	Rose gold
	gold sand
	coral blue

