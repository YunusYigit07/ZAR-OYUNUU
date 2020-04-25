# ZAR-OYUNUU
#include<iostream>
#include<time.h>
#include<string>

using namespace std;
class ZarOyun
{
public:
	ZarOyun();
	int oyna();
	int toplam(int, int);
	~ZarOyun();


private:
	int z1, z2;
	
};
ZarOyun::ZarOyun()
{
	cout << "*-*-*-*-*-* ZAR OYUNU *-*-*-*-*-*" << endl << endl << endl;
	cout << "*-*-*-*-*-*- OYUN BASLADI *-*-*-*-*-*" << endl;

}
int ZarOyun::oyna()
{
	srand(time(NULL));

	z1 = rand() % 6 + 1;
	z2 = rand() % 6 + 1;

	cout << "*-*-* Birinci zar ust degeri: " << z1 << endl << endl;
	cout << "*-*-* Ikinci  zar ust degeri: " << z2 << endl << endl;
	toplam(z1, z2);
	return 0;
}
int ZarOyun::toplam(int zar1, int zar2)
{
	
	z1 = zar1;
	z2 = zar2;
	int sonuc = z1 + z2;
	if (sonuc == 7)
	{
		cout << "*-*-* Oyunu Kazandiniz *-*-*" << endl << endl; 
	}
	else
	{
		cout << "*-*-* Oyunu Kaybettiniz *-*-*" << endl << endl;
		
	}
	return 0;
}
ZarOyun::~ZarOyun()
{
	cout << "*-*-*-*-*-* OYUN BITTI... *-*-*-*-*-*" << endl;
}
int main()
{
	ZarOyun o;
	o.oyna();
	//uluibrahim deneme amacli ekledi.
	ZarOyun o2;
	o2.oyna();

return 0;
}

