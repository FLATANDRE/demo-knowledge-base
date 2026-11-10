# Projeto de demonstração — Base de conhecimento pessoal com OpenCode

A wiki é construída ao vivo pelo agente: este repositório contém apenas o estado inicial.

## Estado inicial

```
demo-knowledge-base/
├── AGENTS.md                # Contrato do agente (copie o do seu projeto)
├── objetivos.md             # Metas de estudo (arquivo do humano)
├── PROMPTS-DA-DEMO.md       # Prompts exatos para digitar durante a gravação
└── raw/
    └── docs/
        └── iceberg-spec-snapshots.md   # Primeira fonte da demo
```

## Preparação antes de gravar

```bash
cd demo-knowledge-base
git init && git add -A && git commit -m "starter da base de conhecimento"
opencode
```

Abra a pasta `demo-knowledge-base/` como cofre no Obsidian (File → Open folder as vault).

## Fluxo da demo

1. Validação do contrato: "Leia o AGENTS.md e o índice..."
2. Ingestão da fonte local: `Ingerir raw/docs/iceberg-spec-snapshots.md`
3. Captura de URL: página de manutenção do Apache Iceberg
4. Consulta com citações (inclui pergunta sem resposta, para mostrar a lacuna declarada)
5. Modo estudo: "Quero estudar snapshots. Me teste antes de explicar."
6. Revisão espaçada: `Revisão`
7. Health-check e lint
