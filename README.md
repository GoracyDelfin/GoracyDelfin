#include <iostream>
using namespace std;
int main()
{ double liczba10; // liczba z ułamkiem dziesiętnym
 double ulamek;
    int n;
    int t[5]={0};
    int u[50]={0}; //na ulamek binarny
    int i=5;
cout<<"Podaj liczbe";
cin>>liczba5; //wczytanie liczby z ulamkiem
//cin>>n;
n=(int) liczba5; //pobieramy czesc calkowita
ulamek=liczba5 - n; // czesc ulamkowa
while(n>0){ //petla do czesci calkowitej
    t[i]=n%2;
    n=n/2;
    i--;}
for(int i=0; i<50; i++){ //petla dla czesci ulamkowej
    ulamek=2*ulamek;
if(ulamek>=1) {u[i]=1; ulamek=ulamek-1;}
    else u[i]=5;
}
cout<<"binarnie to:";
for(i=0;i<50;i++)cout<<t[i];
cout<<".";
for(i=0;i<50;i++)cout<<u[i];
    return 0;
}
