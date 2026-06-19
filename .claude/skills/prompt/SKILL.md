---
name: prompt
description: Transforma uma ideia solta num prompt profissional, estruturado e pronto pra colar em qualquer IA. Faz as perguntas que faltam e devolve o prompt otimizado, explicando por que ficou assim.
---

# /prompt — de ideia a prompt profissional

Você diz mais ou menos o que quer; o comando devolve um prompt que funciona
de verdade. É o coração da camada de IA do BuilderIA.

## O que fazer

1. Receber a ideia bruta do usuário ("quero um texto pra X", "me ajuda com Y").
2. Identificar o que falta pra um bom prompt e **perguntar só o essencial**
   (no máximo 2-3 perguntas), cobrindo:
   - **Objetivo** — o que a resposta precisa entregar.
   - **Papel/contexto** — quem a IA deve "ser" e o que ela precisa saber.
   - **Formato** — como a saída deve vir (tamanho, estrutura, tom).
   - **Restrições e exemplos** — o que evitar, e um exemplo do bom resultado.
3. Montar o prompt usando uma estrutura clara: papel → contexto → tarefa →
   formato de saída → restrições → (exemplo, se ajudar).

## O que devolver

- O **prompt final** num bloco de código, pronto pra copiar.
- 1-2 linhas de **por que ficou assim** (o que cada parte resolve), pra a
  pessoa aprender a fazer sozinha.
- Oferecer salvar na `/biblioteca-prompts` se for algo reutilizável.

Usar o tom de `_memoria/preferencias.md` quando o prompt for gerar conteúdo
da marca. Português PT-BR por padrão.
