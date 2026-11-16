# Layout em tela dividida (vertical 9:16)

O formato mais usado em Reels, TikTok e Shorts de quem fala para a câmera e quer ilustrar a fala: **apresentador embaixo, cenas em cima**. Valores em 1080 × 1920; no render, escale mantendo as proporções. Tendência, não regra: o perfil pode mudar qualquer medida.

## 1. Divisão do quadro
| Zona | Posição (1920 de altura) | O que fica |
|---|---|---|
| **Palco** (cenas) | topo até ~y 1000 | imagens, mapas, números, gráficos, textos em destaque |
| **Apresentador** | ~y 1000 até o fim | o vídeo da pessoa, com o rosto no centro da faixa |
| **Legenda** | logo abaixo do queixo (~y 1450–1600, ajustar pelo rosto) | até 3 palavras, uma linha |

- Ponto de partida: palco **~52%** e apresentador **~48%** da altura. Rosto grande vence: se o rosto ficar pequeno, aumente a faixa do apresentador e reduza o palco.
- **Rosto no terço superior da faixa do apresentador**, com a cabeça sem cortar. O zoom de câmera (punch, aproximação) acontece só nessa faixa.
- Uma linha fina, sombra suave ou degradê na junção separa as duas zonas. Sem linha dura se o perfil for mais limpo.
- **Sem cena:** o palco não fica vazio. Opções: o apresentador ocupa a tela cheia (a faixa dele cresce com movimento suave), ou o palco mostra um fundo da identidade do vídeo (cor, textura ou degradê) com a palavra-chave. Escolha no perfil e use sempre a mesma.

## 2. Área segura (vertical)
Nada essencial nos botões da lateral direita, na legenda do post (parte baixa) nem nas bordas que o celular corta.
- Margem lateral de **~64 px** de cada lado e de **~140 px** no topo.
- Coluna da direita (~180 px de largura, da metade para baixo): botões do app. Não colocar texto nem o elemento principal ali.
- Parte baixa (~260 px): legenda do post e barra. A legenda do vídeo fica **acima** disso.
- Confira em um quadro de cada trecho com a máscara de área segura do app (guia visual em cima do quadro).

## 3. Cenas no palco
- A cena é desenhada **para o retângulo do palco** (1080 × ~1000), nunca para o quadro inteiro.
- O elemento principal entra **centralizado no palco** desde o começo, mesmo com zoom maior.
- Cena em **tela cheia** (cobre o apresentador) é exceção: só para um momento de impacto (mapa grande, número gigante, revelação) e por pouco tempo. A fala continua por baixo. Sai revelando o apresentador.
- **Sobreposição sobre o apresentador** (etiqueta, ícone pequeno): fundo transparente, fora do rosto.

## 4. Transições
- **Entre cenas no palco:** troca rápida (~8–12 f) com a de saída mais curta que a de entrada: desliza para cima, empurra, ou dissolve com desfoque. Variar o tipo ao longo do vídeo.
- **Palco ↔ apresentador (cena some):** a cena sai para cima; o apresentador cresce para ocupar o espaço, ou o fundo da identidade entra.
- **Corte do apresentador** (jump cut): zoom alternado (ex.: 100% e 112%) na faixa dele, para disfarçar o corte, com o rosto sempre no mesmo lugar.
- A velocidade de cada movimento segue `oficio-motion.md` §1 e §2.

## 5. Legendas neste layout
- Posição: **logo abaixo do queixo**, não em cima da cena. Se o apresentador der zoom, a legenda desce junto naquele clipe.
- Até 3 palavras, uma linha, entrada quase imediata e sem fade de saída (detalhes em `etapa-legendas.md`).
- Nunca cobrir o rosto nem o texto da cena de cima.

## 6. Entrega
- **Render único 9:16** com as duas camadas montadas (apresentador + palco + legenda): o mais simples e previsível.
- **Para quem acaba no CapCut:** trilha de baixo com o apresentador (posição e escala já na faixa), trilha de cima com as cenas do palco renderizadas em MP4 na medida exata do palco, trilha de texto para as legendas. Ver `entrega-no-editor.md`.
- Resolução do render: 1080 × 1920 (ou 2160 × 3840 se a câmera for 4K). Taxa de quadros: a real do material.

## 7. Checklist por vídeo
- O rosto está grande o bastante no celular?
- Tem cena que invade a coluna de botões da direita?
- A legenda está perto do queixo e fora da cena?
- O palco nunca fica vazio sem decisão?
- A junção entre as duas zonas parece a mesma em todo o vídeo?
