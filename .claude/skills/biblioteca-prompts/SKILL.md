---
name: biblioteca-prompts
description: Mantém uma biblioteca organizada de prompts reutilizáveis do negócio. Salva, busca e versiona prompts que funcionam, prontos pra reusar em qualquer momento.
---

# /biblioteca-prompts — o acervo de prompts da empresa

Guarda os prompts que dão certo num lugar só, organizados por uso. Em vez de
reinventar toda vez, a pessoa reusa o que já funciona.

## Onde mora

Os prompts ficam em `marketing/prompts/` (criar se não existir), um arquivo
`.md` por categoria (ex.: `vendas.md`, `conteudo.md`, `atendimento.md`).
Cada prompt tem: título, quando usar, o prompt em bloco de código, e
variáveis a preencher entre `[colchetes]`.

## Ações

- **Salvar** — receber um prompt (ou pegar o último gerado pelo `/prompt`),
  classificar na categoria certa e adicionar ao arquivo. Confirmar onde ficou.
- **Buscar** — o usuário descreve a situação ("preciso responder objeção de
  preço") e o comando devolve os prompts mais próximos do acervo.
- **Listar** — mostrar o índice da biblioteca por categoria.
- **Melhorar** — pegar um prompt existente e refinar (encadeia com `/prompt`).

## Regras

- Nunca duplicar: se já existe um parecido, oferecer atualizar em vez de criar.
- Manter os prompts genéricos com `[variáveis]`, pra servirem em vários casos.
- Calibrar pela voz em `_memoria/preferencias.md`.
