#include <stdio.h>
#include <string.h>

int main() {
    char palindromo[100]; // Declara palindromo como uma string
    printf("Escreva uma palavra ou frase:\n");
    scanf("%s", palindromo); // Lê a palavra do usuário

    int len = strlen(palindromo); // Obtém o comprimento da palavra
    int is_palindrome = 1; // Flag para determinar se é um palíndromo

    // Verifica se a palavra é um palíndromo
    for (int i = 0; i < len / 2; i++) {
        if (palindromo[i] != palindromo[len - i - 1]) {
            is_palindrome = 0; // Define a flag como 0 se não for um palíndromo
            break;
        }
    }

    // Imprime o resultado
    if (is_palindrome) {
        printf("Este nome e um palindromo\n");
    } else {
        printf("Este nome nao e um palindromo\n");
    }

    return 0;
}
