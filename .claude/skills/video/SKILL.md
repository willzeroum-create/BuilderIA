---
name: video
description: Gera vídeos curtos por IA (hero video, animação de produto, cena cinematográfica, foto que ganha movimento) para anúncios, redes e páginas, no estilo da marca.
---

# /video — vídeo por IA

Cria o vídeo curto que dá vida ao conteúdo — abertura cinematográfica,
produto em movimento, cena de anúncio. Sem set de filmagem.

## O que fazer

1. Definir o uso: onde entra (anúncio, Reels, topo de página), duração,
   proporção (9:16, 1:1, 16:9) e a sensação desejada. Ler `identidade/design-guide.md`.
2. Escrever o **prompt de vídeo**: cena, movimento de câmera, ritmo, estilo e
   paleta da marca. Se partir de uma imagem (foto vira vídeo), indicar o ponto
   de partida (pode vir do `/foto-ia`).
3. Gerar usando a ferramenta de vídeo Higgsfield, se disponível no ambiente;
   senão, entregar o prompt + as configurações prontas pra usar na ferramenta
   do usuário.

## O que devolver

- O prompt/config usado.
- O vídeo gerado (ou variações), salvo em `marketing/videos/`.
- Sugestão de trilha/legenda e do corte ideal pro formato.

Encadear com `/roteiro` quando o vídeo precisar de narração/estrutura.
