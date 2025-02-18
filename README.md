# Sistema de Jogo de Xadrez

Este projeto implementa um sistema de jogo de xadrez em Java, permitindo que dois jogadores disputem partidas seguindo as regras oficiais do xadrez. O sistema gerencia tabuleiro, peças e movimentos, garantindo a integridade das regras do jogo.

## Tecnologias Utilizadas

- **Java** (Linguagem principal para desenvolvimento do sistema)

## Instalação e Execução

### Pré-requisitos

Certifique-se de ter instalado:
- **Java 17** ou superior
- **IDE Java** (Eclipse, IntelliJ IDEA, NetBeans, etc.)

### Passos para instalação

1. Clone o repositório:
   ```sh
   git clone https://github.com/RafaelCantovitzBueno/chess-system-java.git
   cd chess-system-java
   ```

2. Compile e execute o projeto:
   ```sh
   javac -d bin src/application/Program.java
   java -cp bin application.Program
   ```

## Peças e seus Movimentos

O sistema inclui todas as peças do xadrez, respeitando suas movimentações e regras.

- **K | King (Rei)**: Move-se uma casa em qualquer direção (horizontal, vertical ou diagonal). Pode realizar o movimento especial de roque.
- **Q | Queen (Rainha)**: Move-se qualquer número de casas em linha reta (horizontal, vertical ou diagonal).
- **R | Rook (Torre)**: Move-se qualquer número de casas em linha reta (horizontal ou vertical).
- **B | Bishop (Bispo)**: Move-se qualquer número de casas na diagonal.
- **N | Knight (Cavalo)**: Move-se em formato de "L" (duas casas em uma direção e uma perpendicularmente). Pode pular outras peças.
- **P | Pawn (Peão)**: Move-se uma casa para frente (ou duas casas no primeiro movimento). Captura peças na diagonal e pode realizar a captura "en passant". Pode ser promovido ao alcançar a última fileira.

## Funcionalidades

- Controle completo das regras do xadrez
- Validação de movimentos legais
- Detecção de xeque e xeque-mate
- Registro de jogadas
- Interface gráfica opcional para melhor experiência do usuário
- **Detecção de jogadas especiais:**
  - **Roque**: Movimento especial do rei e da torre, no qual o rei se move duas casas em direção à torre e a torre salta para a casa ao lado do rei, desde que nenhuma peça esteja entre eles e o rei não esteja em xeque.
  - **En Passant**: Captura especial realizada pelo peão. Se um peão avançar duas casas a partir de sua posição inicial e passar por uma casa atacada por um peão adversário, esse último pode capturá-lo como se tivesse se movido apenas uma casa.
  - **Promoção**: Quando um peão alcança a última fileira do tabuleiro, ele pode ser promovido a qualquer outra peça (exceto rei), geralmente uma rainha.

## Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para usá-lo e modificá-lo conforme necessário.
