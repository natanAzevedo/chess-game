# Jogo de Xadrez em Java

Um jogo de xadrez completo desenvolvido em Java, rodando no terminal. Implementa todas as regras básicas do xadrez incluindo movimentos especiais.

## Como jogar

1. Compile e execute o projeto
2. O tabuleiro é exibido no terminal com coordenadas (a1 até h8)
3. Digite a posição da peça que quer mover (ex: `e2`)
4. Digite a posição de destino (ex: `e4`)
5. Continue jogando até o xeque-mate

### Comandos durante o jogo

- **Posições**: Use notação algébrica (a1, b2, c3, etc.)
- **Promoção de peão**: Quando um peão chega na última fileira, escolha uma peça (Q=Rainha, R=Torre, B=Bispo, N=Cavalo)

## Funcionalidades

✅ Todas as peças com seus movimentos corretos  
✅ Sistema de turnos alternados  
✅ Detecção de xeque e xeque-mate  
✅ Movimentos especiais: roque, en passant, promoção  
✅ Interface colorida no terminal  
✅ Lista de peças capturadas  
✅ Validação de movimentos legais  

## Executando o projeto

```bash
# Compile todas as classes
javac -d . src/application/*.java src/boardgame/*.java src/chess/*.java src/chess/pieces/*.java

# Execute o jogo
java application.Program
```

## Estrutura do código

```
src/
├── application/     # Interface do usuário e programa principal
├── boardgame/       # Classes base para tabuleiro e peças
├── chess/           # Lógica específica do xadrez
└── chess/pieces/    # Implementação de cada tipo de peça
```

O projeto usa conceitos de orientação a objetos como herança, polimorfismo e encapsulamento. Cada peça tem sua própria classe que herda de `ChessPiece`, que por sua vez herda de `Piece`.

## Sobre

Projeto desenvolvido para praticar programação orientada a objetos em Java. Implementa um jogo de xadrez funcional com interface de terminal colorizada.