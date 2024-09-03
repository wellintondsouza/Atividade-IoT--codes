#include <stdio.h>
#include <stdlib.h>

#define MAX 150 // Define o tamanho máximo da pilha


typedef struct {
    int topo;
    int itens[MAX];
} Pilha;

void inicializarPilha(Pilha *p) {
    p->topo = -1;
}


int pilhaVazia(Pilha *p) {
    return p->topo == -1;
}


int pilhaCheia(Pilha *p) {
    return p->topo == MAX - 1;
}


void push(Pilha *p, int valor) {
    if (pilhaCheia(p)) {
        printf("Erro: Pilha cheia!\n");
        return;
    }
    p->itens[++(p->topo)] = valor;
}


int pop(Pilha *p) {
    if (pilhaVazia(p)) {
        printf("Erro: Pilha vazia!\n");
        return -1; 
    }
    return p->itens[(p->topo)--];
}


int peek(Pilha *p) {
    if (pilhaVazia(p)) {
        printf("Erro: Pilha vazia!\n");
        return -1; 
    }
    return p->itens[p->topo];
}


int main() {
    Pilha p;
    inicializarPilha(&p);

    push(&p, 10);
    push(&p, 20);
    push(&p, 30);

    printf("Elemento no topo: %d\n", peek(&p));  

    printf("Removendo elemento: %d\n", pop(&p));     printf("Elemento no topo: %d\n", peek(&p));  

    return 0;
}
