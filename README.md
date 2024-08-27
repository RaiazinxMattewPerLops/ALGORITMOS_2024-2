

#include <stdio.h>
 int main() {
    
    //VARIAVEIS
    double n;
    int nota, moeda;
    
    //LER A VARIAVEL n
    scanf("%lf", &n);
    
    //CALCULO E IMPRESSÃO DAS NOTAS
    printf("NOTAS:\n");
    
    /*facilitar calculos com numeros de ponto flutuante multiplicamos o valor monetário por 100 para converter tudo para centavos*/
    
    int money = (int)(n * 100 + 0.5);
   
    nota = money/10000;
    printf("%d nota(s) de R$ 100.00\n", nota);
    money = money % 10000;
    
    nota = money/5000;
    printf("%d nota(s) de R$ 50.00\n", nota);
    money = money % 5000;
    
    nota = money/2000;
    printf("%d nota(s) de R$ 20.00\n", nota);
    money = money % 2000;
    
    nota = money/1000;
    printf("%d nota(s) de R$ 10.00\n", nota);
    money = money % 1000;
    
    nota = money/500;
    printf("%d nota(s) de R$ 5.00\n", nota);
    money = money % 500;
    
    nota = money/200;
    printf("%d nota(s) de R$ 2.00\n", nota);
    money = money % 200;
    
    //IMPRESSÃO DAS MOEDAS
    printf("MOEDAS:\n");
    
    moeda = money/100;
    printf("%d moeda(s) de R$ 1.00\n", moeda);
    money = (int)money % 100;

    moeda = money/50;
    printf("%d moeda(s) de R$ 0.50\n", moeda);
    money = money % 50;
    
    moeda = money/25;
    printf("%d moeda(s) de R$ 0.25\n", moeda);
    money = money % 25;
    
    moeda = money/10;
    printf("%d moeda(s) de R$ 0.10\n", moeda);
    money = money % 10;
    
    moeda = money/5;
    printf("%d moeda(s) de R$ 0.05\n", moeda);
    money = money %5;
 
    moeda= money/1;
    printf("%d moeda(s) de R$ 0.01\n", moeda);
    return 0;
}
