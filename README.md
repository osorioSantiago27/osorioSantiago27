#include<iostream>
#include <cstdlib>

using namespace std;

int main(){	
int time;
void limpiarPantalla();	
void jugarPartida();
char eleccion; 
string palabras[] = {"Monitor","Caja","Celular","Televisor","Carro","Casallas","Paisa","Vape","Damian","Mortadelo"};	


	while(true){
	     limpiarPantalla();	
		cout<<"\t::::MENU::::"<<endl;
		cout<<"1. Jugar Partida."<<endl;
		cout<<"2. Salir."<<endl;
		cout<<"Eleccion: ";
		cin>>eleccion;
		
		switch(eleccion){
			 case '1':
			 	jugarPartida();
			 	  break;
			 case '2':
			 	return 0;
			      break;	  
		}
	}
}

   void jugarPartida(){
   	srand((int)time(NULL)); 
	nA = rand()%10;
	cout<<nA; 	 	
   }
	
void limpiarPantalla(){
	if(system("cls") == -1){
     cout<<"error al borrar la pantalla";	
	}	
}
