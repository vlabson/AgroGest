# Fase 07 — Modelagem de dados

[Índice de todas as fases](../README.md) · [Cartão principal](https://github.com/vlabson/AgroGest/issues/33)

**Situação inicial:** Prevista; execução ainda não iniciada. O estado atualizado deve ser consultado no cartão.

## Atividades e subdocumentos

| Cartão | Guia Markdown |
|---|---|
| [F07.01](https://github.com/vlabson/AgroGest/issues/34) | [Preparação e decisões](01-preparacao-e-decisoes.md) |
| [F07.02](https://github.com/vlabson/AgroGest/issues/35) | [Execução e consolidação](02-execucao-e-consolidacao.md) |
| [F07.03](https://github.com/vlabson/AgroGest/issues/36) | [Validação e encaminhamento](03-validacao-e-encaminhamento.md) |

## Resultados da fase

[Registro dos resultados](registro-resultados.md). Os modelos preparados não representam entregas concluídas.

## Guia de execução

**Objetivo:** obter e validar estruturas, restrições, histórico, origem e qualidade dos dados, migração.

**Entrada mínima:** Domínio e necessidades de persistência; interação com arquitetura.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: estruturas, restrições, histórico, origem e qualidade dos dados, migração.
3. Executar as [verificações da fase 07](../../00-processo/checklist-mestre-desenvolvimento-software.md#fase-07), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** modelo-dados.md e migrations. Os espaços de registro já estão preparados nesta fase; preencher apenas com informações levantadas e validadas.

**Quem valida:** Desenvolvedor valida restrições e persistência; responsável pelos dados confirma histórico e origem.

**Critério para avançar:** Persistência sustenta regras e consultas críticas; riscos de perda e inconsistência tratados.

**O que impede avançar:** Persistência não sustenta uma regra essencial ou há risco de perda de histórico sem tratamento.

**Relação com outras etapas:** Definir junto à arquitetura; orientar migrations e preparação dos dados.

## Uso recorrente

Quando a fase se repetir em outro incremento ou versão, identificar o ciclo no cartão e nos registros. Preservar resultados anteriores; criar um novo cartão de execução quando necessário. Esta estrutura representa o processo conhecido, não funcionalidades de produto inventadas.
