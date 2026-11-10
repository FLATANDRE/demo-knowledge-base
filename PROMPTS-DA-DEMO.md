# Prompts da demo

## 1. Validação do contrato

```
Leia o AGENTS.md e o índice. Em 5 frases, como você opera nesta base?
```

Resposta esperada do agente: três camadas, fluxos, permissões, quem escreve o quê.

## 2. Ingestão da fonte local 

```
Ingerir raw/docs/iceberg-spec-snapshots.md
```

Quando ele perguntar o que enfatizar, responda:

```
Enfatize a relação entre manifest list, manifestos e snapshot, e o que é commitado atomicamente.
```

## 3. Captura de página web 

```
Capture a URL https://iceberg.apache.org/docs/latest/maintenance/ e depois ingira a nova fonte
```

Autorize a gravação do arquivo derivado em raw/ quando ele pedir.

## 4. Consulta com citações 

```
O que a wiki diz sobre compactação de arquivos pequenos?
```

Pergunta sem resposta na wiki (para mostrar a lacuna declarada):

```
O que a wiki diz sobre transactional catalogs?
```

## 5. Modo estudo 

```
Quero estudar snapshots. Me teste antes de explicar.
```

Responda de propósito de forma incompleta na primeira pergunta, para mostrar a correção com citações.

## 6. Revisão espaçada 

```
Revisão
```

## 7. Health-check e lint 

```
Rode um health-check na wiki e depois um lint
```
