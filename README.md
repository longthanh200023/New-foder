#include <iostream>
#include <math.h>
using namespace std;

int main()
{   
    double Nam;
    double TG;
    double TKV;
    double LS;
    do
    {
    	cout << "Nhap so tien gui: ";
    	cin >> TG;
	
    	cout << "Nhap so tien ky vong: ";
    	cin >> TKV;

    	cout << "Nhap lai suat theo nam: ";
    	cin >> LS;
    	if (TKV<=TG||TKV<=0||TG<=0||LS<=0)
    	{
		 cout<<"nhap sai du lieu."<<endl;
    	}	
    }while(TKV <= TG||TKV<=0||TG<=0||LS<=0);
 
    Nam = log(TKV/TG)/log(1+LS);
    cout << "So nam can thiet de dat duoc so tien ky vong la: " << Nam << endl;
	
    return 0;
}
