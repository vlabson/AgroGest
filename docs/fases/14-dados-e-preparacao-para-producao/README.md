# Fase 14 — Dados e preparação para produção

[Índice de todas as fases](../README.md) · [Cartão principal](https://github.com/vlabson/AgroGest/issues/61)

**Situação inicial:** Prevista; execução ainda não iniciada. O estado atualizado deve ser consultado no cartão.

## Atividades e subdocumentos

| Cartão | Guia Markdown |
|---|---|
| [F14.01](https://github.com/vlabson/AgroGest/issues/62) | [Preparação e decisões](01-preparacao-e-decisoes.md) |
| [F14.02](https://github.com/vlabson/AgroGest/issues/63) | [Execução e consolidação](02-execucao-e-consolidacao.md) |
| [F14.03](https://github.com/vlabson/AgroGest/issues/64) | [Validação e encaminhamento](03-validacao-e-encaminhamento.md) |

## Resultados da fase

[Registro dos resultados](registro-resultados.md). Os modelos preparados não representam entregas concluídas.

## Guia de execução

**Objetivo:** obter e validar migração ensaiada, integridade, cópia de segurança, restauração e recuperação.

**Entrada mínima:** Versão candidata, ambiente e fontes de dados.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: migração ensaiada, integridade, cópia de segurança, restauração e recuperação.
3. Executar as [verificações da fase 14](../../00-processo/checklist-mestre-desenvolvimento-software.md#fase-14), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** plano-migracao.md e procedimentos. Os espaços de registro já estão preparados nesta fase; preencher apenas com informações levantadas e validadas.

**Quem valida:** Responsável pelos dados valida integridade; desenvolvedor ensaia; responsável pela operação confere recuperação.

**Critério para avançar:** Ensaio demonstra integridade e recuperação; condições para implantação atendidas.

**O que impede avançar:** Migração sem reconciliação ou impossibilidade de recuperação após uma mudança crítica.

**Relação com outras etapas:** Alimenta homologação e implantação; repetir ensaios quando dados ou scripts mudarem.

## Uso recorrente

Quando a fase se repetir em outro incremento ou versão, identificar o ciclo no cartão e nos registros. Preservar resultados anteriores; criar um novo cartão de execução quando necessário. Esta estrutura representa o processo conhecido, não funcionalidades de produto inventadas.
