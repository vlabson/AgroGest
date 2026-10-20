# F14.02 — Execução e consolidação

Fase 14 — Dados e preparação para produção.

[Voltar à fase](README.md) · [Cartão](https://github.com/vlabson/AgroGest/issues/63)

Situação: prevista, ainda não validada como concluída.

## Objetivo

obter e validar migração ensaiada, integridade, cópia de segurança, restauração e recuperação.

## Dependência

Conferir a preparação da fase. Atividades transversais ou iterativas podem ocorrer em conjunto quando isso for registrado.

## Atividades específicas

- [ ] Definir dados que serão levados para produção
- [ ] Limpar e validar dados legados antes da importação
- [ ] Mapear campos entre fonte antiga e novo sistema
- [ ] Definir scripts/processo de migração
- [ ] Testar migração em ambiente seguro
- [ ] Validar quantidade e integridade dos registros migrados
- [ ] Definir estratégia de rollback da migração
- [ ] Preparar migrations de produção
- [ ] Revisar configurações de produção
- [ ] Revisar secrets de produção
- [ ] Revisar permissões de banco e infraestrutura
- [ ] Confirmar política de backup
- [ ] Executar/testar restauração quando aplicável
- [ ] Preparar checklist de implantação
- [ ] Definir reconciliação e tratamento de registros rejeitados na migração; testar compatibilidade entre versões de aplicação e dados
- [ ] Definir limites de perda de dados e tempo de recuperação conforme a necessidade, sem presumir que backup garante restauração

## Saída esperada

plano-migracao.md e procedimentos. Consolidar os resultados e referências em [registro-resultados.md](registro-resultados.md).

## Critério de conclusão

Atividades aplicáveis executadas e resultados registrados, com evidências e pendências identificadas. A aceitação final ocorre na validação da fase.
