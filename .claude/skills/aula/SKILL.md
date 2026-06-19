---
name: aula
description: Estrutura uma aula individual — objetivo, roteiro, exemplo prático e exercício — pronta pra gravar ou dar ao vivo, com material de apoio.
---

# /aula — estruturar uma aula

Pega um tópico e monta a aula pronta pra gravar: o aluno entra sem saber e
sai sabendo fazer.

## O que fazer

1. Definir: o tópico, o objetivo único da aula ("ao final, o aluno consegue
   X") e onde ela encaixa no curso (ler `saidas/curso/estrutura.md` se existir).
2. Montar o roteiro pedagógico:
   - **Gancho** — por que isso importa pro aluno (em 1 frase).
   - **Conceito** — o mínimo de teoria, explicado simples.
   - **Demonstração** — o passo a passo na prática, com um exemplo real.
   - **Exercício** — o que o aluno faz pra fixar (a parte que gera resultado).
   - **Fechamento** — recap + ponte pra próxima aula.
3. Gerar o **material de apoio**: resumo de uma página, checklist e/ou
   exercício pra baixar.

## O que devolver

- O roteiro da aula (pra gravar — encadear com `/roteiro` pra a locução).
- O material de apoio em `saidas/curso/<modulo>/`.
- Tom didático conforme `_memoria/preferencias.md`.
