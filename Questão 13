#include <stdio.h>

int main() {
    
    int primeiroElemento;// primeiro Elemento
	int segundoElemento;// segundo Elemento
	int proximoElemento;// terceiro Elemento
	int contador; //contador
    
    printf("Os primeiros numeros na sequencia de fibonacci são:");
  
    primeiroElemento=1;
    segundoElemento=1;
    
    for (contador = 3; contador <= 10; contador++) {
        proximoElemento = primeiroElemento + segundoElemento;
        printf("%d ", proximoElemento);

        // Atualiza os valores para o próximo cálculo
        primeiroElemento = segundoElemento;
        segundoElemento = proximoElemento;
    }

    printf("\n"); // Adiciona uma nova linha no final da saída
    
    return 0;
}
