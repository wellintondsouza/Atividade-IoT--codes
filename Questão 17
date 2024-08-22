#include <stdio.h>
#include <math.h> 

int calcularMDC(int a, int b) {
    while (b != 0) {
        int temp = b;
        b = a % b;
        a = temp;
    }
    return a;
}

int calcularMMC(int a, int b) {
    return (a * b) / calcularMDC(a, b);
}

int main() {
    int num1, num2;

    printf("Digite o primeiro numero: ");
    scanf("%d", &num1);
    printf("Digite o segundo numero: ");
    scanf("%d", &num2);

        int mdc = calcularMDC(num1, num2);
        int mmc = calcularMMC(num1, num2);

    // Exibe o resultado
         printf("O Maximo Divisor Comum de %d e %d é %d.\n", num1, num2,"ira ser", mdc);
         printf("O Minimo Multiplo Comum de %d e %d é %d.\n", num1, num2,"ira ser", mmc);
     }
