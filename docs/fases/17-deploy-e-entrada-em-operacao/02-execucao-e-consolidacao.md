# F17.02 — Execução e consolidação

Fase 17 — Deploy e entrada em operação.

[Voltar à fase](README.md) · [Cartão](https://github.com/vlabson/AgroGest/issues/75)

Situação: prevista, ainda não validada como concluída.

## Objetivo

obter e validar publicação controlada, migração, testes de fumaça, comunicação e reversão.

## Dependência

Conferir a preparação da fase. Atividades transversais ou iterativas podem ocorrer em conjunto quando isso for registrado.

## Atividades específicas

- [ ] Confirmar janela/condições de implantação
- [ ] Confirmar backup imediatamente antes de mudanças críticas quando aplicável
- [ ] Aplicar infraestrutura/configuração necessária
- [ ] Aplicar migrations
- [ ] Executar migração/importação de dados
- [ ] Publicar backend
- [ ] Publicar frontend
- [ ] Configurar domínio/DNS/HTTPS quando aplicável
- [ ] Configurar serviços externos
- [ ] Executar smoke tests em produção
- [ ] Validar autenticação e permissões
- [ ] Validar fluxos críticos em produção
- [ ] Validar logs/monitoramento
- [ ] Confirmar que não houve perda/corrupção de dados
- [ ] Executar rollback se critérios mínimos não forem atendidos
- [ ] Registrar versão implantada
- [ ] Comunicar a mudança às pessoas afetadas e confirmar responsáveis pela observação inicial e por incidentes

## Saída esperada

registro-release.md e logs operacionais. Consolidar os resultados e referências em [registro-resultados.md](registro-resultados.md).

## Critério de conclusão

Atividades aplicáveis executadas e resultados registrados, com evidências e pendências identificadas. A aceitação final ocorre na validação da fase.
