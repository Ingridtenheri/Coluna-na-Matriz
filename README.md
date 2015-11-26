# Coluna-na-Matriz

#include <stdio.h>
#include <stdlib.h>
int main() {
     
int C, LINHA, COLUNA;
        char T;
        float  M[12][12], R=0;
            
    scanf("%d",&C); //numero requerido pelo usuario
        
    scanf(" %c", & T);
            
  
    for(LINHA=0;LINHA<12;LINHA++) // montando linha da matriz
    {
       for (COLUNA=0;COLUNA<12;COLUNA++) // montando coluna da matriz
       {
           scanf("%f", &M[LINHA][COLUNA]);
       }
    }
        
       for (COLUNA=0;COLUNA<12;COLUNA++) 
       {
       R += M[COLUNA][C]; // somando a coluna do numero digitado
       }
       if (T == 'S' || T == 's') // se o usuario desejar somar digitando assim a letra s
       {
       printf ("%.1f\n",R); // a soma sera apresentada na tela
}
       if (T == 'M' || T == 'm') // se o usuario desejar a media da linha digitando a letra m 
       {
       printf ("%.1f\n",R/12);     // a media sera apresentada na tela
       }   
     
    return 0;
}
