# F07.02 — Execução e consolidação

Fase 07 — Modelagem de dados.

[Voltar à fase](README.md) · [Cartão](https://github.com/vlabson/AgroGest/issues/35)

Situação: prevista, ainda não validada como concluída.

## Objetivo

obter e validar estruturas, restrições, histórico, origem e qualidade dos dados, migração.

## Dependência

Conferir a preparação da fase. Atividades transversais ou iterativas podem ocorrer em conjunto quando isso for registrado.

## Atividades específicas

- [ ] Identificar dados persistentes necessários
- [ ] Definir estruturas de persistência adequadas à tecnologia escolhida; tabelas quando o banco for relacional
- [ ] Definir campos e tipos de dados
- [ ] Definir identificadores; chaves primárias quando aplicáveis
- [ ] Definir relacionamentos e sua representação na persistência; chaves estrangeiras quando aplicáveis
- [ ] Definir obrigatoriedade e nulabilidade
- [ ] Definir restrições e unicidade
- [ ] Definir índices necessários inicialmente
- [ ] Definir estratégia para histórico/auditoria quando necessária
- [ ] Definir tratamento de exclusão lógica/física conforme o domínio
- [ ] Definir convenções de nomes
- [ ] Definir dados de referência e seeds quando necessários
- [ ] Produzir DER para modelo relacional ou representação equivalente adequada à persistência escolhida
- [ ] Validar o modelo contra os principais casos de uso
- [ ] Planejar migração/importação de dados legados, se houver

## Saída esperada

modelo-dados.md e migrations. Consolidar os resultados e referências em [registro-resultados.md](registro-resultados.md).

## Critério de conclusão

Atividades aplicáveis executadas e resultados registrados, com evidências e pendências identificadas. A aceitação final ocorre na validação da fase.
