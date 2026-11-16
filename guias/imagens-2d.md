# Imagens, mapas e gráficos em 2D de alta qualidade

Como obter, conferir e animar as imagens que as cenas pedem (ver `fala-para-cena.md`). Só 2D. Detalhes que mudam com o tempo (APIs, limites, preços, licenças das fontes), pesquise na hora.

## 1. De onde vêm as imagens
| Precisa de… | Fonte, em ordem de preferência |
|---|---|
| Foto de lugar, objeto, evento, pessoa pública | Wikimedia Commons (licença clara, anote autor e licença); bancos com licença livre (Unsplash, Pexels, Pixabay: confira os termos de uso) |
| Ilustração, ícone | Iconify (Lucide, Phosphor, Tabler…), em SVG, recolorido pelo render |
| Logo | biblioteca local do perfil; depois logos oficiais em SVG e o Iconify (`logos`, `devicon`) |
| Print de site | navegador sem interface, na resolução do palco, da página pública |
| Imagem sob medida do conceito | **geração por IA**, se a pessoa tiver uma ferramenta ou API para isso; marcar como ilustração, nunca como "foto real" |
| Foto da própria pessoa, produto dela | a pessoa manda |

- **Nunca** pegar imagem sem licença clara. Sem licença, vira "a pessoa manda" ou muda de cena (texto, ícone, mapa).
- **Pessoa real** só quando a fala trata dela e a foto é pública e de contexto adequado. Sem insinuar nada que não foi dito.
- **Créditos:** um arquivo `creditos.txt` por vídeo (autor, licença, link) para a descrição, quando a licença pedir.

## 2. Checklist de qualidade (antes de entrar numa cena)
- **Resolução:** largura ≥ a do palco (1080 px) e, se vai ter zoom, ≥ 2160 px. Imagem pequena demais é descartada, nunca esticada.
- **Sem marca d'água, sem barra de cookie, sem texto cortado, sem borda estranha.**
- **Assunto reconhecível** em tela pequena de celular.
- **Proporção:** o crop vertical/quadrado preserva o assunto. Se não, outra imagem.
- **Consistência:** várias imagens no mesmo vídeo com luz e cor parecidas; se não, um tratamento único (leve correção de cor ou moldura igual).
- **Descartar o claramente errado** antes de mostrar opções: lugar homônimo, produto antigo, logo da empresa-mãe no lugar do produto.

## 3. Como animar uma imagem (sem 3D)
- **Entrada:** ~15 f, opacidade e foco primeiro, escala de ~92% a 100% com ease-out.
- **Vida depois que assenta:** deslize ou zoom lento e linear (1–4%) pelo tempo da cena (Ken Burns 2D). Nunca parada por mais de ~1,5 s.
- **Camadas:** fundo desfocado da própria imagem (ou da identidade) atrás, a imagem nítida na frente com sombra suave e cantos do perfil.
- **Destaque pontual:** círculo, seta ou recorte (zoom na parte citada) desenhado quando a fala aponta para ela.
- **Saída:** ~8 f, mais rápida que a entrada, um movimento só.

## 4. Mapas
O mapa é uma das cenas que mais valorizam um vídeo falado, e é desenhado em código, não baixado como imagem.
- **Dados:** contornos de países e estados de uma fonte aberta (ex.: Natural Earth) em GeoJSON/TopoJSON; cidades por coordenadas conhecidas; fundo de mapa com tiles só se a licença e o crédito forem cumpridos. Pesquise a fonte atual.
- **Desenho:** SVG ou canvas com projeção adequada (ex.: d3-geo), estilo plano da identidade (cor de terra, de água, de destaque).
- **Animação:**
  1. mapa abre em plano geral, com o destaque apagado;
  2. a câmera 2D (translate e scale) vai ao lugar, com ease-out e sem rotação;
  3. o país/estado acende, ou o ponto da cidade pulsa, **na palavra** que o cita;
  4. rotas e fronteiras se desenham no ritmo da fala (traço que cresce).
- **Rótulo:** nome do lugar em uma linha, fonte do perfil, perto do ponto sem cobrir.
- **Conferência:** o lugar certo? A escala não distorce (Groenlândia gigante)? Fronteiras atuais? Rótulo legível no celular?
- Várias cidades na mesma frase: o mapa percorre em ordem, uma de cada vez.

## 5. Gráficos e números
- **Dado vem da pessoa ou de fonte citada.** Nunca inventar número. Se a fonte for pública, cite o nome da fonte em letra pequena na cena.
- **Um dado protagonista:** destacar a barra, o ponto ou o trecho da linha que a fala cita; o resto em cor neutra.
- **Número grande:** conta até o valor no ritmo da palavra; unidade menor; uma linha de contexto.
- **Desenho em código** (SVG/canvas), com a paleta do perfil e eixos mínimos (só o que ajuda a ler).
- Para gráficos de dados reais com várias séries, siga o guia de visualização de dados que o ambiente tiver.

## 6. Ilustração conceitual
Para conceitos abstratos: ícone grande + palavra, ou diagrama simples (caixas e setas) desenhado no código, em traço limpo. Sem clip-art e sem emoji decorativo. Uma ideia por ilustração.

## 7. Biblioteca do perfil
Logos, ícones e fundos que voltam em vários vídeos ficam numa biblioteca local (`<pasta de ferramentas>/biblioteca/`), com um índice (nome, arquivo, fonte, licença). A etapa de assets olha ali primeiro.
