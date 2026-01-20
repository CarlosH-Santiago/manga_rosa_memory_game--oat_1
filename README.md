# 🧠 Manga Rosa Memory Game (Java Console Edition)

![Java](https://img.shields.io/badge/Java-17-orange?logo=java)
![Type](https://img.shields.io/badge/Application-Console-black)
![License](https://img.shields.io/github/license/CarlosH-Santiago/manga_rosa_memory_game--oat_1)

Implementação de um **Jogo da Memória** via terminal, desenvolvido como parte da OAT 1 da diciplina de Estrutura de dados.

O projeto foca na manipulação de matrizes, lógica de pontuação complexa e interação via linha de comando, seguindo estritamente as regras de negócio definidas no desafio.

## 📋 Sobre o Projeto

O objetivo foi criar um jogo multijogador (local) onde a lógica e a memória são testadas. Diferente de um jogo da memória tradicional, este possui "armadilhas" e bônus baseados nas cores das cartas.

**Principais Requisitos Atendidos:**
* Desenvolvido em **Java 17**.
* Execução exclusiva via **Console/Terminal** (Sem GUI)].
* Implementação em classe única (`MangaRosaMemoryGame`).
* Pacote base: `br.com.mangarosa.games`.

## 🎮 Regras do Jogo

O jogo suporta 2 participantes que competem por pontos.

### ⚙️ Configuração
**Tabuleiro:** Tamanhos selecionáveis de 4x4, 6x6, 8x8 ou 10x10.
**Cartas:** Possuem pares de imagens e uma cor de fundo (Vermelho, Azul, Amarelo ou Preto).

### 🏆 Sistema de Pontuação
Cada jogador tem uma cor atribuída (Vermelho ou Azul). A pontuação varia conforme a cor da carta encontrada:

| Tipo da Carta | Ação | Pontuação |
| :--- | :--- | :--- |
| **Par Amarelo** | Acertar | **+1 ponto** |
| **Par da Sua Cor** | Acertar | **+5 pontos** |
| **Par do Adversário** | Acertar | **+1 ponto** |
| **Par do Adversário** | Errar | **-2 pontos** |

### ☠️ A Regra da Carta Preta
Existe um par de cartas com **fundo preto** em todo jogo. Ela define o destino da partida instantaneamente:
* ⚠️ **Se errar o par:** O jogador perde o jogo imediatamente (Game Over).
* 👑 **Se acertar o par:** O jogador vence o jogo automaticamente (Win).

## 🚀 Como Executar

Certifique-se de ter o **JDK 17** ou superior instalado.

1. **Clone o repositório:**
```bash
   git clone [https://github.com/CarlosH-Santiago/manga_rosa_memory_game--oat_1.git](https://github.com/CarlosH-Santiago/manga_rosa_memory_game--oat_1.git)

```

2. **Compile o código:**
Navegue até a pasta `src` (ou onde está o arquivo `.java`) e execute:
```bash
javac -d . MangaRosaMemoryGame.java

```


3. **Execute o jogo:**
```bash
java br.com.mangarosa.games.MangaRosaMemoryGame

```


*(Nota: O caminho do pacote pode variar conforme a sua estrutura de pastas, ajuste se necessário para `games.mangarosa.com.br` se seguiu o PDF literalmente).*

## 📂 Estrutura de Arquivos

Conforme solicitado na especificação, o código pode estar concentrado para facilitar a avaliação:

```
src/
└── br/com/mangarosa/games/
    └── MangaRosaMemoryGame.java  # Classe principal com método main

```

## 🛠️ Tecnologias

* **Linguagem:** Java 17 (LTS)
* **Entrada/Saída:** `java.util.Scanner`, `System.out`

## ✒️ Autor

Desenvolvido por 
1. *Carlos Henrique de Souza Santana Santiago* - *carloshsssantiago@gmail.com*
2. *Gustavo Bezerra Nonato* - *gustavaobezerra@gmail.com*
3. *João Guilherme Gonçalves Pinheiro* - *jgpinheiro30@gmail.com*
4. *Leonardo Freitas de Carvalho Nery* - *leoneryfreitas@gmail.com*
5. *Moisés de Souza Oliveira* - *Moisessouza0204@gmail.com*

---

<p align="center">
Projeto desenvolvido para fins educacionais.
</p>

