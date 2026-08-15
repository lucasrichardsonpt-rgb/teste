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
| 💊 **Colocar comprimido** | A mão dela leva o comprimido até a boca, a boca abre e ele entra |
| 💧 **Beber água** | Ela leva o copo à boca, inclina, bebe e engole |
| 🔍 **Ligar raio-X** | O corpo fica transparente e azulado: aparecem a garganta e o estômago |
| 🔄 **Recomeçar** | Volta tudo ao início |

O raio-X pode ser ligado **a qualquer momento** — antes, durante ou depois.
O melhor é ligar antes de beber a água: aí dá para ver o comprimido escorregando
pela garganta, empurrado pela água, até chegar no estômago.

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
