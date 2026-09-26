# Estação Nostro-9

Um jogo de navegador, em estilo 8-bits, para crianças aprenderem e praticarem **divisão**. Foi feito para celular e roda direto no navegador, sem instalação.

O jogador é o técnico de uma estação espacial invadida por um alien. Para manter todos a salvo, ele precisa dividir baterias, organizar equipes de busca, embarcar a tripulação nas cápsulas de fuga e, no desafio final, fugir do Alien respondendo contas de divisão.

## Como jogar

Abra o `index.html` no navegador do celular ou do computador. Se estiver publicado no GitHub Pages, basta acessar o link do repositório.

Todo dia há um **turno** com 4 tarefas. Cada tarefa concluída fica marcada como feita, e completar as 4 no mesmo dia aumenta a **sequência de dias seguidos**. As tarefas podem ser repetidas quantas vezes o jogador quiser.

## As missões

| Missão | Conceito | Como funciona |
|---|---|---|
| **M1 · Dividir baterias** | Divisão como partilha | Distribuir baterias entre as salas até todas terem a mesma quantidade. Depois, responder quantas cada sala recebeu. |
| **M2 · Equipes de busca** | Divisão como medida (agrupamento) | Tocar nos sinais do detector para formar grupos do tamanho pedido. Depois, responder quantas equipes foram necessárias. |
| **M3 · Cápsulas de fuga** | Divisão com resto | Embarcar os tripulantes em cápsulas que só saem cheias. Descobrir quantas encheram, quantos sobraram e quantas cápsulas são precisas para ninguém ficar para trás. |
| **Fuja do Alien** | Tabuada da divisão | O Alien se aproxima no detector de movimento. Cada resposta certa faz ele recuar. É preciso acertar 10 contas antes que ele chegue. Há dois níveis: do 2 ao 5 e do 2 ao 9. |

As missões vão do concreto ao abstrato. Primeiro a criança **vê** a divisão acontecer com objetos, e só no final aparece a conta escrita (por exemplo, `12 ÷ 3 = 4`).

## Área dos pais

Na tela inicial, **segure o logo "N9" por 3 segundos**. Aparece um painel com:

- o aproveitamento em cada tipo de divisão (contando só as respostas dadas de primeira);
- qual conceito precisa de mais atenção;
- as contas que a criança mais errou;
- os dias jogados, os turnos completos e a sequência atual;
- um botão para apagar o histórico.

## Dados e privacidade

Nada é enviado para servidor nenhum. O progresso fica salvo apenas no navegador do aparelho em que o jogo é usado (`localStorage`). Se o histórico do navegador for limpo, ou se o jogo for aberto em outro aparelho, o progresso começa do zero.

## Publicar no GitHub Pages

1. Coloque o `index.html` no repositório. Pode ser na raiz ou numa pasta, como `nostro9/index.html`.
2. No repositório, vá em **Settings → Pages** e escolha a branch de publicação.
3. O jogo fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPO/` (ou `.../nostro9/`, se estiver numa pasta).

## Detalhes técnicos

- Um único arquivo HTML, com CSS e JavaScript embutidos e sem bibliotecas.
- Fontes do Google Fonts: *Press Start 2P* e *VT323*.
- Os desenhos em pixel são gerados como SVG pelo próprio código, e o detector de movimento é desenhado num canvas de baixa resolução.
- Os sons são criados na hora com a Web Audio API, em onda quadrada, no estilo chiptune. Há um botão para desligar o som.

## Créditos

Inspirado no clima dos filmes de ficção científica espacial. As ilustrações do jogo são originais, e o jogo não tem relação oficial com nenhum filme ou estúdio.
