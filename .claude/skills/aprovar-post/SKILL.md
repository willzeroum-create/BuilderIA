---
name: aprovar-post
description: Faz a revisão final e a publicação de um conteúdo em blog, Instagram e Facebook num fluxo só — checa marca, erros e CTA antes de mandar pro ar.
---

# /aprovar-post — revisar e publicar

O último passo antes do "publicar". Garante que a peça está redonda e leva
pro ar, sem você abrir cinco ferramentas.

## O que fazer

1. Receber a peça (post, artigo, carrossel + legenda). Rodar o checklist:
   - **Marca** — tom e visual batem com `_memoria/preferencias.md` e `identidade/`?
   - **Erro** — gramática, datas, links, preço, @ e #.
   - **CTA** — tem um próximo passo claro?
   - **SEO** (se for blog) — título, meta, palavra-chave no lugar.
2. Mostrar os ajustes sugeridos e aplicar os aprovados.
3. Publicar conforme o que estiver conectado no ambiente:
   - Se houver integração/automação configurada (API, n8n, agendador),
     disparar a publicação.
   - Se não houver, gerar o pacote final pronto pra postar + as instruções
     de onde e como publicar em cada canal.

## Fechar

Confirmar o que foi publicado/agendado e onde. Registrar a saída em
`marketing/` e oferecer marcar no `/calendario`.
