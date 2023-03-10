# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: M Galang Pangestu NH
<br>NIM		: 1227050066
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
1).Untuk mencetak matrix transpose, Anda bisa menggunakan loop dan operator cout. Berikut ini adalah langkah-langkah umum yang dapat Anda ikuti:
Buat sebuah array multidimensi untuk menyimpan matrix yang ingin ditranspose.
Buat sebuah loop untuk mengelilingi setiap element dalam matrix tersebut.
Dalam loop tersebut, salin nilai dari setiap element ke posisi baris dan kolom yang berlawanan di dalam matrix transpose. Misalnya, jika element saat ini berada di baris ke-2 dan kolom ke-3, maka element tersebut harus disalin ke posisi baris ke-3 dan kolom ke-2 di dalam matrix transpose.
Buat sebuah loop lain untuk mencetak setiap element dalam matrix transpose. Anda bisa menggunakan operator cout dengan format "cout << element << " ";". Ingat untuk menambahkan baris baru setelah setiap baris dari matrix transpose selesai dicetak.

2).Untuk membuat program yang mencetak bilangan yang habis dibagi 3, 5, dan 7, Anda bisa menggunakan loop dan operator modulus. Berikut ini adalah langkah-langkah umum yang dapat Anda ikuti:
Tentukan batas atas dari rentang bilangan yang akan dicetak. Misalnya, jika Anda ingin mencetak bilangan yang habis dibagi 3, 5, atau 7 hingga 1000, maka batas atasnya adalah 1000.
Buat sebuah loop yang akan mengelilingi setiap bilangan dalam rentang tersebut.
Dalam loop tersebut, cek apakah bilangan tersebut habis dibagi 3, 5, atau 7 dengan menggunakan operator modulus. Anda bisa menggunakan if statement dengan format "if (bilangan % 3 == 0 || bilangan % 5 == 0 || bilangan % 7 == 0) {...}".
Jika bilangan tersebut habis dibagi 3, 5, atau 7, maka cetak bilangan tersebut dengan menggunakan operator cout dengan format "cout << bilangan << endl;".
## Source Code
1).Mencari Matrix Transpose



	#include<iostream>
	#include<iomanip>
	using namespace std;

	int main(){

		int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

		cout<< "=======================================\n";
		cout<< "Program Mencetak Matrix Transpos\n";
		cout<< "=======================================\n";
		cout<< "Nama  : M Galang Pangestu NH\n";
		cout<< "Nim   : 1227050066\n";
		cout<< "Kelas : Informatika - B\n\n";

	    cout<<"Input jumlah baris: "; cin>>jumlahBaris;
	    cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
	    cout << endl;

	    for(i = 0; i < jumlahBaris; i++){
		for(j = 0; j < jumlahKolom; j++){
		    cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
		    cin >> arr[i][j];
		}
		cout << endl;
	    }
	    cout << "Hasil matriks: " << endl;

	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
		cout << setw(3) << arr[i][j] << " ";
	    }
	    cout << endl;
	    }

	    baris = jumlahBaris;
	    kolom = jumlahKolom;

	    jumlahKolom = baris;
	    jumlahBaris = kolom;

	    cout << "\nUbah kolom jadi baris dan baris jadi kolom: " << endl;

	    for(i = 0; i < jumlahBaris ; i++){
		for(j = 0; j < jumlahKolom; j++){
		cout << setw(3) << arr[j][i] << " ";
	    }
	    cout << endl;
	    }
		return 0;
	}
2).Membuat program bilangan yang habis dibagi 3,5,7

	

	#include <iostream>
	#include <iomanip>
	using namespace std;
	int main(){

		int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

		cout<< "==============================================\n";
		cout<< "Program Bilangan Yang Habis Dibagi 3, 5, dan 7\n";
		cout<< "==============================================\n";
		cout<< "Nama  : M Galang Pangestu NH\n";
		cout<< "Nim   : 1227050066\n";
		cout<< "Kelas : Informatika - B\n\n";

	    cout<<"Input jumlah baris: "; cin>>jumlahBaris;
	    cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
	    cout << endl;

	    for(i = 0; i < jumlahBaris; i++){
		for(j = 0; j < jumlahKolom; j++){
		    cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
		    cin >> arr[i][j];
		}
		cout << endl;
	    }

	    cout << "Hasil input nilai : " << endl;

	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
		cout << setw(3) << arr[i][j] << " ";
	    }
	    cout << endl;
	    }

	    cout << "\nHasil bilangan yang habis dibagi 3,5,7 : " << endl;

	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
		if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
		cout << setw(3) << arr[i][j] << " ";
		}
	    }
	    cout << endl;
	    }


	    cout << endl;
	    return 0;
	}
## Output
![Screenshot_20221219_190826](https://user-images.githubusercontent.com/121006608/208424471-702d0d62-26e0-40b3-b240-98fde1cfb1f5.png)
![Screenshot_20221219_191042](https://user-images.githubusercontent.com/121006608/208424543-cb53e406-00da-43d4-889f-bc8a75c6f522.png)

