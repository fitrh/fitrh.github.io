# Tugas Pendahuluan : _Array_

0. Jelaskan Apa yang dimaksud dengan Array pada Bahasa Pemrograman dan Perbedaannya dengan Tipe Data Primitif serta tuliskan cara-cara untuk mendeklarasikan Array pada Java!  

1. Jelaskan Apa yang dimaksud dengan ```ArrayIndexOutOfBoundsException``` pada Java dan tuliskan masing-masing 1 (satu) contoh program untuk mencegah atau mengatasinya dengan  :  
    - Menggunakan Percabangan Kondisi
    - Menggunakan _Try Catch_
    - Menggunakan Perulangan
    - Tanpa Menggunakan Ketiga Konsep Sebelumnya  

2. Jelaskan Apa itu ```For-Each```, dan tuliskan contoh program untuk mengakses elemen array 2 dimensi menggunakan ```For-Each``` !  

3. Tuliskan Contoh Program, dimana didalamnya terdapat array String yang menampung nim, nama asisten, dan nama-nama teman satu asistensi anda dengan ketentuan  :  
    - NIM dan Nama asisten anda berada pada indeks ke-0
	- Indeks selanjutnya berisi NIM dan Nama teman anda
	- Tampilkan isi Array anda sebagai berikut :  
 
		![alt text][01_list]
	- Menu *view* menerima inputan ```int n``` dimana ```n``` adalah nomor urut sesuai *list*, jika ```n``` tidak menghasilakn ```ArrayIndexOutOfBoundsException```, maka cetak NIM, Nama, dan Status dengan format berikut :  
		
		![alt text][02_list]  
	Jika ```n``` adalah nomor urut asisten anda, maka pada Status cetak **Asisten**, selain itu, cetak **Praktikan**.
	- Program akan berhenti jika ```n``` menghasilkan ```ArrayIndexOutOfBoundsException``` dan akan mencetak **Exit . . .** .  

		![alt text][03_list]  

		![alt text][04_list]

[01_list]: assets/img/01_list.png "Tampilan List"
[02_list]: assets/img/02_view.png "Tampilan Jika Inputan adalah Nomor urut Asisten"
[03_list]: assets/img/03_view.png "Tampilan Jika Inputan adalah nomor urut teman"
[04_list]: assets/img/04_exit.png "Tampilan Ketika ArrayIndexOutOfBoundsException"
