# Fase 17 — Deploy e entrada em operação

[Índice de todas as fases](../README.md) · [Cartão principal](https://github.com/vlabson/AgroGest/issues/73)

**Situação inicial:** Prevista; execução ainda não iniciada. O estado atualizado deve ser consultado no cartão.

## Atividades e subdocumentos

| Cartão | Guia Markdown |
|---|---|
| [F17.01](https://github.com/vlabson/AgroGest/issues/74) | [Preparação e decisões](01-preparacao-e-decisoes.md) |
| [F17.02](https://github.com/vlabson/AgroGest/issues/75) | [Execução e consolidação](02-execucao-e-consolidacao.md) |
| [F17.03](https://github.com/vlabson/AgroGest/issues/76) | [Validação e encaminhamento](03-validacao-e-encaminhamento.md) |

## Resultados da fase

[Registro dos resultados](registro-resultados.md). Os modelos preparados não representam entregas concluídas.

## Guia de execução

**Objetivo:** obter e validar publicação controlada, migração, testes de fumaça, comunicação e reversão.

**Entrada mínima:** Autorização específica e plano de implantação.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: publicação controlada, migração, testes de fumaça, comunicação e reversão.
3. Executar as [verificações da fase 17](../../00-processo/checklist-mestre-desenvolvimento-software.md#fase-17), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** registro-release.md e logs operacionais. Os espaços de registro já estão preparados nesta fase; preencher apenas com informações levantadas e validadas.

**Quem valida:** Responsável pela implantação executa; responsável pela operação acompanha e decide recuperação conforme o plano.

**Critério para avançar:** Fluxos críticos e integridade conferidos; versão disponível ou reversão executada e registrada.

**O que impede avançar:** Falha em um critério de entrada em operação, integridade comprometida ou autorização ausente.

**Relação com outras etapas:** Entrega à operação; falha relevante aciona recuperação e registro de incidente.

## Uso recorrente

Quando a fase se repetir em outro incremento ou versão, identificar o ciclo no cartão e nos registros. Preservar resultados anteriores; criar um novo cartão de execução quando necessário. Esta estrutura representa o processo conhecido, não funcionalidades de produto inventadas.
