#include <iostream>
using namespace std;


int main()
{
int monto_1=200,monto_2=100,monto_3=50,monto_4=20;



char telcel();
char movistar();
char unefon();

int recarga = 200;
int recarga_2 = 100;
int recarga_3 = 50;
int recarga_4 = 20;

char opcion;
char numero;
int saldo_inicial=1000,monto,seguir,a;



do{//aqui inicia el do while------------------------------------------------------------------------------

	int opcion;
	cout<<"\n\t\t\t----selecciona la compania---- \n";
	cout<<"\n\t\t\t1. telcel :\n";
	cout<<"\n\t\t\t2. movistar :\n";
	cout<<"\n\t\t\t3. unefon :\n";
	cout<<"\n\t\t\t4. salir :\n";
	cin>>opcion;
	
//con condicion para que el programa se acabe
	switch(opcion)
	{




		case 1:  //recarga telcel-------------------200-------------------------
		do{
		
            cout<<"\n\t\t\tingrese el numero de tu celular de 10 digitos:";
			cin>>numero;
			
			if(numero>=10)// se realiza la cuenta del monto
			{
				saldo_inicial = saldo_inicial - recarga;
			    cout<<"\n\t\t\tsu recarga fue exitosa de:"<<recarga;
			    cout<<"\n\t\t\tsu cuenta es :"<<saldo_inicial;
			}
			else
			{
				
			    cout<<"\n\t\t\topcion invalida:";
			}
		cout<<"\n\t\t\tidesea realizar otra recarga telcel:(s/n)";
		cin>>seguir;
	    }while(seguir!='n');
	    cout<<"\n\t\t\tla cantidad de la cuenta es :"<<saldo_inicial<<endl;
		break;





		case 2://recarga movistar--------------------100-----------------------------
		do{
		cout<<"\n\t\t\tingrese el numero de tu celular de 10 digitos:";
			cin>>numero;
			
			if(numero>=10)// se realiza la cuenta del monto
			{
				saldo_inicial = saldo_inicial - recarga_2;
			    cout<<"\n\t\t\tsu recarga fue exitosa :"<<recarga_2;
			    cout<<"\n\t\t\tsu cuenta es :"<<saldo_inicial<<endl;
			}
			else
			{
				
			    cout<<"\n\t\t\topcion invalida:";
			}



		cout<<"\n\t\t\tdesea retirar mas dinero a su cuenta:(s/n)";
		cin>>seguir;
	    }while(seguir!='n');
	    cout<<"\n\t\t\tla cantidad disponible es :"<<saldo_inicial<<endl;	
		break;
		









		
		case 3://recarga unefon---------------------------------------------------------50------------------------------------
			cout<<"\n\t\t\tingrese el numero de tu celular de 10 digitos:";
			cin>>numero;
			
			if(numero>=10)// se realiza la cuenta del monto
			{
				saldo_inicial = saldo_inicial - recarga_3;
			    cout<<"\n\t\t\tsu recarga fue exitosa :"<<recarga_3;
			    cout<<"\n\t\t\tsu cuenta es :"<<saldo_inicial<<endl;
			}
			else
			{
				
			    cout<<"\n\t\t\topcion invalida:";
			}
			break;
			




                   case 4://-----------------------20--------------------------------
                       cout<<"\n\t\t\tingrese el numero de tu celular de 10 digitos:";
			cin>>numero;
			
			if(numero>=10)// se realiza la cuenta del monto
			{
				saldo_inicial = saldo_inicial - recarga_4;
			    cout<<"\n\t\t\tsu recarga fue exitosa :"<<recarga_4;
			    cout<<"\n\t\t\tsu cuenta es :"<<saldo_inicial<<endl;
			}
			else
			{
				
			    cout<<"\n\t\t\topcion invalida:";
			}





			
			case 5:  //esta funcion hace salir del programa-----------------------------------4444444444444444444-----------------------------------------
			cout<<"\n\tpresiona -1- para ir opciones o -2- para salir:";
			cin>>a;		
			if(a!='1')
			{
				return 0;
			}
			else
			{
		    	opcion++;
			}
			break;
	}
	opcion++;
}while(opcion!='n');
return 0;
}
