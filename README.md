# Chess Game

Este projeto implementa um jogo de xadrez em Java. O jogo permite que dois jogadores façam movimentos alternados em um tabuleiro de xadrez, realizando jogadas, capturas e promoção de peças.

## Funcionalidades

- **Tabuleiro de Xadrez**: Um tabuleiro visual interativo onde você pode ver as peças e suas posições.
- **Movimentos Possíveis**: O programa exibe os movimentos possíveis para a peça selecionada.
- **Capturas**: As peças capturadas pelos jogadores são registradas e exibidas durante a partida.
- **Promoção de Peças**: O jogador pode promover um peão quando ele alcança a linha de promoção.
- **Verificação de Xeque-Mate**: O jogo verifica quando um jogador está em xeque-mate e finaliza a partida.

## Requisitos

- Java 8 ou superior

## Como Executar

1. Clone o repositório ou faça o download do código.
2. Compile o código utilizando um ambiente de desenvolvimento Java ou diretamente no terminal com o comando:

    ```bash
    javac Program.java
    ```

3. Execute o programa:

    ```bash
    java Program
    ```

## Estrutura de Pastas

```
src/
├── chess/
│   ├── ChessException.java
│   ├── ChessMatch.java
│   ├── ChessPiece.java
│   ├── ChessPosition.java
│   └── UI.java
└── Program.java
```

### Descrição dos Arquivos

- `Program.java`: A classe principal que executa o jogo de xadrez. Contém o loop do jogo e a lógica de movimentação das peças.
- `ChessMatch.java`: Contém a lógica de um jogo de xadrez, incluindo o estado das peças e a verificação de xeque-mate.
- `ChessPiece.java`: Define as peças de xadrez e seus comportamentos.
- `ChessPosition.java`: Representa a posição das peças no tabuleiro.
- `UI.java`: Responsável por imprimir o tabuleiro e o estado da partida no console, além de lidar com a entrada do usuário.
- `ChessException.java`: Exceções específicas para erros no jogo de xadrez.

## Como Jogar

1. O jogo é jogado no console.
2. Cada jogador insere a posição da peça que deseja mover (por exemplo, "e2").
3. O programa exibirá os movimentos possíveis para a peça selecionada.
4. O jogador então escolhe a posição de destino para o movimento (por exemplo, "e4").
5. O programa realiza o movimento, mostra o estado atual do tabuleiro e continua a partida.
6. Em caso de promoção de um peão, o jogador escolhe entre as opções: Bispo (B), Cavalo (N), Torre (R), ou Dama (Q).
7. O jogo continua até que um jogador seja colocado em xeque-mate.

## Exemplo de Execução

```
Source: e2
Target: e4
[Tabuleiro do Jogo]

Enter piece for promotion (B/N/R/Q): Q

[Estado Atual da Partida]
```

## Tratamento de Erros

- **Entrada inválida**: Caso o jogador insira uma posição inválida, o programa irá capturar a exceção e solicitará uma nova entrada.
- **Exceções no Jogo**: Caso um movimento seja inválido ou impossível, uma `ChessException` será lançada, e a mensagem de erro será exibida.

## Contribuições

Sinta-se à vontade para contribuir para este projeto! Caso tenha sugestões de melhorias ou correções de bugs, abra uma issue ou envie um pull request.

## Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
