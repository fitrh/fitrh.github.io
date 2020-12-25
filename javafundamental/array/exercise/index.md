# Latihan : _Array_

1. Buatlah Sebuah Program untuk mencetak elemen array char dalam bentuk kode desimal sesuai pada tabel ASCII !
	Contoh
		
		Array Char	:
			char[] chars = {'A', 'B', 'C'};
		
		Output		:
			{65, 66, 67}

2. Buatlah Sebuah Program yang memiliki 2 buah Array char a dan b, kemudian tukarlah nilai elemen-elemennya,
   jika kedua array memiliki panjang yang berbeda, maka nilai yang tertukar hanya sampai elemen indeks terakhir array terpendek, !

   Contoh 1
		
		Array Char	:
			char[] a = {'F', 'I', 'T'};
			char[] b = {'R', 'A', 'H'};

		Output		:
			A : {F, I, T}
			B : {R, A, H}

			A <-> B

			A : {R. A, H}
			B : {F, I, T}

	Contoh 2

		Array Char	:
			char[] a = {'I', 'L', 'K', 'O', 'M'};
			char[] b = {'2', '0', '1', '9'};

		Output		:
			A : {I, L, K, O, M}
			B : {2, 0, 1, 9}

			A <-> B

			A : {2, 0, 1, 9, M}
			B : {I, L, K, O}

3. Modifikasi program soal nomor 2 sehingga array char a dan b dapat ditukar nilainya tanpa menggunakan array tambahan !

