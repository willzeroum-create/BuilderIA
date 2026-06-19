---
name: atualizar
description: Varre o projeto inteiro e atualiza a memória. Compara o que está nos arquivos com o que está em _memoria/ e identidade/, e propõe atualizações onde o contexto ficou desatualizado.
---

# /atualizar — sincronizar a memória

Faz uma varredura geral e deixa a memória do negócio em dia. Use quando
muita coisa mudou ou quando bater a dúvida "será que o sistema ainda sabe
de tudo?".

## O que fazer

1. Ler `_memoria/empresa.md`, `_memoria/preferencias.md`,
   `_memoria/estrategia.md` e a seção do negócio no `CLAUDE.md`.
2. Varrer o projeto procurando sinais de mudança:
   - Pastas novas em `marketing/`, `saidas/`, `dados/` ou novos projetos.
   - Skills novas em `.claude/skills/` que não estão documentadas.
   - Se for git, os commits desde a última atualização.
3. Comparar realidade × memória e listar as **divergências**: o que mudou
   no negócio e ainda não está registrado (cliente novo, foco novo,
   ferramenta nova, processo novo).

## O que devolver

Uma lista curta de atualizações propostas, agrupadas por arquivo de destino,
cada uma com a linha exata que seria adicionada/alterada. Perguntar:

> "Quer que eu aplique essas atualizações?"

Aplicar só as aprovadas, editando linha a linha — sem reformatar arquivos.
Se nada mudou, dizer isso em uma frase e encerrar.
