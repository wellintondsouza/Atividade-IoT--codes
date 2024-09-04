#include <stdio.h>
#include <stdlib.h>


void printSubsequencia(int arr[], int antecessor[], int i) {
    if (i == -1)
        return;
    printSubsequencia(arr, antecessor, antecessor[i]);
    printf("%d ", arr[i]);
}


void maiorSubsequenciaCrescente(int arr[], int n) {
    int lis[n];  
    int antecessor[n]; 

    
    for (int i = 0; i < n; i++) {
        lis[i] = 1;  
        antecessor[i] = -1; 
    }

    
    for (int i = 1; i < n; i++) {
        for (int j = 0; j < i; j++) {
            if (arr[i] > arr[j] && lis[i] < lis[j] + 1) {
                lis[i] = lis[j] + 1;
                antecessor[i] = j;
            }
        }
    }

    
    int maxIndex = 0;
    for (int i = 1; i < n; i++) {
        if (lis[i] > lis[maxIndex]) {
            maxIndex = i;
        }
    }

   
    printf("A maior subsequência crescente é: ");
    printSubsequencia(arr, antecessor, maxIndex);
    printf("\n");
}

int main() {
    int arr[] = {10, 22, 9, 33, 21, 50, 41, 60, 80};
    int n = sizeof(arr) / sizeof(arr[0]);

    maiorSubsequenciaCrescente(arr, n);

    return 0;
}
