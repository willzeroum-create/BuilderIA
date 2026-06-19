---
name: frontend-design
description: Cria interfaces e páginas web de alto nível (landing page, site, área de membros) com código limpo e design profissional, fugindo do visual genérico de IA.
---

# /frontend-design — interface web de verdade

Cria páginas e telas com cara de produto profissional — não o template
genérico de sempre. Código limpo + design com intenção.

## O que fazer

1. Definir: o que é a tela (landing, site, dashboard, área de membros), o
   objetivo e o stack (HTML/CSS, React, etc.). Ler `identidade/` e os tokens
   do `/design-system` (se existirem).
2. Projetar antes de codar:
   - **Estrutura** — hierarquia da página, seções, fluxo do olho.
   - **Conversão** (se for landing) — gancho, prova, oferta, CTA repetido.
   - **Responsivo** — pensar mobile primeiro.
   - **Personalidade** — escolhas visuais que fogem do padrão (tipografia,
     espaçamento generoso, detalhe de marca), sem cair no exagero.
3. Implementar com código limpo, acessível e performático. Usar os tokens da
   marca pra cor/tipo/espaçamento.

## O que devolver

O código pronto (em `app/` ou no projeto indicado) + uma nota das decisões de
design. Encadear com `/ui-styling` pro polimento e `/ui-ux-pro-max` pra
revisão de UX. Refinar junto com o usuário até ficar redondo.
