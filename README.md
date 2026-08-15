# Tomar comprimido é fácil 💊

Uma página web interativa que mostra, de forma lúdica e sem susto, que tomar um
comprimido é fácil: ele é pequeno, a garganta é bem maior do que ele, e a água
ajuda-o a descer.

Feita a pensar numa criança de ~11 anos com medo de tomar comprimidos, para ser
usada sobretudo no telemóvel.

## Como usar

Abre o ficheiro `index.html` num browser. Não precisa de servidor, instalação
nem ligação à internet — é um único ficheiro, sem imagens nem dependências
externas (todos os desenhos são SVG feitos à mão).

## O percurso

1. A mascote "Lili" aparece com um comprimido e um copo de água.
2. Arrasta-se o comprimido até à boca — ela abre a boca e recebe-o.
3. Arrasta-se o copo — o copo inclina-se, a água desce e ela engole.
4. Aparece o botão **Ver por dentro 🔍**.
5. A cena faz zoom para uma visão raio-X fofa: boca → garganta → estômago, com o
   comprimido a escorregar pela garganta (muito mais larga do que ele), empurrado
   pela água.
6. O comprimido chega ao estômago: estrelinha, brilhinhos e "Conseguiu!".
7. **Tentar de novo 🔄** reinicia tudo.

## Detalhes

- **Arrastar** funciona com rato e com o dedo (Pointer Events). A zona de acerto
  é generosa e um toque simples também conta, para não frustrar.
- **Tom gentil**: se o item for largado longe, a mensagem encoraja em vez de
  corrigir.
- **Som** opcional (sintetizado com a Web Audio API, sem ficheiros) e vibração
  nos momentos-chave; o botão 🔊 no canto liga/desliga.
- **Acessibilidade**: os itens são focáveis e aceitam Enter/Espaço; animações
  reduzidas quando o sistema pede `prefers-reduced-motion`.
- **Responsivo**, com transições de pelo menos 0,4 s e cores pastéis; a visão
  raio-X usa azul/violeta translúcido, sem ar clínico.
