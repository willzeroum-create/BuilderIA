---
name: relatorio-ads
description: Lê os exports de Google Ads e Meta Ads e devolve um relatório semanal com métricas, alertas e recomendações de otimização em linguagem simples.
---

# /relatorio-ads — relatório de anúncios com recomendação

Pega os números das campanhas e traduz em "o que está indo bem, o que está
queimando dinheiro e o que fazer essa semana".

## O que fazer

1. Receber os exports (CSV/planilha) do Google e/ou Meta. Ler `_memoria/`
   pro contexto de meta e ticket.
2. Calcular o que importa: investimento, cliques, CTR, CPC, conversões, CPA,
   ROAS/retorno. Comparar com a semana anterior.
3. Gerar **alertas** automáticos:
   - Campanha/anúncio com CPA acima do aceitável.
   - Verba indo pra termo que não converte.
   - Anúncio com CTR baixo (criativo cansado).
   - Oportunidade de escalar o que está performando.
4. Traduzir tudo em **3-5 ações** concretas pra semana, em ordem de impacto.

## O que devolver

O relatório em `saidas/ads/relatorios/<data>.md`: resumo no topo (1 parágrafo
sem jargão), tabela de métricas, alertas e ações recomendadas. Linguagem de
dono, não de gerente de tráfego.
