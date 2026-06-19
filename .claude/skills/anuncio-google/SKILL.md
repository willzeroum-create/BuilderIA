---
name: anuncio-google
description: Monta uma campanha de Google Ads completa em CSV pronto para importar no Google Ads Editor — estrutura de campanha, grupos, palavras-chave, anúncios e extensões.
---

# /anuncio-google — campanha pronta pra importar

Monta a campanha inteira de Google Ads e entrega em CSV pra você importar no
Google Ads Editor — sem montar tudo na mão.

## O que fazer

1. Levantar o essencial: objetivo (vendas/leads/ligações), produto/oferta,
   orçamento diário, localização e página de destino. Ler `_memoria/empresa.md`.
2. Estruturar a campanha:
   - **Campanha** — tipo (Search, na maioria dos casos), orçamento, locais, lances.
   - **Grupos de anúncios** — por tema/intenção, bem segmentados.
   - **Palavras-chave** — por grupo, com correspondências (ampla modificada/
     frase/exata) e uma lista de **negativas** pra cortar desperdício.
   - **Anúncios responsivos** — títulos e descrições (vários, pra otimização).
   - **Extensões** — sitelinks, frases de destaque, snippets.
3. Gerar os **CSVs** no formato do Google Ads Editor, salvos em `saidas/ads/`.

## Fechar

Entregar os arquivos + um passo a passo curto de como importar. Recomendar o
acompanhamento (encadear com `/relatorio-ads`). Avisar sobre conversão/tag
no site pra medir resultado.
