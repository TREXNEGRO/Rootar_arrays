/*
************************************
*                                  *
*           By TREXNEGRO           *
*                                  *
************************************
*/
//LIBRERIAS
#include <stdio.h>
#include <stdlib.h>
//LOGITUD MAIMA DE ARRAY
#define LONG_MAX 10

//DECLARACION DE FUNCIONES
void lecturaVector (int[],int);
void cifradoVector (int[],int[],int);
void impresionVector (int[],int);

//CUERPO
int main(){

  int dim, clave,P=0;
  int v1[LONG_MAX], v2[LONG_MAX];
  
  //LEER Y ESCRIBIR 
  
    printf("Cifrado de datos!\n");
    printf("Ingrese la dimension: ");
    scanf("%d",&dim);
   if(dim<=10){
        printf("ingrese la clave: ");
        scanf("%d",&clave);
        printf("Ingrese los elementos del vector en texto claro\n");
        lecturaVector(v1, dim);
        do{
            P++;
        cifradoVector(v1, v2, dim);
        }while(P!=clave);
        printf("\nVector cifrado:\n");
        impresionVector(v2, dim);
    }else{
        printf("\nnumero invalido!");
    }
    return 0;
}

//DESCRIPCION DE FUNCIONES

//LECTURA DE ARRAY 
void lecturaVector(int vector[], int dim){
	for(int i=0;i<dim;i++){
		printf("claro[%d]:",i);
		scanf("%d",&vector[i]);
	}
}
//IMPRIMIR ARRAY 
void impresionVector (int vectorCifrado[], int dim){
	for(int i=0;i<dim;i++){
		printf("cifrado[%d]:%d\n",i,vectorCifrado[i]);
	}
}


//ROTAR EL ARRAY (PARA UNA VEZ)
void cifradoVector(int vector[], int vectorCifrado[], int dim){
    int aux = vector[dim-1];
   
    for(int i = dim - 1; i > 0; --i)
        vector[i] = vector[i-1];
    vector[0] = aux;
    
    for(int i=0;i<=dim-1;i++){
        vectorCifrado[i]=vector[i];
    }

    }
    
