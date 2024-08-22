#include <stdio.h>


int buscaLinear(int vetor[], int tamanho, int chave) {
    for (int i = 0; i < tamanho; i++) {
        if (vetor[i] == chave) {
            return i; 
        }
    }
    return -1; 
}

int main() {
    int tamanho;
    
    printf("Digite o tamanho do vetor: ");
    scanf("%d", &tamanho);
    
    int vetor[tamanho];
        
    printf("Digite os %d elementos do vetor:\n", tamanho);
    for (int i = 0; i < tamanho; i++) {
        scanf("%d", &vetor[i]);
    }
    
    int chave;
    printf("Digite o valor a ser buscado: ");
    scanf("%d", &chave);
    
    
    int indice = buscaLinear(vetor, tamanho, chave);
    
    if (indice != -1) {
        printf("O valor %d foi encontrado no indice %d.\n", chave, indice);
    } else {
        printf("o valor %d não foi encontrado no vetor.\n", chave);
    }
    
    return 0;
}
