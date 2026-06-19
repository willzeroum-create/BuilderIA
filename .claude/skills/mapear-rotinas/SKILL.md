---
name: mapear-rotinas
description: Descobre o que o usuário repete no dia a dia e transforma essas repetições em skills personalizadas. Entrevista leve sobre a rotina e propõe comandos novos sob medida.
---

# /mapear-rotinas — transformar repetição em comando

Acha as tarefas que você refaz toda semana e vira cada uma num comando.
É como o BuilderIA cresce junto com o negócio.

## O que fazer

1. Olhar o histórico recente (arquivos em `marketing/`/`saidas/`, commits)
   e a estratégia atual pra levantar hipóteses de tarefas repetidas.
2. Fazer uma entrevista curta:
   - O que você faz **toda semana** que dá trabalho manual?
   - O que você sempre pede do mesmo jeito?
   - O que você adia porque é chato/repetitivo?
3. Pra cada repetição clara, propor uma skill: nome do comando, o que faria,
   e que informação ele pediria a cada uso.

## Fechar

Listar as skills sugeridas em ordem de impacto. Para cada uma aprovada,
criar a pasta em `.claude/skills/<nome>/SKILL.md` seguindo o padrão do
sistema (frontmatter `name`/`description` + passos claros), calibrada pelo
`_memoria/`. Confirmar mostrando os comandos novos disponíveis.
