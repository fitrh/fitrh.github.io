# Tugas Praktikum : Data Definition Language

1. Buatlah 2 Buah Table dengan nama ```table_mahasiswa``` dan ```table_matakuliah``` dengan ketentuan berikut :   
	1. ```table_mahasiswa``` memiliki *field* awal sebagai berikut :   
		| table_mahasiswa |     | table_matakuliah |
		| --------------- | --- | ---------------- |
		| ```id_mhs```    |     | `id_mk`             |
		| ```nim_mhs```   |     |                  |
		| ```nama_mhs```  |     |                  |

	2. Setiap `table`, Salah satu dari *field*nya harus ada yang menjadi `PRIMARY KEY`.
	3. *Field* `nim` memiliki panjang maksimal 10 dan harus bersifat `UNIQUE`.
	4. Tambahkan *field* baru pada `table_mahasisw` dengan nama ```status_mhs``` yang hanya boleh menampung nilai ```Aktif``` dan ```Lulus```.
	5. Tambahkan *field* baru pada `table_matakuliah` dengan nama `kode_mk`, `nama_mk`, `sks_mk`.
	6. *Field* `sks_mk` hanya boleh menampung nilai 2, 3, dan 4.
	7. Ubahlah nama `table_mahasiwa` dan `table_matakuliah` menjadi `tb_mahasiswa` dan `tb_matakuliah`.
	8. Ubahlah nama *field* pada kedua `table` sehingga tidak lagi memiliki suffiks `_mhs` dan `_mk`.

	Ketentuan diatas dijalankan secara berurutan dari 1 - 8.
2. Buatlah Sebuah `database` dengan struktur `table` berikut :
   