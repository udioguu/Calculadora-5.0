# Calculadora-5.0
A calculadora mais simples e prática.
#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>
int main()
{ //By: Diogo Biaggio
    //First Project
    // Em linguagem C

    float num1, num2, resultado;
    char op = '0';


        printf("==========Calculadora 5.0===========\n\n");
    do{
        num1, num2, resultado = 0;
        //imprimindo as opções da nossa calculadora
        printf(" (1) somar\n");
        printf(" (2) subtracao\n");
        printf(" (3) multiplicacao\n");
        printf(" (4) divisao\n");
        printf(" (0) encerrar calculadora\n");

          printf("Informe a operacao que deseja fazer: \t >>");
          op = getche();
          printf("\n\n");

          if (op == '0'){
            printf("O programa foi encerrado!\n");
            }else{
         printf("Digite o primeiro numero:\t\t >>");
         scanf("%f", &num1);
         printf("\n");
         printf("Digite o segundo numero:\t\t >>");
         scanf("%f", &num2);
         printf("\n");
         }

         if(op != '0' && op != '1' && op != '2' && op != '3' && op != '4'){
            printf("O operador indicado es invalido, escolha um dos 4 números!! \n");
         }
             else if (op == '1') {
            resultado = num1 + num2;
            printf("A soma entre os dois numeros vale:\t >> %f", resultado);
            }
             else if (op == '2'){
            resultado = num1 - num2;
            printf("A subtracao entre os dois numeros vale:\t >> %f", resultado);
            }
             else if (op == '3') {
            resultado = num1 * num2;
            printf("A multiplicacao entre os dois numeros vale:\t >> %f", resultado);
            }
             else if (op == '4'){
            resultado = num1 / num2;
            printf("A divisao entre os dois numeros vale:\t >> %f \n\n", resultado);
            }

            printf("\n\n\n\n===========================================\n\n");

            system("pause");
            system("cls");
    }while (op != '0');


    return 0;
}
