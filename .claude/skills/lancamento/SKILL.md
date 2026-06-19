---
name: lancamento
description: Monta um plano de lançamento completo — cronograma, conteúdo de aquecimento, eventos de abertura/fechamento de carrinho, e-mails e anúncios — para vender um curso ou produto.
---

# /lancamento — plano de lançamento

Organiza o lançamento do começo ao fim, com datas e peças, pra você não
chegar no dia do carrinho aberto improvisando.

## O que fazer

1. Definir o básico: produto, oferta (usar `/oferta`), data de venda, meta
   (faturamento/alunos — ver `_memoria/estrategia.md`) e o tamanho da audiência.
2. Escolher o modelo conforme o caso: lançamento semente (lista pequena),
   lançamento com aquecimento + carrinho (CPL/aulas gratuitas), ou
   perpétuo. Recomendar o mais realista pra fase atual.
3. Montar o **cronograma** em fases:
   - **Aquecimento** — conteúdo que prepara o desejo (encadear `/calendario`, `/roteiro`).
   - **Evento** — aulas/lives de pré-lançamento, se for o caso.
   - **Abertura de carrinho** — oferta no ar, urgência real.
   - **Fechamento** — últimas chamadas, bônus por tempo limitado.
4. Listar as **peças por dia**: e-mails, posts, anúncios (`/anuncio-google`),
   página de vendas, VSL (`/vsl`).

## O que devolver

- O plano com calendário (fase → data → peça → canal → CTA), em
  `saidas/lancamento/`.
- A sequência de e-mails de carrinho aberto/fechamento.
- Os números-alvo por etapa pra acompanhar (e revisar depois com `/revisar`).
