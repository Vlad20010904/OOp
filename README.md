# OOp
#include<TCHAR.H>
#include "iostream"
#include "windows.h"
#include "math.h" 


using namespace std;

int _tmain(int argc, _TCHAR* argv[])
{
	double z, x, y, a , S, N;
	

	SetConsoleCP(1251);
	SetConsoleOutputCP(1251);

	cout << "Введіть тризначне число ";
	cin >> z;
	x = static_cast<int>(z) % 10;
	y = (int)z / 10 % 10;
	a = (int)z / 100 % 10;
	S = x + y + a;
	N = x * y * a;
	cout << "Сумма цифр числа " << S << "\n" ;
	cout << (char)S << "\n";
	cout << "Добуток цифр числа " << N << "\n";
	cout << (char)N << "\n";
	system("pause");

	return 0;
}
