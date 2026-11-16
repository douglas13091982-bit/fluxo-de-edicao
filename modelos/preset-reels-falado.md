# Preset: Reels falado em tela dividida

Atalho do **modo rápido**. Para quem grava em pé ou sentado, falando para a câmera (conta histórias, explica), e quer cenas 2D que aparecem conforme fala. A fase 2 (entrevista) vira uma **confirmação** destas respostas, em vez de perguntar tudo do zero. A pessoa pode mudar qualquer linha.

## Respostas pré-preenchidas (confirmar em um bloco)
| Decisão | Valor do preset |
|---|---|
| Onde revisa | **sem programa**: o Claude entrega o vídeo pronto em MP4; o retoque fino é por pedido no chat. (Se a pessoa usar CapCut, trocar pelo caminho D de `entrega-no-editor.md`.) |
| Tipo e formato | apresentador falando para a câmera, **vertical 9:16**, 1080 × 1920, taxa de quadros real da câmera |
| Duração típica | 30 s a 3 min |
| Pasta | sem subpastas; arquivos na raiz da pasta do vídeo; o Claude cria só `_CLAUDE/` |
| Transcrição | tempo por palavra, mantendo hesitações; português; lista de termos do vídeo |
| Notas faladas | opcional ("nota de edição … fim da nota") |
| Cortes | ritmo apertado; corta erro e pausa longa; na dúvida, não corta e marca |
| Layout | **tela dividida**: palco (cenas) em cima, apresentador embaixo (`guias/layout-tela-dividida.md`) |
| Cenas | **2D de alta qualidade**: imagem, texto em destaque, número, lista, gráfico, mapa, ícone (`guias/fala-para-cena.md`); **sem 3D** |
| Ferramenta de animação | HyperFrames (ou outra escolhida na fase 2) |
| Câmera | zoom alternado só na faixa do apresentador; punch em ênfase |
| Som | efeitos leves de entrada/saída das cenas; música a pessoa decide |
| Legendas | pergunta a cada vídeo; até 3 palavras, uma linha, logo abaixo do queixo |
| Revisão | chat, por número da cena (`mo04`) ou por tempo |

## Etapas do fluxo no preset (de 9 para 7)
1. **iniciar** (briefing e papel dos arquivos)
2. **preparar** (inventário, transcrição, notas)
3. **cortes**
4. **cenas-mapa** (= motion-mapa com a divisão em batidas de `fala-para-cena.md`)
5. **assets** (imagens, ícones, prints; mapas e gráficos são desenhados no render)
6. **cenas-render** (= motion-render, no palco 1080 × ~1000)
7. **acabamento** (câmera + som + legendas + montagem final em 9:16)

Etapas 7, 8 e 9 do fluxo original podem ficar separadas se a pessoa preferir revisar uma por vez.

## Perfil inicial (preenche `identidade.md` e `estilo-motion.md`)
- **Material:** plano 2D, sombra suave, cantos arredondados; sem 3D. (default do preset)
- **Cores e fontes:** a definir com as referências (fase 3). Sem referência, propor 1 cor de destaque, 1 neutra clara e 1 escura, e uma fonte sem serifa de peso forte.
- **Densidade:** gancho denso (troca a cada 1,5–3 s), corpo com respiro, fechamento simples.
- **Entradas e saídas:** entrada ~15 f, saída ~8 f, variar o tipo de transição entre cenas.
- **Texto na cena:** ≥ 56 px, até ~6 palavras por linha, palavra-chave com punch.

## Como usar
Na fase 2, diga: "Vi que você grava falando para a câmera e quer cenas em cima, conforme a fala. Tenho um preset pronto para isso. Posso partir dele e só ajustar o que você quiser?" Com o "sim", confirme a tabela acima em um bloco, registre no `montagem.md` e siga para a fase 3 (referências).
