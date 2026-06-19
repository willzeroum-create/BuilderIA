---
name: agente
description: Desenha um agente/subagente do Claude sob medida para uma tarefa que se repete (qualificar lead, responder DM, triar e-mail). Define o papel, as instruções, as ferramentas e os limites.
---

# /agente — criar um agente sob medida

Cria um "funcionário de IA" especializado numa tarefa recorrente. Diferente
de um prompt avulso, um agente tem papel fixo, regras e roda sempre igual.

## O que fazer

1. Entender a tarefa: o que o agente faz, com que frequência, qual a entrada
   (o que ele recebe) e a saída (o que ele entrega).
2. Definir o agente:
   - **Papel** — quem ele é e o objetivo único dele.
   - **Instruções** — o passo a passo que ele segue sempre.
   - **Conhecimento** — o que precisa ler do `_memoria/` pra acertar o tom.
   - **Limites** — o que ele NÃO pode fazer; quando deve parar e chamar o humano.
   - **Formato de saída** — o padrão da resposta.
3. Escolher a forma de entrega que faz sentido:
   - Um **prompt de sistema** pronto pra colar (salvar na `/biblioteca-prompts`).
   - Ou uma **skill** em `.claude/skills/` se ele vai rodar dentro do BuilderIA.

## Fechar

Entregar o agente pronto + um exemplo de uso real. Sugerir testar com um
caso e ajustar. Se for virar rotina automática, encadear com `/tarefa-programada`.
