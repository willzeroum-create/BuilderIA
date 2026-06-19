---
name: foto-ia
description: Gera imagens por IA para conteúdo, anúncios e capas — fundos, cenas, mockups e ilustrações — no estilo visual da marca. Escreve o prompt de imagem e produz a arte.
---

# /foto-ia — imagem por IA na cara da marca

Cria a imagem que falta — sem banco de imagem genérico. Fundo de carrossel,
cena de anúncio, ilustração de post.

## O que fazer

1. Entender o uso: onde a imagem entra (post, anúncio, capa, thumbnail),
   proporção e clima. Ler `identidade/design-guide.md` pra estilo e cores.
2. Escrever um **prompt de imagem** forte: sujeito, cenário, estilo,
   iluminação, paleta (puxar da identidade), enquadramento e proporção.
   (Pode encadear com `/prompt` pra refinar.)
3. Gerar a imagem. Se a ferramenta de geração Higgsfield estiver disponível
   no ambiente, usar ela; senão, entregar o prompt pronto pra colar na
   ferramenta de imagem do usuário.

## O que devolver

- O prompt de imagem usado (pra reusar/ajustar).
- A imagem gerada (ou variações), salva em `marketing/imagens/`.
- Se for pra texto em cima (thumbnail/capa), entregar uma versão "limpa"
  com área de respiro pro texto.

Evitar gerar rostos de pessoas reais/identificáveis sem necessidade e marcas
de terceiros.
