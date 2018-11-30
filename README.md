# praktikum6

 
## latihan **menggunakan header untuk mengabungka fungsi void**
**Alur Algoritma**
1. mulai program fungsi dengan menggunakan void
2. deklarasiakan terlebihdahulu fungsi yang ingin kita masukan ke header di satu file
3. masukan file tadi ke header yang ingin kita buat
4. kemudian panggil semua data tadi yang sudah di buat di foder yang berbeda kedalam pusat project yang,
yang ingin kita buat jalan kan project itu dengan menggunakan fungsi juga 
5. run project jika tidak ada kendala atau eror
5. end


**Kode Program**
##Header 
```
#ifndef KALKULATOR_H_INCLUDED
#define KALKULATOR_H_INCLUDED
int kali(int, int);
double bagi(int, int);
int tambah(int, int);
int kurang(int, int);


#endif // KALKULATOR_H_INCLUDED
##isi
```
#include<iostream>
using namespace std;

int kali(int a, int b){
return a*b;
}

double bagi(int a, int b){
return a/b;
}

int tambah(int a, int b){
return a+b;
}

int kurang(int a, int b){
return a-b;
}

##utama
```
#include<iostream>
#include"kalkulator.h"

using namespace std;

int inputData(string v="a");

int main(int argc, char const *argv[])
{
    int a, b;
    a = inputData();
    b = inputData("b");

    cout << "\nHasil perkalian axb adalah: " << kali(a,b);
    cout << "\nHasil pembagian a/b adalah: " << bagi(a,b);
    cout << "\nHasil penambahan a+b adalah: " << tambah(a,b);
    cout << "\nHasil pengurangan a-b adalah: " << kurang(a,b);

    return 0;
}

int inputData(string v) {
    cout << "masukan bilangan " << v << ": ";
    int bil;
    cin >> bil;
    return bil;

}
```
**gambar program**
https://github.com/rivaldiahmad/praktikum6/blob/master/latihan1/gambar1.png


##latihan2.1

**Alur Algoritma**
1.mulai program untuk menukar nilai 
2.gunakan cara passing parameter untuk mengalamatkan yang nantinya akan di ubah dalam fungsi
3.untuk menukar gunakan pointer pada variabel penukar untuk menandakan.
4.build dan run jika tidak ada kendala (eror) jalankan
5. end

**kode Program**
```
#include<iostream>
using namespace std;

void tukar(int *a, int *b)
{
    int c;
    c = *a;
    *a = *b;
    *b = c;

}
main(){
int a = 5, b = 8;
cout<< "\nSebelum di tukar\n";
cout << "Nilai 1 : " << a << endl;
cout << "Nilai 2 : " << b << endl;
tukar(&a, &b);
cout << "\nSesudah ditukar\n";
cout << "Nilai 1 : " << a << endl;
cout << "Nilai 2 : " << b << endl;
return 0;
}
```
**gambar program**
https://github.com/rivaldiahmad/praktikum6/blob/master/latihan2/gambar2.1.png

##latihan2.2

**Alur Algoritma**
1. mulai program menghitung dua bilangan dengan oprator penjumlah
2. deskripsikan interger a dan b
3. gunakan fungsi pengulangan for.
4. gunakann kembali rumus fungsi untuk menjalankan program
5. build and run
6. end

**Code Program**
```
#include<iostream>
#include<math.h>

using namespace std;

int kali(int m, int n)
{
    int i, hasil=0;
    for (i=1; i<=(n);i++)
        hasil +=m;
    if (n<0) return(-hasil); else return(hasil);
}
main(){
    int a,b;
    cout<<"\nMasukan Bilangan : ";
    cin >>a;
    cout<<"\nDikali Dengan : ";
    cin >>b;
    cout<< "Nilai " << a << " X " << b <<"=" << kali(a,b);
    return 0;
}
```
**gambar program**
https://github.com/rivaldiahmad/praktikum6/blob/master/latihan2/gambar2.2.png