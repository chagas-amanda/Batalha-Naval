# Batalha-Naval

Jogo de Batalha Naval para o terminal: você contra o computador, em um tabuleiro de 5x8. Vence quem afundar todos os barcos do adversário primeiro. Quem será que leva essa disputa?

## Compilar e executar

```bash
gcc batalha_naval.c -o batalha
./batalha
```

> No Windows, se o `■` ou os acentos saírem estranhos, rode `chcp 65001` antes.

## Como jogar

- Ao abrir, digite `c` para aceitar a disputa ou `n` para recusar.
- Na sua vez, digite a jogada como **letra + número**, por exemplo `B3`.
- Jogada inválida ou repetida não gasta a vez: o jogo avisa e você joga de novo.
- O tabuleiro de cima é o do computador (barcos escondidos). O de baixo é o seu.

## Símbolos

| Símbolo | Significado |
|---|---|
| `@` | barco comum (1 posição), só no seu tabuleiro |
| `#` | metade de um barco grande, só no seu tabuleiro |
| `*` | barco comum atingido |
| `■` | metade de barco grande atingida |
| `x` | tiro na água |

Cada jogador tem 7 barcos comuns e 1 barco grande, que ocupa 2 posições vizinhas.

## Bibliotecas

`stdio.h`, `stdlib.h`, `string.h`, `ctype.h` (maiúsculas/minúsculas) e `time.h` (semente do `rand`).
