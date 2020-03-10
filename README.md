# Aiken
own project 
#include <iostream>
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

using namespace std;


int main(int argc, char** argv) 
{	
	int pay,save;
	int n,i,j,l,a,s,k;
	save = 0;
	n = 0;
	i = 0;
	j = 0;
	k = 0;
	l = 0;
	a = 0;
	s = 0;
	srand(time(NULL));
	int money=(rand() % 10000)+1; 
		
		
	while(money > 0)
	{
	
	
	cout << "您消費的金額是:" << money << endl;
	
	cout <<"您投入的金額是:";
	cin >> pay;
	cout <<endl;
	
	
	// money = 6400 pay = 1000執行 IF  
	while (money > k)
	{	money =  money - pay;
	
		if (  money > k)	
		{
		
			cout << "你投入的金額不足" << money << "元" << endl ;
			cout << "請再投入金額" << endl;
		
			cout <<"您投入的金額是:";
			cin >> pay;
			cout << endl;
			
			//money = -money;
		}
}
	}
	cout <<endl;
	money = -money;

	cout << "自動找零中..."  <<endl;
	
	save=money;

	if (save >= 1000)
	{	
	
		n= save/1000;
		cout << n << "張1000元鈔票" << endl; 
		//save = money - n*1000;
	
	}
	
	save = save - n*1000;
	//	save = money - n*1000;
	
	 if (save >= 500)
	{
		i = save/500;
		cout << i << "張500元鈔票" << endl; 
		//save = money - i*500;
		//save = save - i*500;
	
	}
	
	save = save - i*500;
		//save = money - i*500;
		
	 if (save >= 100)
	{
		j = save/100;
		cout << j << "張100元鈔票" << endl; 
		//save = money - j*100;
		//cout << save << endl;
	//	save = save - i*100;
	
	}
	
	save = save - j*100;
		//save = money - j*100;
	
		int p = 0;
	 if (save >= 50)
	{	
		p = save/50;
		cout << p << "個50元硬幣" << endl; 
		//save = money - k*50;
		//cout << save << endl;
		//save = save - k*50;
	}
		//save = money - k*50;
	save = save - p*50;
		
 if (save >= 10)
	{
		a = save/10;
		cout << a << "個10元硬幣" << endl; 
		//save = money - a*10;
		//cout << save << endl;
		//save = save - a*10;
	}
		//save = money - a*10;
		save = save - a*10;
	 if (save >= 5)
	{
		s = save/5;
		cout << s << "個5元硬幣" << endl; 
		//save = money - s*5;
		//save = save - s*5;
		//cout << save << endl;
	}
		//save = pay - s*5;
		save = save - s*5;
	 if (save >= 1)
	{
		 l = save /1;
		cout << l << "個1元硬幣" << endl; 
	//	save = money - l*1;
	//	save = save - l*1;
		//cout << save << endl;
	}
	//pay = pay - l*1;
	cout << "共找了" <<money <<"元";
	return 0;
}
