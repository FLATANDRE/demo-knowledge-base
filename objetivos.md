# Objetivos de estudo

> Arquivo do humano. O agente lê, mas não escreve aqui.

## Assunto: Apache Iceberg (formato de tabela aberto)

## Metas

1. Explicar a hierarquia de metadados (arquivo de metadados da tabela, manifest list ou root manifest, manifestos) e o que cada camada referencia.
2. Explicar snapshots: o que são, quando um commit cria um novo snapshot, e como habilitam time travel e rollback.
3. Entender o problema de arquivos pequenos e quando a compactação (`rewriteDataFiles`) ajuda.
4. Comparar Iceberg, Delta Lake e Hudi em schema evolution e hidden partitioning.

## Perguntas que quero saber responder ao final

- Como funciona um commit por dentro?
- Por que o Iceberg não sofre com o small files problem como o Hive?
- O que muda da v1 para a v4 da especificação?
