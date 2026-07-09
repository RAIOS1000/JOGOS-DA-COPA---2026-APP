# Como atualizar a Copa (fácil) ⚽

A partir de agora **você não precisa mexer no `index.html`**. Todos os dados que
mudam ficam no arquivo **`dados.json`**. É só editar esse arquivo e salvar.

O app carrega o `dados.json` automaticamente ao abrir. Se o arquivo não existir
ou você estiver offline, ele usa os dados embutidos como reserva.

## O que dá pra editar no `dados.json`

- **`grupos[].res[]`** — os jogos e placares de cada grupo.
  Basta mudar o **placar** (`sc`), ex.: `"sc":"2–1"`. Um jogo ainda não jogado
  fica `"sc":"×"`.
  > ⚠️ Você **não** precisa mexer na tabela de classificação: **pontos, saldo,
  > gols e a ordem são calculados sozinhos** a partir dos placares.
- **`artilheiros[]`** — a lista de goleadores (`n` nome, `s` país, `f` bandeira,
  `g` gols, `j` jogos).
- **`calendario[]`** — os jogos por dia (data, hora, times).
- **`ticker[]`** — as frases que passam na faixa dourada do topo.
- **`facts[]`** — os destaques da aba Artilheiros.

## Passo a passo (pelo GitHub, no celular ou PC)

1. Abra o repositório no GitHub e clique em **`dados.json`**.
2. Toque no **lápis** (Editar).
3. Mude o que quiser (por ex., o placar de um jogo).
4. Role até o fim e clique em **Commit changes**.
5. Em ~1 minuto o site atualiza. No app, **recarregue** (puxe a tela pra baixo).

## Dica

Use a aba **🎮 Simulador** dentro do app pra testar placares e ver a
classificação mudar na hora, antes de gravar no `dados.json`.
