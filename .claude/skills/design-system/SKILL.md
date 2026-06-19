---
name: design-system
description: Cria e mantém o design system do negócio — tokens de cor, tipografia, espaçamento e componentes — em CSS/JSON reutilizáveis para site, app e peças.
---

# /design-system — o sistema de design

Transforma a identidade da marca em **tokens e componentes** reutilizáveis,
pra que tudo (site, app, peças) saia consistente e rápido.

## O que fazer

1. Partir de `identidade/design-guide.md`. Se não existir, rodar `/brand` antes.
2. Definir os **tokens**:
   - **Cores** — primária, secundária, neutros, estados (sucesso/erro/aviso).
   - **Tipografia** — escala de tamanhos, pesos, alturas de linha.
   - **Espaçamento** — escala (4/8px), raios de borda, sombras.
3. Definir **componentes** base: botões, inputs, cards, badges — com estados
   (normal, hover, foco, desabilitado).
4. Gerar os arquivos: `identidade/design-tokens.css` (variáveis CSS) e
   `identidade/design-tokens.json`, mais um guia rápido de uso.

## Fechar

Entregar os tokens prontos pra importar no site/app (encadear com
`/frontend-design` e `/ui-styling`). Manter sincronizado quando a marca mudar.
