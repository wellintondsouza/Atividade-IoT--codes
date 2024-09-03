#include <stdio.h>
#include <stdlib.h>

// Função para trocar dois elementos
void troca(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}

// Função para particionar o array
int particionar(int arr[], int baixo, int alto) {
    int pivo = arr[alto]; // Escolhe o último elemento como pivô
    int i = (baixo - 1); // Índice do menor elemento

    for (int j = baixo; j < alto; j++) {
        if (arr[j] <= pivo) {
            i++; // Incrementa o índice do menor elemento
            troca(&arr[i], &arr[j]);
        }
    }
    troca(&arr[i + 1], &arr[alto]);
    return (i + 1);
}

// Função principal do Quick Sort
void quickSort(int arr[], int baixo, int alto) {
    if (baixo < alto) {
        int pi = particionar(arr, baixo, alto); // Particiona o array
        quickSort(arr, baixo, pi - 1); // Ordena a parte esquerda
        quickSort(arr, pi + 1, alto); // Ordena a parte direita
    }
}

// Função para imprimir o array
void imprimirArray(int arr[], int tamanho) {
    for (int i = 0; i < tamanho; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}

// Função para ler um array do usuário
void lerArray(int arr[], int tamanho) {
    printf("Digite %d numeros:\n", tamanho);
    for (int i = 0; i < tamanho; i++) {
        scanf("%d", &arr[i]);
    }
}

// Função principal
int main() {
    int tamanho;

    printf("Digite o numero de elementos do array: ");
    scanf("%d", &tamanho);

    // Aloca dinamicamente o array
    int *arr = (int *)malloc(tamanho * sizeof(int));
    if (arr == NULL) {
        printf("Erro na alocacao de memoria.\n");
        return 1;
    }

    lerArray(arr, tamanho);

    printf("Array original: ");
    imprimirArray(arr, tamanho);

    quickSort(arr, 0, tamanho - 1);

    printf("Array ordenado: ");
    imprimirArray(arr, tamanho);

    // Libera a memória alocada
    free(arr);

    return 0;
}
