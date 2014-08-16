algoritmos
==========
#include <iostream>
#include "conio.h"
using namespace std;

int sumapares(int a){
int i=0,c=0;
while(i<=a){
	if(i%2==0){
c=c+i;
	}
i++;
}
return(i);
}
int sumaNpares(int a){
int c=0,i=0;
while(i<=a){
c=c+(i*2);
i++;
}
return(c);
}
int sumalosNparescnwhile(int a){
int i=0,c=0;
a=(a*-1);
while(i<=a){
	if(i%2==0){
c=c+i;
	}
i++;
}
i=(i*-1);
return(i);
}
int main (){
	int opcion,a,r;
	do{
		cout <<endl<< "\n\n******MENU****";
		cout <<endl<<"---ingrese opcion---";
		cout <<endl<< "1.-suma de pares hasta N ";
		cout <<endl<< "2.-suma de los primeros N pares";
		cout <<endl<< "3.-suma de los primeros N pares con while";
		cin >> opcion;
		switch(opcion){
			case 1 :sumapares(a);
				cout<<"ingrese numero";
				cin>>a;
				r=sumapares(a);
				cout<<r;
				    break;
			case 2 :sumapares(a);
				cout<<"ingrese numero";
				cin>>a;
				r=sumaNpares(a);
				cout<<r;
				    break;
			case 3 :sumalosNparescnwhile(a);
				do{
				cout<<"ingrese numero";
				cin>>a;
				}while(a>0);
				r=sumalosNparescnwhile(a);
				cout<<r;
				    break;
		
		}
	}while (opcion !=0);
	return(0);
	}
