# Set 

Set sama dengan List akan tetapi set tidak bisa menyimpan objek yang sama berkali-kali, set juga tidak menyimpan objek yang kita masukkan secara urut.

Set memiliki 3 class :

1. HashSet 

Data yang ditampilkan oleh HashSet tidak urut dengan yang kita masukkan,dan di dalam HashSet tidak ada method set dan get
perfirma nya cepat.

		HashSet <String> warna = new HashSet<String>();// kita harus import class HashSet dulu
		
		warna.add("tosqa");
		warna.add("aquablue");
		warna.add("blueSaphire");
		
		
		//kita tampilkan dengan iterator
		
		Iterator<String> it = warna.iterator();
		
		System.out.print("Pilihan warna : \n");
		
		while (it.hasNext()) {
			
			
			System.out.println(it.next());
		}

Hasil outputnya 

	Pilihan warna : 
	blueSaphire
	aquablue
	tosqa


2. LinkedHashSet

Data yang ditampilkan akan diurutkan sesuai dengan yang kita masukkan 
performanya hampir sama dengan HashSet.

		LinkedHashSet <String> warna = new LinkedHashSet<String>();//kita harus import LinkedHashSet dulu
		
		warna.add("tosqa");
		warna.add("aquablue");
		warna.add("blueSaphire");
		
		
		//kita tampilkan dengan iterator
		
		Iterator<String> it = warna.iterator();
		
		System.out.print("Pilihan warna : \n");
		
		while (it.hasNext()) {
			
			
			System.out.println(it.next());
		}

Hasil output

	Pilihan warna : 
	tosqa
	aquablue
	blueSaphire

3. TreeSet

TreeSet akan mengurutkan data yang kita masukkan sesuai dengan urutan alphabet atau sesua dengan urutan angka sebelum ditampilkan.

performa dari TreeSet terbilang lambat karna dia harus mengurutkan terlebih dulu sesua abjad.

		TreeSet <String> warna = new TreeSet<String>();//Kia harus import class TreeSet dulu
		
		warna.add("tosqa");
		warna.add("aquablue");
		warna.add("blueSaphire");
		
		
		//kita tampilkan dengan iterator
		
		Iterator<String> it = warna.iterator();
		
		System.out.print("Pilihan warna : \n");
		
		while (it.hasNext()) {
			
			
			System.out.println(it.next());
		}

Hasil output 

	Pilihan warna : 
	aquablue
	blueSaphire
	tosqa


