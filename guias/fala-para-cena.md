# Da fala para a cena (o vídeo que se monta conforme a pessoa fala)

É o coração do estilo "falou, apareceu": enquanto a pessoa fala, entram imagens, textos, números, mapas e gráficos que ilustram **exatamente** aquela frase. Este guia descreve como transformar a transcrição em cenas, com tempo certo e qualidade. Vale para qualquer formato; no vertical com tela dividida, leia junto com `layout-tela-dividida.md`.

Tudo aqui é tendência, não regra. Quanto aparece, o visual e o ritmo são do perfil.

## 1. O princípio
- **A fala decide a cena.** Nada de template: para cada ideia, a forma visual que explica *aquela* ideia (ver tabela do §3).
- **Uma coisa protagonista por vez** no espaço de cima. Quando a ideia muda, a cena muda.
- **Mostrar a coisa de verdade** (foto, mapa, print, número) explica mais que um card genérico com o nome dela.
- **Nunca mentir com imagem:** o que aparece tem de ser o que foi dito (lugar certo, pessoa certa, dado certo). Na dúvida, texto em destaque no lugar de uma imagem que "parece".

## 2. O pipeline (um script faz cada passo; o Claude decide só o que é de texto)
1. **Transcrição com tempo por palavra** (etapa preparar). Retranscrever trechos com som e sem palavra.
2. **Divisão em batidas (beats).** Um beat é um trecho da fala que carrega **uma ideia visualizável**: um lugar, uma pessoa, um número, uma lista, uma comparação, um conceito, uma frase de impacto. O script propõe pelas pausas e pontuação; o Claude relê por frase e ajusta. Tamanho típico: 2–6 s. Beat sem nada a mostrar fica sem cena (o apresentador sozinho também é um bom plano).
3. **Classificação do beat** pela tabela do §3: qual tipo de cena, qual palavra-gatilho, o que precisa de asset.
4. **Lista de assets** (imagem, mapa, ícone, print). Cada um com tipo e termo de busca. Ver `imagens-2d.md`.
5. **Plano numerado** (`mo01`, `mo02`…) com tempo, tipo de cena, gatilho e asset. A pessoa aprova ou risca por número. Gancho primeiro e com mais detalhe.
6. **Assets** são buscados ou gerados; o que faltar vai marcado.
7. **Render** de cada cena com o ofício de `oficio-motion.md`, no tempo das palavras-gatilho.
8. **Montagem** sobre o vídeo, câmera, som e legendas, como nas outras etapas.

## 3. Tabela: o que a pessoa diz → o que aparece
| A fala traz… | Cena | Como construir |
|---|---|---|
| Um lugar, país, cidade, rota | **Mapa** | Mapa 2D limpo, zoom no lugar, ponto ou rota desenhada no tempo da fala. Ver `imagens-2d.md` §4 |
| Uma pessoa, marca, produto, objeto real | **Imagem** (foto, logo, print) | Imagem em alta qualidade com entrada suave e leve movimento (Ken Burns de 2D) |
| Um número, porcentagem, valor | **Número grande** | O número conta até o valor no tempo da palavra; unidade pequena; contexto em uma linha |
| Uma comparação (antes/depois, A vs B) | **Duas colunas ou divisão** | Os dois lados entram um de cada vez, na ordem da fala |
| Uma lista ou passos ("primeiro… segundo…") | **Lista em cascata** | Cada item entra **na palavra** que o diz; o grupo fica centralizado |
| Evolução no tempo, crescimento, queda | **Gráfico simples** | Linha ou barra desenhada no ritmo da fala; um dado só destacado |
| Linha do tempo, datas | **Timeline** | Eixo que avança; cada data entra quando é dita |
| Um conceito abstrato | **Metáfora visual 2D** | Ilustração, ícone grande ou diagrama simples desenhado no código |
| Uma frase de impacto, uma regra, uma citação | **Texto em destaque** | Palavra-chave com punch na hora em que é dita |
| Uma ferramenta, site ou app citado | **Print ou logo** | Print de página pública ou logo oficial, com destaque pontual |
| Uma pergunta ao espectador | **Ponto de interrogação ou texto** | Curto, sem enfeite |

Várias ideias na mesma frase: uma cena por ideia, na ordem em que a fala as diz, com transição rápida entre elas.

## 4. Ritmo
- **Gancho (primeiros ~3–8 s):** o mais denso; a primeira cena aparece logo na primeira ideia, sem esperar. Troca a cada 1,5–3 s.
- **Corpo:** uma cena por ideia, tipicamente 2–6 s; entre cenas, respiro com só o apresentador, para o olho descansar.
- **Fechamento:** menos cenas; a chamada final com texto simples.
- **Não repetir a mesma fórmula** (mesma entrada, mesma transição) em duas cenas seguidas. Variar o tipo.
- **Tempo de leitura:** com texto, a cena fica ~1–1,5 s depois da última palavra, salvo se a ideia seguinte já começou.
- **Sincronia:** a cena entra **na palavra-gatilho** (tempo da transcrição), nunca num intervalo fixo. Se a palavra vem no meio da frase, a cena entra nela, não no começo.

## 5. Regras de qualidade (2D de alta qualidade)
- **Só 2D**, salvo se o perfil pedir outra coisa: camadas planas com profundidade por sombra suave, desfoque de fundo e parallax leve. Nada de rotação 3D, `perspective` ou mockup 3D.
- **Resolução:** imagem a no mínimo a largura da área de cima do layout; de preferência 2× (para o zoom não borrar). Ver o checklist em `imagens-2d.md`.
- **Enquadramento:** o assunto da imagem no centro; o corte (crop) vai no que importa, não no que sobrou.
- **Texto:** mínimo 56 px em 1080 de largura, poucas palavras (até ~6 por linha), alto contraste, dentro da área segura.
- **Cor e fonte:** só as do perfil (`identidade.md`). Sem emoji decorativo, sem clip-art.
- **Uma sombra e uma borda coerentes** em todos os cards do vídeo: é o que faz tudo parecer do mesmo vídeo.

## 6. Armadilhas
- Imagem de banco genérica ("pessoa apertando a mão") num trecho que pedia dado: texto ou número explica melhor.
- Mapa errado (cidade homônima, fronteira que mudou): confira o lugar pelo contexto do vídeo antes de desenhar.
- Cena que entra **antes** da palavra: o espectador vê a resposta antes da pergunta. Entrar na palavra, ou até ~0,1 s depois.
- Cena longa demais num trecho sem ideia nova: corta para o apresentador.
- Tudo com zoom e impacto: vira ruído. Ênfase com critério.
- Pessoa real em imagem de apoio sem contexto: nunca insinuar o que a pessoa não disse. Foto de pessoa pública só em contexto jornalístico claro.

## 7. Como conferir
Renderize e veja três quadros por cena (entrada, meio, saída). Cada cena tem de responder "sim" a: aparece na palavra certa? Mostra o que foi dito? Legível no celular? Fica dentro da área segura? Combina com a cena anterior sem repetir?
