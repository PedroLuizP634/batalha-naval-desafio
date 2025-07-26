# batalha-naval-desafio
└── nivel-novato/
#include <stdio.h>

int main() {
    int tabuleiro[5][5] = {0};

    // Navio vertical
    int x_vert = 0, y_vert = 1;
    for (int i = 0; i < 3; i++) {
        tabuleiro[x_vert + i][y_vert] = 1;
    }

    // Navio horizontal
    int x_horiz = 4, y_horiz = 0;
    for (int j = 0; j < 4; j++) {
        tabuleiro[x_horiz][y_horiz + j] = 1;
    }

    // Exibe coordenadas
    printf("Coordenadas do Navio Vertical:\n");
    for (int i = 0; i < 3; i++) {
        printf("(%d, %d)\n", x_vert + i, y_vert);
    }

    printf("\nCoordenadas do Navio Horizontal:\n");
    for (int j = 0; j < 4; j++) {
        printf("(%d, %d)\n", x_horiz, y_horiz + j);
    }

    return 0;
}

    └── README.md 
    
    # 🟢 Nível Novato - Desafio Batalha Naval

## Objetivo
Simular o posicionamento de dois navios em um tabuleiro 5x5 utilizando vetores bidimensionais.

## O que foi feito
- Um navio vertical de 3 posições.
- Um navio horizontal de 4 posições.
- Exibição das coordenadas ocupadas no console com printf.

## Entrada
- As posições são definidas diretamente no código.

## Saída esperada
