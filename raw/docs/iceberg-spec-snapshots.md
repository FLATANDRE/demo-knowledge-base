---
origem: https://iceberg.apache.org/spec/
acesso_em: 2026-11-07
titulo: "Apache Iceberg Table Specification — trecho sobre snapshots e metadados"
nota: "Trecho de estudo, transcrito da especificação oficial para a demo. Ingerir esta fonte no vídeo."
---

# Trecho da especificação do Iceberg: snapshots e metadados

> Fonte: https://iceberg.apache.org/spec/ — Apache Iceberg Table Specification. Conteúdo abaixo condensado para fins de estudo; a fonte canônica é a página oficial.

## Snapshots

Um snapshot é o estado da tabela em um ponto no tempo, incluindo o conjunto de todos os arquivos de dados. Os arquivos de dados de um snapshot são rastreados por manifestos. Em v1–v3, os manifestos ficam listados em um manifest list (um por snapshot); a partir da v4, são substituídos por um root manifest.

## Commits

Quando uma operação produz commit, a tabela escreve novo arquivo de metadados e o substitui atomicamente — o commit é atômico. Mudanças de metadado produzem novo arquivo de metadados commitado atomicamente; commits de dados podem criar novos snapshots.

## Observação de estudo

Perguntas que este trecho deve alimentar na wiki:

1. O que exatamente um snapshot referencia?
2. Quais mecanismos permitem consultar estados históricos da tabela (time travel) e quais custos de retenção isso envolve?
3. O que acontece com arquivos antigos após um commit?
