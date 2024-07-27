# Jogo-da-Velha
Descrição: Um jogo da velha para dois jogadores.
#include <stdio.h>

char tabuleiro[3][3];

void inicializarTabuleiro() {
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            tabuleiro[i][j] = ' ';
        }
    }
}

void exibirTabuleiro() {
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            printf("%c ", tabuleiro[i][j]);
            if (j < 2) printf("| ");
        }
        printf("\n");
        if (i < 2) printf("---------\n");
    }
}

int main() {
    inicializarTabuleiro();
    exibirTabuleiro();
    // Continue o desenvolvimento do jogo da velha...
    return 0;
}
