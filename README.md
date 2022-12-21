# Ujian Akhir Semester

<br> Mata Kuliah  : Dasar Pemograman
<br> Nama         : Anissya Auliani Supriadi Putri
<br> NIM          : 1227050023
<br> Jurusan      : Teknik Informatika UIN Sunan Gunung Jati Bandung



# Deskripsi Umum

Tema utama dari source code yang satu ini adalah untuk membuat array 2 dimensi menggunakan bahasa C++.
Tujuan utama dari source code ini adalah mengubah letak nilai yang tadinya sebuah baris menjadi sebuah kolom, begitupun sebaliknya.
<br> Algoritma dari Source code ini yaitu :
<br> 1.User menginputkan berapa banyak baris pada array.
<br> 2.User menginputkan berapa banyak kolom dari baris pada array.
<br> 3.User menginputkan satu persatu nilai array,dimulai dari baris 1 dan kolom 1.
<br> 4.Jika sudah,Nilai dalam array tersebut di tampilkan sesuai aturan matriks.
<br> 5.Lalu ditampilkan juga nilai dalam array yang sudah dibalik,dari baris menjadi kolom dan sebaliknya.



# Source Code

#include <iostream>
using namespace std;

int main(){
	int input [100][100];
	int baris, kolom, a, k;
	
	cout <<"Masukan Jumlah Baris : ";
	cin >> baris;
	cout <<"Masukan Jumlah Kolom : ";
	cin >> kolom;
	cout << endl;
	
	for (a = 0; a < baris; a++){
		for (k = 0; k < kolom; k++){
			cout << " Baris " << a+1 << " kolom " << k+1 << " = ";
			cin >> input[a][k];
		}
		cout << endl;
	}
	
	cout << "Hasil : " << endl;
	
	for (a = 0; a < baris; a++){
		for (k = 0; k < kolom; k++){
			cout << " " << input[a][k];
		}
		cout << endl;
	}
	
	cout << "=================================" << endl;
	
	for (a = 0; a < kolom; a++){
		for (k = 0; k < baris; k++){
			cout << " " << input[k][a];
		}
		cout << endl;
	}
}



# Output

![image](https://user-images.githubusercontent.com/119275711/208843612-1102fa93-4217-40d1-b16a-718dfda44154.png)
