---
name: ui-styling
description: Refina o visual de uma interface existente — espaçamento, cor, tipografia, estados, micro-interações — elevando o acabamento sem reescrever a estrutura.
---

# /ui-styling — polimento de interface

Pega uma tela que funciona mas parece "quase" e leva pro nível profissional.
É o acabamento que separa amador de produto.

## O que fazer

1. Olhar a interface atual (código ou print) e o `identidade/design-tokens`.
2. Refinar nos pontos que mais elevam o resultado:
   - **Espaçamento e ritmo** — escala consistente, respiro, alinhamento.
   - **Tipografia** — hierarquia, peso, altura de linha, contraste de tamanho.
   - **Cor** — uso correto de neutros, destaque só onde importa, contraste AA.
   - **Estados** — hover, foco, ativo, desabilitado, carregando, vazio, erro.
   - **Micro-interações** — transições sutis que dão polimento (sem exagero).
   - **Detalhes** — bordas, sombras, raios coerentes com os tokens.
3. Manter a estrutura; mexer no estilo.

## O que devolver

As mudanças aplicadas (ou um diff comentado) + um "antes/depois" do que
melhorou e por quê. Se faltar token, sugerir criar no `/design-system`.
