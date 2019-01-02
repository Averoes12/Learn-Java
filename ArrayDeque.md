# Array Deque

Array Deque adalah class yang paling bebas atau flexible karna class ini memilki hampir semua method yang ada pada class lain, dan class ini memiliki method yang paling banyak.

# Method Array Deque

- .peekFirst(); melihat data yang paling pertama.

- .peekLast(); melihat data yang paling terakhir

- .addFirst(); menambah data yang paling pertama.

- .addLast(); menambah data yang paling terakhir.

- .poolFirst();

- .pollLast();

- .getFirst();

- .getLast();

dan masih banyak methode lainnya yang bisa di lihat di link berikut.

https://docs.oracle.com/javase/7/docs/api/java/util/Deque.html

cara penggunaannya 

import java.util.ArrayDeque;
import java.util.Iterator;


	public class Dequeue {
	
	public static void main(String[] args) {
		
		ArrayDeque<String> warna = new ArrayDeque<String>(); 
		
		warna.addLast("Torquise");
		warna.push("Coral");
		warna.add("Silver");
		warna.addFirst("Cyan");
	
		
		Iterator<String> it = warna.iterator();
		
		System.out.println("Pick Color :");
		
		while(it.hasNext()) {
			System.out.println(it.next());
			}
		}

	}

Hasil output

	Pick Color :
	Cyan
	Coral
	Torquise
	Silver
