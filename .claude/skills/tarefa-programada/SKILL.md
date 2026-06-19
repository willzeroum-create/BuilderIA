---
name: tarefa-programada
description: Configura rotinas automáticas que rodam sozinhas num horário (relatório semanal, post diário, follow-up). Define o gatilho, o que roda e onde o resultado é entregue.
---

# /tarefa-programada — colocar no automático

Pega uma tarefa repetida e faz ela rodar sozinha no horário certo. É o
"loop fechado" da tese do BuilderIA na prática.

## O que fazer

1. Definir a rotina:
   - **O quê** — a ação que vai rodar (de preferência já uma skill existente).
   - **Quando** — frequência e horário (ex.: toda segunda 9h).
   - **Entrega** — onde o resultado aparece (arquivo no projeto, e-mail, mensagem).
2. Escolher o mecanismo conforme o ambiente:
   - Rotinas dentro do Claude Code → orientar o uso de agendamento/cron do
     próprio Claude Code (ex.: `/schedule`), descrevendo o comando a agendar.
   - Rotinas fora (sistema operacional, n8n/Make/Zapier) → gerar a
     configuração e o passo a passo de instalação.
3. Registrar a rotina criada numa lista em `_memoria/empresa.md` (seção
   "Automações"), pra não perder de vista o que roda sozinho.

## Regras

- Toda rotina automática precisa de um ponto de revisão humana: dizer **como
  conferir** se está funcionando e **como desligar**.
- Começar simples: uma rotina por vez, testada antes de confiar.
