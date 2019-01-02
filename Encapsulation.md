# Encapsulation

Encasulation proses ketika class yang kita buat bisa dugnakan oleh class lain tapi tidak bisa dirubah, encapsulation berguna untuk melindungi codingan kita agar tidak di bisa di rubah oleh siapapun.

contoh

Untuk menggunakan Encapsulation kita perlu menggunakan methode set dan get

- set untuk merubah variable atau men setting nya
- get untuk mengambil variable nya.

Petama kita butuh dua class agar bisa saling berhubungan 

Kita buat class main untuk menjalankan kode nya

	package Executor;
	
	public class Executor {

    public static void main(String[] args) {

    	}

	}

Setelah itu kita buat class yang akan kita enkapsulasi,dan kita mulai buat programnya

	public class Encapsulation {

    private String name = "Daff"; // objek harus di private agar tidak bisa di rubah
    private int code = 1705;

    //lalu kita buat public method

    public String getNama(){//


        return name;
    }

    public int getCode() {

        return code;
    }

    public  void setNama() {

        this.name = name;//kata this di sini mendefinisikan bahwa kita ingin mengakses variable yang ada di class ini.
    }

    public void	 setCode() {

        this.code =code;
    	}
	}

Setelah kita membuat program nya, kita jalankan programnya pada class main

   		
   	 public static void main(String[] args) {

        Encapsulation id = new Encapsulation();//kita beri objek dengan nama class yang kita enkapsulasi

        id.setNama();
        id.setCode();

        System.out.println("Your id " + id.getNama() + " " + id.getCode());

    }

dari kode diatas akan menghasilkan kode di atas 

	
	Your id Daff 1705

	Process finished with exit code 0



