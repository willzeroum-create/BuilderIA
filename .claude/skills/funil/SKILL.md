---
name: funil
description: Desenha o funil de vendas e a escada de produtos do negócio — da isca ao alto ticket, com order bumps e upsells. Mapeia cada etapa, a oferta de cada uma e a passagem entre elas.
---

# /funil — desenhar o funil e a escada de produtos

Monta o caminho que leva um estranho a virar cliente e depois a comprar de
novo, com cada degrau de preço no lugar certo.

## O que fazer

1. Levantar o que existe: produtos atuais, preços, e por onde o cliente entra.
2. Montar a **escada de valor**:
   - **Isca / topo** — algo de baixo (ou nenhum) custo que gera o primeiro "sim".
   - **Produto principal** — a oferta central.
   - **Order bump** — um "leva também" barato na hora do checkout.
   - **Upsell / downsell** — a próxima oferta logo após a compra.
   - **Recorrência** — algo que gera receita mensal.
   - **Alto ticket** — a oferta premium pra quem quer mais.
3. Definir, pra cada etapa: a oferta, o preço, a taxa de conversão esperada e
   a chamada pra próxima etapa (o que faz a pessoa avançar).
4. Mapear os **pontos de captura** (onde pega contato) e o **acompanhamento**
   (e-mail/mensagem) entre as etapas.

## O que devolver

- O diagrama do funil em texto (etapa → oferta → preço → próximo passo).
- Os gargalos prováveis e o que priorizar primeiro.
- Encadear com `/oferta` (cada degrau) e `/precificar` (os valores).

Se for um funil de info-produto/curso, alinhar com `/lancamento`.
