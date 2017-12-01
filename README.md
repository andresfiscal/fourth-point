# fourth-point
#include <iostream>
#include <cstdlib>

using namespace std;

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main() {
	system("PAUSE");
	int m; //tamaño del arreglo
    cout<<"introduce el tamaño del arreglo "; // pedir el tamaño del arreglo
    cin>> m;
    int arreglo1[m][m];
    int arreglo2[m][m];
    int numero;
    for(int i=0; i<m; i=i+1){
        for(int j=0; j<m; j=j+1){
        cout<<"introduce el numero ";
		cin>> numero;	
		arreglo1[i][j] = numero;
		 
		arreglo2[j][i] = arreglo1[i][j];
		 
		}
	}
	for(int i=0; i<m; i=i+1){
        for(int j=0; j<m; j=j+1){
        	cout << "el numero " << arreglo1[i][j]<< " esta en la posicion "  << i << j <<endl;
        	
		}
	}
	cout<< "" <<endl;
	for(int i=0; i<m; i=i+1){
        for(int j=0; j<m; j=j+1){
        	
        	cout << "el numero " << arreglo2[i][j]<< " esta en la posicion "  << i << j <<endl;
		}
	}
	return 0;
}
