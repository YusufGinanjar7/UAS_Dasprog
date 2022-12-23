# Ujian Akhir Semester
<br>Mata Kuliah   : Dasar Pemrograman
<br>Nama           : Yusuf Ginanjar
<br>NIM            : 1227050136
<br>Jurusan        : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/)

## Deskripsi Umum
Tugas akhir mata kuliah dasar pemrograman untuk membuat inputan untuk banyaknya baris dan kolom,
mengisi nilainya dan menukar kolom jadi baris, baris menjadi kolom. pada array 2 dimensi angka yang
sudah diinput, akan menampilkan bilangan bilangan yang habis dibagi 3, 5, dan 7.

## Source Code
    #include <iostream>
    using namespace std;

    int main(){
	
    cout << "Nama 	: Yusuf Ginanjar"<<endl;
    cout << "NIM	: 1227050136"<<endl;

	int a, b, c, l;
	int matriks [50][50], transpose [50][50];
	cout << "======================================"<<endl;
	cout << "Masukkan Jumlah Banyaknya Baris :" <<endl;
	cin >> c;
	cout << "======================================"<<endl;
	cout << "Masukkan jumlah banyaknya kolom :" <<endl;
	cin >> l;
	cout << "======================================"<<endl;
	
	cout << "Masukkan nilai :"<<endl;
	for (a = 0; a < c; a++){
    for (b = 0; b < l; b++){
    	 cout <<"("<<a<<","<<b<<") : ";
      cin  >> matriks[a][b];
    }
    }
    cout << endl;
    cout << "Hasil nilai matriks : " <<endl;
    for (a = 0; a < c; a++){
    for (b = 0; b < l; b++){
    	cout << matriks[a][b] << " ";
    }
    cout << endl;
    }
    cout << endl;

    for (a = 0; a < c; a++){
    for (b = 0; b < l; b++){
      transpose[b][a] = matriks[a][b];
    }
    }
  
    cout << "Hasil pengubahan Transpose :" <<endl;
    for (a = 0; a < l; a++){
    for (b = 0; b < c; b++){
      cout << transpose[a][b] << " ";
    }
    cout << endl;
    }
    cout << "-----------------------------------" <<endl;
	cout << "Nilai yang Habis dibagi 3, 5, dan 7 : "<<endl;
	for(a=0; a<c; a++){
		for(b=0; b<l; b++){
			if(matriks[a][b]%3 == 0 && matriks[a][b]%5 == 0 && matriks[a][b]%7 ==0 ){
				cout<< "Nilai " << matriks[a][b] << " : 3 = " << matriks [a][b]%3<<endl;
				cout<< "Nilai " << matriks[a][b] << " : 5 = " << matriks [a][b]%5<<endl;
				cout<< "Nilai " << matriks[a][b] << " : 7 = " << matriks [a][b]%7<<endl;
				cout<< " "<<endl;
		}
		}
	}	
	cout << "-----------------------------------" <<endl;
	}

## Output 
  ![image](https://user-images.githubusercontent.com/119514056/209346456-79e2efc4-53cb-4c28-929e-3f459b52ea86.png)
