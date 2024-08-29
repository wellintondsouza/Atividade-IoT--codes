#include <stdio.h>

// Função para trocar dois elementos
void trocar(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}

// Função para ordenar o array usando Bubble Sort
void bubbleSort(int arr[], int n) {
    int i, j;
    int trocou;

    // Loop para passar por todos os elementos
    for (i = 0; i < n - 1; i++) {
        trocou = 0; // Inicializa a flag de troca

        // Loop para comparar elementos adjacentes
        for (j = 0; j < n - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                // Se o elemento atual é maior que o próximo, troca-os
                trocar(&arr[j], &arr[j + 1]);
                trocou = 1; // Marca que uma troca ocorreu
            }
        }

        // Se nenhuma troca ocorreu, o array está ordenado
        if (trocou == 0) {
            break;
        }
    }
}

// Função para imprimir o array
void imprimirArray(int arr[], int tamanho) {
    int i;
    for (i = 0; i < tamanho; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}

// Função principal
int main() {
    int arr[] = {64, 34, 25, 12, 22, 11, 90};
    int n = sizeof(arr) / sizeof(arr[0]);

    printf("Array original: \n");
    imprimirArray(arr, n);

    bubbleSort(arr, n);

    printf("Array ordenado: \n");
    imprimirArray(arr, n);

    return 0;
}
