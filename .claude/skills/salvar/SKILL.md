---
name: salvar
description: Salva um ponto de retorno do trabalho. Por padrão salva LOCAL (no próprio computador, sem conta nem internet). Backup na nuvem (GitHub) é opcional e pode ser conectado depois, sem perder nada.
---

# /salvar — guardar um ponto de retorno

Seus arquivos já ficam salvos na pasta o tempo todo — toda vez que o sistema
escreve algo, já está no seu computador. A pasta **é** o salvo. O `/salvar`
serve pra criar um **ponto de retorno**: uma "foto" do estado atual, pra você
conseguir voltar atrás depois se precisar.

> Importante: **salvar é local.** Não precisa de GitHub nem de internet.
> GitHub é só pra quem quiser uma cópia na nuvem — e dá pra conectar depois,
> a qualquer momento, sem perder nada.

## Padrão — salvar no próprio computador (sem conta, sem internet)

1. Resumir em uma linha o que mudou (ex.: "3 carrosséis novos + memória atualizada").
2. Criar o ponto de retorno:
   - Se o git estiver disponível: `git add -A` + `git commit` com uma mensagem
     clara em português. (Se ainda não for um repositório, rodar `git init`
     antes — continua 100% local, sem nuvem.)
   - Se a pessoa preferir não usar git: criar uma cópia datada da pasta em
     `backups/<data>/` (ou um `.zip`).
3. Confirmar: o que foi salvo e como voltar a um ponto anterior, em linguagem
   simples.

## Backup na nuvem (GitHub) — perguntar uma vez

Na **primeira vez** que o `/salvar` rodar sem backup na nuvem configurado,
**perguntar** ao usuário (e lembrar a resposta pra não repetir a cada vez):

> "Quer ligar um backup na nuvem (GitHub)? É grátis e opcional — guarda uma
> cópia online e sincroniza entre computadores. Posso deixar só no seu
> computador por enquanto e você liga quando quiser."

- Se **não**: seguir só local. Registrar a escolha em `_memoria/empresa.md`
  (seção "Configurações", ex.: "Backup: local, sem nuvem por enquanto") pra
  não perguntar de novo. Lembrar que dá pra ligar a nuvem a qualquer momento.
- Se **sim**: explicar em 1 linha, criar/logar a conta, criar o repositório
  (**privado** por padrão) e subir: `git remote add origin <url>` +
  `git push -u origin main`. **Tudo o que já foi salvo localmente sobe junto,
  com o histórico inteiro — nada se perde** (a "migração" sem dor). Registrar
  que a nuvem está ligada; daí em diante o `/salvar` manda pra nuvem também.

Se o usuário já tiver respondido antes, **não perguntar de novo** — só
respeitar a configuração registrada.

## Sempre

- Nunca subir segredos pra nuvem (`.env`, chaves, senhas). Se aparecerem no
  que vai ser salvo na nuvem, parar e avisar.
- Falar a língua do iniciante: "ponto de retorno" em vez de "commit", "cópia
  na nuvem" em vez de "push". Sem jargão de git.
