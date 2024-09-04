#include <stdio.h>
#include <stdlib.h>

#define MAX 100  

typedef struct {
    int itens[MAX];
    int frente;
    int traseira;
} Fila;

void inicializarFila(Fila *f) {
    f->frente = -1;
    f->traseira = -1;
}


int estaVazia(Fila *f) {
    return (f->frente == -1 && f->traseira == -1);
}

int estaCheia(Fila *f) {
    return (f->traseira == MAX - 1);
}

void enfileirar(Fila *f, int valor) {
    if (estaCheia(f)) {
        printf("A fila está cheia\n");
        return;
    }
    if (estaVazia(f)) {
        f->frente = 0;
    }
    f->traseira++;
    f->itens[f->traseira] = valor;
    printf("Enfileirado: %d\n", valor);
}

int desenfileirar(Fila *f) {
    if (estaVazia(f)) {
        printf("A fila está vazia\n");
        return -1;
    }
    int valor = f->itens[f->frente];
    if (f->frente == f->traseira) {
        f->frente = f->traseira = -1;
    } else {
        f->frente++;
    }
    return valor;
}

void exibirFila(Fila *f) {
    if (estaVazia(f)) {
        printf("A fila esta vazia!\n");
        return;
    }
    printf("Fila: ");
    for (int i = f->frente; i <= f->traseira; i++) {
        printf("%d ", f->itens[i]);
    }
    printf("\n");
}

int main() {
    Fila f;
    inicializarFila(&f);

    enfileirar(&f, 10);
    enfileirar(&f, 20);
    enfileirar(&f, 30);

    exibirFila(&f);

    printf("Desenfileirado: %d\n", desenfileirar(&f));
    printf("Desenfileirado: %d\n", desenfileirar(&f));

    exibirFila(&f);

    return 0;
}
