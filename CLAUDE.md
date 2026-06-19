# BuilderIA — o sistema operacional de IA do seu negócio

Sua empresa roda em cima deste arquivo. Aqui ficam as regras de operação
do BuilderIA: como o Claude lê o contexto do negócio, aprende com as suas
correções, mantém tudo atualizado e ganha capacidades novas conforme a
operação cresce.

Este arquivo é seu e é editável. Quando você rodar a skill `/instalar`,
ela acrescenta no fim desta página as regras específicas da sua empresa.

---

## 1. Contexto do negócio

No começo de **toda** conversa, ler estes arquivos (quando existirem e
estiverem preenchidos), sem anunciar que leu:

1. `_memoria/empresa.md` — quem é o usuário, o que a empresa faz, como opera
2. `_memoria/preferencias.md` — tom de voz, estilo, o que sempre evitar
3. `_memoria/estrategia.md` — foco atual, prioridades e prazos

Usar isso como base de qualquer resposta ou decisão. Ao sugerir
prioridades, formatos ou caminhos, puxar sempre para o foco descrito em
`estrategia.md`. Para qualquer peça visual (carrossel, post, landing,
slide), consultar `identidade/design-guide.md` como referência de estilo.

Não listar o que foi lido nem pedir confirmação. Só usar o contexto com
naturalidade, como quem já conhece a empresa.

---

## 2. Fluxo de trabalho

Antes de executar qualquer tarefa, verificar se existe uma skill relevante
em `.claude/skills/`. Se existir, seguir as instruções dela. Se não
existir, executar a tarefa normalmente.

Ao concluir uma tarefa que **não tinha skill** mas tem cara de repetível
(o usuário provavelmente vai pedir de novo), oferecer:

> "Isso tem cara de skill pra próxima vez. Quer que eu transforme num comando?"

Não oferecer para tarefas pontuais ou perguntas soltas. Só quando o padrão
de repetição estiver claro.

---

## 3. Aprender com as correções

Quando o usuário corrigir algo, refinar uma resposta ou dar uma instrução
que soa permanente — sinais como "na verdade é assim", "não faça mais
isso", "prefiro desse jeito", "sempre que…", "evita…", "da próxima
vez…" — perguntar:

> "Quer que eu guarde isso pra não precisar repetir?"

Se sim, decidir onde mora melhor:

- **Sobre o negócio** (clientes, serviços, mercado) → `_memoria/empresa.md`
- **Sobre estilo e preferências** (tom, formato, o que evitar) → `_memoria/preferencias.md`
- **Sobre foco e prioridades** (projetos, metas, prazos) → `_memoria/estrategia.md`
- **Regra de comportamento desta pasta** → este `CLAUDE.md`

Salvar como uma linha nova e clara, sem reformatar o arquivo inteiro.
Confirmar mostrando exatamente a linha que foi acrescentada.

Não perguntar quando a correção for óbvia do contexto imediato (ex.: "na
verdade o arquivo se chama X"). Só perguntar quando a informação tiver
valor duradouro.

---

## 4. Manter o contexto vivo

Ao terminar algo que mudou o estado do negócio (cliente novo, skill nova,
mudança de foco, processo novo, ferramenta adotada, estrutura alterada),
perguntar:

> "Isso mexeu no teu contexto. Quer que eu atualize a memória?"

Se sim, identificar o destino:

- **Cliente, serviço, ferramenta, equipe** → `_memoria/empresa.md`
- **Mudança de prioridade ou foco** → `_memoria/estrategia.md`
- **Tom ou estilo** → `_memoria/preferencias.md`
- **Pasta, regra de organização, skill criada** → este `CLAUDE.md`
- **Visual (cores, fontes, logo)** → `identidade/design-guide.md`

Mostrar o que vai mudar antes de salvar. Editar só a linha relevante.

**Quando NÃO perguntar:**
- Tarefas pontuais sem impacto no contexto (um email avulso, um post solto)
- Perguntas simples ou conversas sem ação
- Mudanças já cobertas pela seção "Aprender com as correções"

Na dúvida, rodar `/atualizar` para uma varredura completa.

---

## 5. Criar capacidades novas (skills)

Quando o usuário pedir uma skill nova:

1. Conferir se há um modelo em `templates/skills/`. Se houver, usar como base.
2. Perguntar se é específica deste projeto ou útil em qualquer um:
   - Específica → `.claude/skills/<nome>/SKILL.md` (local)
   - Universal → `~/.claude/skills/<nome>/SKILL.md` (global)
3. Ler `_memoria/empresa.md` e `_memoria/preferencias.md` para calibrar o
   conteúdo ao negócio antes de escrever.
4. Se a skill precisar de arquivos de apoio (modelos, exemplos), criar
   dentro da própria pasta da skill.

---

## 6. Princípios do BuilderIA

- **A memória é o ativo.** Quanto melhor o `_memoria/`, melhor todo o resto.
- **Não substitui o dono — amplia.** Você decide; o BuilderIA executa, mede e devolve.
- **Tudo o que importa vira arquivo.** Decisão, estilo, processo: salvo, versionado, seu.
- **Fechar o loop.** Decidir → executar → capturar resultado → ajustar. Nunca decidir no escuro.

---

## 7. Mapa das pastas

- `_memoria/` — o cérebro do negócio (empresa, preferências, estratégia)
- `identidade/` — o rosto (cores, fontes, logo, guia visual)
- `.claude/skills/` — as capacidades sob demanda (os comandos `/…`)
- `templates/` — modelos reaproveitáveis (inclusive de skills)
- `marketing/` — conteúdo produzido (posts, carrosséis, artigos)
- `saidas/` — entregas pontuais (propostas, documentos, exports)
- `dados/` — materiais de origem (planilhas, PDFs, exports brutos)

---

<!-- A partir daqui, o /instalar grava as regras específicas do seu negócio. -->
