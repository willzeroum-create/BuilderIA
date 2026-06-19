---
name: abrir
description: Abre uma sessão de trabalho. Carrega a memória do negócio (empresa, preferências, estratégia), verifica pendências e devolve um resumo curto de onde paramos e o que faz sentido fazer hoje.
---

# /abrir — começar a sessão

Use no início de cada sessão de trabalho. Ele carrega o contexto e te
coloca pronto pra agir.

## O que fazer

1. Ler `_memoria/empresa.md`, `_memoria/preferencias.md` e
   `_memoria/estrategia.md`. (Se algum estiver só com o template, avisar que
   vale rodar `/instalar` ou preencher.)
2. Ler a seção específica do negócio no fim do `CLAUDE.md`, se existir.
3. Olhar rapidamente o que mudou desde a última vez (arquivos novos em
   `marketing/` e `saidas/`; se for repositório git, os últimos commits).

## O que devolver

Um resumo **curto** (não um relatório), no tom definido em `preferencias.md`:

- **Foco atual:** a frase de `estrategia.md`.
- **Onde paramos:** 1-2 linhas do que foi feito por último.
- **Sugestão de hoje:** 2-3 ações que empurram o foco atual pra frente,
  em ordem de prioridade.
- **Pendências**, se houver alguma clara.

Terminar perguntando: "Por onde você quer começar?"

Não despejar o conteúdo bruto dos arquivos. O usuário quer o destilado, não a leitura.
