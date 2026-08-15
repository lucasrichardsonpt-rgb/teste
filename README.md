# Simulador: como o comprimido desce 💊

Um simulador para brincar e perder o medo de tomar comprimido. A personagem
(a Mia) faz as ações quando se clica nos botões, e o **raio-X** mostra, dentro
do corpo dela, o comprimido descendo pela garganta com a ajuda da água.

Feito para uma criança de ~11 anos usar sozinha, principalmente no celular.

## Como usar

Abra o `index.html` em qualquer navegador. Não precisa de internet, instalação
nem servidor — é um único arquivo, todo desenhado em SVG.

## Os botões

| Botão | O que acontece |
|---|---|
| 💊 **Colocar na língua** | A mão leva o comprimido até a boca e a câmera se aproxima: dá para ver ele em cima da língua, entre os dentes e a garganta |
| 💧 **Beber água** | Ela leva o copo à boca e bebe; de perto, a água enche a boca em volta do comprimido |
| 😮 **Engolir** | O comprimido vai para o fundo da garganta e desce até o estômago |
| 🔎 **Ver de perto** | Alterna entre a Mia inteira e o close da boca, na hora que quiser |
| 🔍 **Ligar raio-X** | O corpo fica transparente e azulado: aparecem a garganta e o estômago |
| 🔄 **Recomeçar** | Volta tudo ao início |

O raio-X pode ser ligado **a qualquer momento** — antes, durante ou depois.
O melhor é ligar antes de engolir: aí dá para ver o comprimido escorregando pela
garganta, empurrado pela água, até chegar no estômago.

Dá para engolir sem beber água antes — e aí o simulador mostra o comprimido
descendo bem mais devagar, para deixar claro por que a água ajuda.

## A ideia

O medo costuma vir de imaginar que o comprimido é grande demais para passar.
Então o simulador mostra o contrário, visualmente:

- a garganta é desenhada **bem mais larga** que o comprimido (umas 3 a 4 vezes),
  com uma medida marcando isso;
- a água aparece **empurrando** o comprimido para baixo;
- ele chega ao estômago e ganha uma estrelinha — nada de assustador.

## Detalhes técnicos

- Um único arquivo HTML, sem dependências, imagens ou fontes externas.
- Personagem e órgãos em SVG; as animações (braço, boca, engolir, descida) são
  feitas em JavaScript com `requestAnimationFrame`, o que permite acompanhar o
  movimento passo a passo em vez de um vídeo pronto.
- Sons suaves sintetizados na hora (Web Audio API) com botão 🔊 para desligar, e
  vibração nos momentos-chave.
- Responsivo: funciona em pé e deitado no celular; respeita
  `prefers-reduced-motion`.
