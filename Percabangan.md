# Percabangan 
Percabangan dalam java adalah dimana kita punya lebih dari satu kondisi kita, percabangan bisa kita sebut dengan control flow statement,karna tugas utamanya adalah mengatur alur program

## if then
if then adalah percabangan yang paling dasar dan simple
contoh
	int i= 0;
	if(i == 0){
		System.out.println("Buka pintu")
	}

Untuk setiap perintah di dalam if then kita harus menulis nya di dalam sebuah curly bracket `{}`

##if else
if else digunakan ketika kita ingin memasang nilai default jika kondisi yang di minta tidak ada

contoh

		int i= 0;
	if(i == 0){
		System.out.println("Buka pintu");
	}else {
		System.out.print("Pintu rusak");
	}

## else if
else digunakan ketika kita punya lebih dari suatu kondisi
contoh

		int i= 0;
	if(i == 0){
		System.out.println("Buka pintu");
	}else if(i != 0){
		System.out.print("Tutup pintu");
	}else {
		System.out.print("Pintu rusak");
	}
## switch case
Selain if then ada percabangan lain yang kita bisa gunakan yaitu switch case

contoh

	int i = 8;
	switch(i){
		case 3:
			System.out.print("angka 3");
		break;

		case 8:
			System.out.print("angka 8")
		break;

		default :
			System.out.print("tidak ada angka");

	}

dalam penggunaan switch case kita harus menulis break setelah case agar jika java sudah menemukan kondisi yang minta java tidak akan mejalankan kode lain yang ada di bawah nya.