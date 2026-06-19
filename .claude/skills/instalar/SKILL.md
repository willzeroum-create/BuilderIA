---
name: instalar
description: Configura o BuilderIA pela primeira vez. Entrevista o usuário sobre o negócio, preenche a memória (_memoria/) e o guia de identidade, e grava as regras específicas no fim do CLAUDE.md. Roda uma vez só.
---

# /instalar — ligar o BuilderIA

Este comando roda **uma única vez**, na primeira abertura. Ele transforma
um BuilderIA genérico no sistema operacional de UMA empresa específica.

> **Tom:** comece com uma saudação humana e simples e vá **direto** pra
> entrevista. **Nunca** exponha detalhes técnicos internos pro usuário (não
> falar de "clone", "skills carregadas", "harness", "repositório", etc.) —
> ele não quer saber disso, só quer começar.

## Antes de começar

1. **Desamarrar do repositório de origem.** Esta pasta veio de um clone do
   repositório do produto, então ainda aponta pra ele. Pra virar um projeto
   limpo e do próprio usuário, remover esse vínculo **sem alarde**:
   `git remote remove origin` (se existir). Assim nada que o usuário criar
   vai parar no repositório do produto, e o `/salvar` poderá montar a nuvem
   dele depois.
2. Conferir se `_memoria/empresa.md` já está preenchido (não só o template).
   Se já estiver, avisar que o sistema já foi instalado e perguntar se o
   usuário quer **refazer** ou só **complementar**.
3. Explicar em uma frase o que vai acontecer: "Vou te fazer algumas
   perguntas rápidas sobre o negócio pra deixar o sistema com a sua cara."

## A entrevista

Fazer **uma pergunta por vez**, em linguagem simples, sem jargão. Não
despejar tudo de uma vez. Reaproveitar o que o usuário já disser para
encadear a próxima pergunta. Blocos:

**Bloco 1 — A empresa** (vai pra `_memoria/empresa.md`)
- Como é o seu nome e o nome da empresa?
- Em uma frase, o que vocês vendem?
- Quem é o cliente ideal? (perfil + principal dor)
- Como o cliente chega até você hoje? E como você entrega?
- O que faz o cliente escolher você e não o concorrente?

**Bloco 2 — A voz** (vai pra `_memoria/preferencias.md`)
- Como você quer que o sistema fale com você e nos textos? (próximo? formal? direto?)
- Tem alguma coisa que você NÃO quer ver nunca? (palavra, promessa, clichê)
- Se tiver um texto seu (post, anúncio, email), cole aqui — é o que melhor calibra a voz.

**Bloco 3 — O foco** (vai pra `_memoria/estrategia.md`)
- Qual é o objetivo número 1 dos próximos 2-3 meses?
- Tem uma meta com número e data? (ex.: 50 vendas até tal dia)

**Bloco 4 — A marca** (vai pra `identidade/design-guide.md`)
- Tem cores e fonte definidas? (se não, sugerir a partir do segmento)
- Tem logo? Se sim, peça pra salvar em `identidade/logo.png`.
- Em 3 palavras, como a marca deve parecer? (ex.: moderna, confiável, premium)

## Gravar

À medida que avança (ou no fim), preencher:
- `_memoria/empresa.md`, `_memoria/preferencias.md`, `_memoria/estrategia.md`
- `identidade/design-guide.md`
- No fim do `CLAUDE.md`, abaixo do comentário marcador, escrever um bloco
  curto **"## Sobre a [empresa]"** com o resumo do negócio, foco atual,
  marca e regras de organização específicas. Espelhar o tom das seções de
  cima. Não reformatar o resto do arquivo.

## Fechar

- Mostrar um resumo do que foi configurado.
- Sugerir renomear a pasta `BuilderIA/` para o nome da empresa.
- Apontar os primeiros comandos úteis: `/abrir` no começo de cada sessão e
  `/salvar` para versionar.
- Lembrar que o sistema aprende sozinho dali pra frente (correções viram memória).
