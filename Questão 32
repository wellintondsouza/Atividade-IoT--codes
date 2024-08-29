#include <stdio.h>

// Função para realizar a ordenação por Selection Sort
void selectionSort(int arr[], int n) {
    int i, j, minIndex, temp;

    // Percorre o array
    for (i = 0; i < n-1; i++) {
        // Encontra o menor elemento no array não ordenado
        minIndex = i;
        for (j = i+1; j < n; j++) {
            if (arr[j] < arr[minIndex]) {
                minIndex = j;
            }
        }

        // Troca o menor elemento encontrado com o primeiro elemento
        temp = arr[minIndex];
        arr[minIndex] = arr[i];
        arr[i] = temp;
    }
}

// Função para imprimir o array
void printArray(int arr[], int size) {
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}

int main() {
    int arr[] = {64, 25, 12, 22, 11};
    int n = sizeof(arr)/sizeof(arr[0]);

    printf("Array antes da ordenação:\n");
    printArray(arr, n);

    selectionSort(arr, n);

    printf("Array após a ordenação:\n");
    printArray(arr, n);

    return 0;
}
