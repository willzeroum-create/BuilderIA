---
name: analisar-dados
description: Lê arquivos de dados (CSV, XLSX, PDF) e gera um resumo executivo com os números que importam, tendências e recomendações — sem o usuário precisar montar planilha.
---

# /analisar-dados — resumo executivo de qualquer dado

Joga a planilha/PDF aqui e recebe de volta o que ela quer dizer: os números
que importam, o que mudou e o que fazer.

## O que fazer

1. Ler o(s) arquivo(s) de `dados/` (CSV, XLSX, PDF). Entender o que cada
   coluna/seção representa. Confirmar com o usuário se algo estiver ambíguo.
2. Extrair o essencial:
   - Os **indicadores-chave** do conjunto (totais, médias, variações).
   - **Tendências** e padrões (crescimento, queda, sazonalidade, outliers).
   - **Destaques e alertas** (o melhor, o pior, o que foge do normal).
3. Relacionar com o objetivo do negócio (ler `_memoria/estrategia.md`).

## O que devolver

- Um **resumo executivo** no topo (3-5 linhas, direto ao ponto).
- Os números-chave em tabela e, se ajudar, uma descrição de gráfico.
- **Recomendações** acionáveis a partir dos dados.
- Salvar em `saidas/analises/<nome>-<data>.md`.

Linguagem simples. Sempre dizer o que o dado significa pra decisão, não só o número.
