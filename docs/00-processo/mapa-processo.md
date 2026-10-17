# Mapa do processo de desenvolvimento

Revisão 0.3 — 2026-10-16. Adaptação para o AgroGest e projetos pessoais de aprendizagem. Este mapa é o guia para saber o que definir, quando aprofundar e como avaliar a conclusão. Não representa certificação nem garante ausência de descobertas futuras.

## Aprovação e situação da aplicação

- Objeto aprovado: mapa do processo, revisão 0.3, e sua adoção como orientação do AgroGest.
- Responsável pela aprovação: Vlabson, responsável pelo projeto.
- Data: 2026-10-16.
- Evidência: aprovação expressa na conversa — “ok aprovo o mapa vamos seguir”.
- Encaminhamento confirmado: estruturar e salvar as definições antes de iniciar o levantamento de negócio.
- Limite: esta aprovação não aprova a visão do produto, requisitos, MVP, decisões ainda pendentes ou implantação.
- Situação: preparação documental; a entrevista de discovery ainda não foi iniciada. Os registros existentes representam o contexto já conhecido.

## Base e aplicação

O [SWEBOK, da IEEE Computer Society](https://www.computer.org/education/bodies-of-knowledge/software-engineering) organiza conhecimentos de requisitos, projeto, construção, testes, manutenção e gestão. Usamos essas áreas como referência de cobertura, sem reproduzir um ciclo obrigatório.

O [SEBoK sobre necessidades](https://sebokwiki.org/wiki/Stakeholder_Needs_Definition) ajuda a distinguir expectativas dos participantes de requisitos técnicos. A [definição de requisitos](https://sebokwiki.org/wiki/System_Requirements) orienta a ligação entre necessidades, funções, interfaces e critérios verificáveis. A [gestão de requisitos](https://sebokwiki.org/wiki/Requirements_Management) fundamenta os vínculos e a revisão de mudanças. A [retirada de operação](https://sebokwiki.org/wiki/Disposal_and_Retirement) lembra que o ciclo não termina na implantação. A numeração, os cartões, os modelos e os portões abaixo são escolhas de adaptação deste projeto.

As fases se repetem por incremento. Esclarecer apenas o necessário à próxima decisão, antecipando riscos críticos. Protótipos e investigação podem revelar mudanças na visão. Segurança, testes, riscos, documentação e aprendizagem acompanham todo o ciclo; suas fases específicas consolidam verificações, não marcam o primeiro momento para pensar nelas.

## Onde estão as definições do sistema

Na Fase 01, definir o que é o produto, para quem existe, capacidades propostas, fronteiras, interações, ambiente de uso e resultados. Na Fase 02, compreender a operação atual e a mudança desejada. Na Fase 03, especificar funções, regras, dados, interfaces, qualidades e aceitação. Na Fase 04, selecionar o MVP. Modelos de domínio, UX, dados e arquitetura detalham a solução sem substituir essas decisões.

Capacidade geral é algo que o produto deverá permitir fazer; requisito define um comportamento verificável; arquitetura define como implementá-lo. Uma capacidade proposta na visão não é automaticamente uma funcionalidade aprovada para o MVP.

## Entradas, registros e critérios de saída

Os nomes de registros futuros são sugestões de destino. Criá-los quando necessários e registrar o caminho real na issue. Não criar 21 pastas ou documentos vazios para simular progresso. Um documento pode conter várias seções desde que sua responsabilidade seja clara.

| Fase | Entrada mínima | Registro de saída | Critério de saída |
|---|---|---|---|
| 00 — Iniciação e organização | Intenção e responsável conhecidos | contexto-inicial-projeto.md e README | Responsável confirma condições iniciais; acesso e organização permitem registrar o trabalho |
| 01 — Descoberta e visão do projeto | Contexto inicial e pessoas a consultar | registro-discovery.md e visao-projeto.md | Visão revisada e aprovada; nenhuma dúvida impede compreender problema, produto, objetivo e limites |
| 02 — Levantamento e análise dos processos | Atividade e contexto de investigação delimitados | processos-negocio.md | Responsável pela atividade valida cenários principais e exceções relevantes; mudança operacional compreendida |
| 03 — Requisitos e regras de negócio | Necessidades e processos suficientemente compreendidos | requisitos-sistema.md | Requisitos do próximo incremento são claros, consistentes, viáveis e verificáveis; lacunas bloqueadoras resolvidas |
| 04 — Escopo, MVP e priorização | Requisitos candidatos e riscos conhecidos | escopo-mvp.md e issues | Responsável aprova um incremento útil e viável com critérios de conclusão e limites explícitos |
| 05 — Modelagem do domínio | Casos de uso e regras do incremento | modelo-dominio.md | Exemplos reais percorrem o modelo sem contradições nas regras críticas |
| 06 — Experiência do usuário e fluxos | Usuários, tarefas e capacidades priorizadas | fluxos-usuario.md e protótipos | Usuário consegue compreender o fluxo principal e a recuperação de erros; observações tratadas |
| 07 — Modelagem de dados | Domínio e necessidades de persistência; interação com arquitetura | modelo-dados.md e migrations | Persistência sustenta regras e consultas críticas; riscos de perda e inconsistência tratados |
| 08 — Arquitetura e decisões técnicas | Requisitos significativos, restrições e riscos | arquitetura.md e decisões técnicas | Solução proporcional; riscos técnicos principais avaliados; contratos e responsabilidades compreendidos |
| 09 — Segurança e privacidade | Dados, usuários, fronteiras e ambiente conhecidos | seguranca-privacidade.md | Riscos críticos mitigados ou impeditivos; exceções explicitamente avaliadas pelo responsável |
| 10 — Planejamento do desenvolvimento | Escopo priorizado e riscos de execução | plano-desenvolvimento.md e issues | Próximo incremento executável com critérios de aceite, responsável e capacidade disponível |
| 11 — Preparação do ambiente e repositório | Decisões técnicas mínimas e ações autorizadas | README, configuração e evidências | Instalação e execução verificadas; testes e build aplicáveis funcionam; nenhum segredo versionado |
| 12 — Ciclo de implementação | Issue pronta e alteração autorizada | issue, alterações e evidências | Critérios de aceite e DoD atendidos; autorização de integração respeitada |
| 13 — Qualidade e testes do sistema | Estratégia definida antes da execução e incremento testável | plano-testes.md e resultados | Requisitos críticos cobertos; defeitos impeditivos resolvidos; limitações aceitas registradas |
| 14 — Dados e preparação para produção | Versão candidata, ambiente e fontes de dados | plano-migracao.md e procedimentos | Ensaio demonstra integridade e recuperação; condições para implantação atendidas |
| 15 — Documentação para entrega | Comportamento e operação reais da versão | README, guia-usuario.md e operacao.md | Documentação permite executar, usar e recuperar a versão; instruções conferidas |
| 16 — Pré-release e homologação | Versão identificada e evidências técnicas | registro-release.md | Responsável aprova implantação com critérios de aceite atendidos e pendências aceitáveis |
| 17 — Deploy e entrada em operação | Autorização específica e plano de implantação | registro-release.md e logs operacionais | Fluxos críticos e integridade conferidos; versão disponível ou reversão executada e registrada |
| 18 — Pós-deploy e validação real | Versão em uso e referência inicial de resultados | avaliacao-release.md e issues | Resultado confrontado com objetivo; ações e responsáveis registrados |
| 19 — Operação, manutenção e evolução | Produto ativo e responsável pela operação | operacao.md e issues | Ciclo operacional revisado na periodicidade definida; melhorias voltam à análise de necessidade |
| 20 — Encerramento da versão ou projeto | Entregas e pendências avaliadas | encerramento.md ou registro-release.md | Resultado e responsabilidades aceitos; continuidade ou encerramento seguro definido; nenhuma pendência sem destino |

## Guia detalhado por fase

Cada fase segue a estrutura abaixo. “Concluído” exige evidência e validação, não apenas um arquivo criado. Registrar uma dúvida não bloqueadora com responsável e condição de retomada; se ela puder invalidar a próxima decisão, resolver antes de avançar. Aplicar os passos ao incremento em avaliação.

### Fase 00 — Iniciação e organização

**Objetivo:** obter e validar nome, propósito, responsáveis, repositório, organização, disponibilidade e limites iniciais.

**Entrada mínima:** Intenção e responsável conhecidos.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: nome, propósito, responsáveis, repositório, organização, disponibilidade e limites iniciais.
3. Executar as [verificações da fase 00](checklist-mestre-desenvolvimento-software.md#fase-00), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** contexto-inicial-projeto.md e README. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pelo projeto valida a organização e os limites iniciais.

**Critério para avançar:** Responsável confirma condições iniciais; acesso e organização permitem registrar o trabalho.

**O que impede avançar:** Falta de responsável ou de autorização para criar e acessar os recursos necessários.

**Relação com outras etapas:** Prepara a Fase 01. Condições podem ser revistas ao longo do projeto.

### Fase 01 — Descoberta e visão do projeto

**Objetivo:** obter e validar problema ou oportunidade, evidências, produto proposto, capacidades, fronteiras, interações, uso, objetivos e viabilidade inicial.

**Entrada mínima:** Contexto inicial e pessoas a consultar.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: problema ou oportunidade, evidências, produto proposto, capacidades, fronteiras, interações, uso, objetivos e viabilidade inicial.
3. Executar as [verificações da fase 01](checklist-mestre-desenvolvimento-software.md#fase-01), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** registro-discovery.md e visao-projeto.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pelo produto aprova; usuários e conhecedores da atividade validam os relatos; analista organiza a proposta.

**Critério para avançar:** Visão revisada e aprovada; nenhuma dúvida impede compreender problema, produto, objetivo e limites.

**O que impede avançar:** Não compreender necessidade, produto, objetivo ou limites; proposta sem viabilidade inicial suficiente.

**Relação com outras etapas:** Orienta processos, requisitos e escopo. Revisitar a visão se esses trabalhos revelarem mudança relevante.

### Fase 02 — Levantamento e análise dos processos

**Objetivo:** obter e validar fluxo atual e desejado, responsáveis, entradas, saídas, exceções, controles e impacto da mudança.

**Entrada mínima:** Atividade e contexto de investigação delimitados.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: fluxo atual e desejado, responsáveis, entradas, saídas, exceções, controles e impacto da mudança.
3. Executar as [verificações da fase 02](checklist-mestre-desenvolvimento-software.md#fase-02), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** processos-negocio.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Quem executa a atividade valida o fluxo; responsável pelo produto confirma a mudança desejada.

**Critério para avançar:** Responsável pela atividade valida cenários principais e exceções relevantes; mudança operacional compreendida.

**O que impede avançar:** Fluxo crítico contraditório ou desconhecimento de quem executa e valida uma etapa essencial.

**Relação com outras etapas:** Alimenta requisitos e domínio; pode exigir ajustar a visão.

### Fase 03 — Requisitos e regras de negócio

**Objetivo:** obter e validar funções, regras, dados, interfaces, qualidades mensuráveis, condições de operação, aceitação e rastreabilidade.

**Entrada mínima:** Necessidades e processos suficientemente compreendidos.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: funções, regras, dados, interfaces, qualidades mensuráveis, condições de operação, aceitação e rastreabilidade.
3. Executar as [verificações da fase 03](checklist-mestre-desenvolvimento-software.md#fase-03), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** requisitos-sistema.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Analista ou desenvolvedor verifica consistência e viabilidade; usuário valida comportamento; responsável pelo produto aprova o recorte.

**Critério para avançar:** Requisitos do próximo incremento são claros, consistentes, viáveis e verificáveis; lacunas bloqueadoras resolvidas.

**O que impede avançar:** Requisito crítico ambíguo, conflitante, sem origem ou impossível de verificar.

**Relação com outras etapas:** Alimenta MVP, modelos, arquitetura e testes; recebe retorno de protótipos e implementação.

### Fase 04 — Escopo, MVP e priorização

**Objetivo:** obter e validar recorte de entrega, exclusões, prioridades, dependências, esforço, custo e aprendizagem.

**Entrada mínima:** Requisitos candidatos e riscos conhecidos.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: recorte de entrega, exclusões, prioridades, dependências, esforço, custo e aprendizagem.
3. Executar as [verificações da fase 04](checklist-mestre-desenvolvimento-software.md#fase-04), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** escopo-mvp.md e issues. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pelo produto decide prioridade e abrangência, com estimativas do desenvolvedor.

**Critério para avançar:** Responsável aprova um incremento útil e viável com critérios de conclusão e limites explícitos.

**O que impede avançar:** Incremento sem utilidade demonstrável, sem critério de aceite ou incompatível com os recursos disponíveis.

**Relação com outras etapas:** Seleciona o recorte das fases 05 a 13. Reavaliar quando custo, necessidade ou risco mudar.

### Fase 05 — Modelagem do domínio

**Objetivo:** obter e validar glossário, conceitos, relações, estados e invariantes.

**Entrada mínima:** Casos de uso e regras do incremento.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: glossário, conceitos, relações, estados e invariantes.
3. Executar as [verificações da fase 05](checklist-mestre-desenvolvimento-software.md#fase-05), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** modelo-dominio.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor modela; conhecedor do negócio verifica conceitos, exemplos e regras.

**Critério para avançar:** Exemplos reais percorrem o modelo sem contradições nas regras críticas.

**O que impede avançar:** Contradição nas regras críticas ou nos significados dos conceitos usados pelo incremento.

**Relação com outras etapas:** Interage com requisitos, UX, dados e implementação.

### Fase 06 — Experiência do usuário e fluxos

**Objetivo:** obter e validar jornadas, navegação, estados de erro, acessibilidade e protótipos necessários.

**Entrada mínima:** Usuários, tarefas e capacidades priorizadas.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: jornadas, navegação, estados de erro, acessibilidade e protótipos necessários.
3. Executar as [verificações da fase 06](checklist-mestre-desenvolvimento-software.md#fase-06), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** fluxos-usuario.md e protótipos. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Usuário valida as tarefas; desenvolvedor ou responsável por UX analisa acessibilidade e estados da interface.

**Critério para avançar:** Usuário consegue compreender o fluxo principal e a recuperação de erros; observações tratadas.

**O que impede avançar:** Usuário não consegue executar a tarefa principal ou se recuperar de erro relevante.

**Relação com outras etapas:** Interage com requisitos e domínio; mudanças aprovadas alimentam implementação e testes.

### Fase 07 — Modelagem de dados

**Objetivo:** obter e validar estruturas, restrições, histórico, origem e qualidade dos dados, migração.

**Entrada mínima:** Domínio e necessidades de persistência; interação com arquitetura.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: estruturas, restrições, histórico, origem e qualidade dos dados, migração.
3. Executar as [verificações da fase 07](checklist-mestre-desenvolvimento-software.md#fase-07), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** modelo-dados.md e migrations. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor valida restrições e persistência; responsável pelos dados confirma histórico e origem.

**Critério para avançar:** Persistência sustenta regras e consultas críticas; riscos de perda e inconsistência tratados.

**O que impede avançar:** Persistência não sustenta uma regra essencial ou há risco de perda de histórico sem tratamento.

**Relação com outras etapas:** Definir junto à arquitetura; orientar migrations e preparação dos dados.

### Fase 08 — Arquitetura e decisões técnicas

**Objetivo:** obter e validar componentes, contratos, implantação, dependências, alternativas e decisões justificadas.

**Entrada mínima:** Requisitos significativos, restrições e riscos.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: componentes, contratos, implantação, dependências, alternativas e decisões justificadas.
3. Executar as [verificações da fase 08](checklist-mestre-desenvolvimento-software.md#fase-08), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** arquitetura.md e decisões técnicas. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor justifica decisões; responsável pelo projeto aceita custos e riscos relevantes.

**Critério para avançar:** Solução proporcional; riscos técnicos principais avaliados; contratos e responsabilidades compreendidos.

**O que impede avançar:** Decisão técnica crítica sem validação de viabilidade ou dependência indispensável indisponível.

**Relação com outras etapas:** Interage com dados, segurança e ambientes; fundamenta implementação e operação.

### Fase 09 — Segurança e privacidade

**Objetivo:** obter e validar ameaças, acesso, proteção de dados, segredos, dependências e resposta a incidentes.

**Entrada mínima:** Dados, usuários, fronteiras e ambiente conhecidos.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: ameaças, acesso, proteção de dados, segredos, dependências e resposta a incidentes.
3. Executar as [verificações da fase 09](checklist-mestre-desenvolvimento-software.md#fase-09), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** seguranca-privacidade.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor avalia controles; responsável pelo projeto decide riscos e consulta especialista quando necessário.

**Critério para avançar:** Riscos críticos mitigados ou impeditivos; exceções explicitamente avaliadas pelo responsável.

**O que impede avançar:** Risco crítico de acesso indevido, perda ou exposição de dados sem tratamento aceitável.

**Relação com outras etapas:** Atividade transversal desde a descoberta; controles são implementados e verificados em cada entrega.

### Fase 10 — Planejamento do desenvolvimento

**Objetivo:** obter e validar issues pequenas, dependências, estimativas, disponibilidade, marcos, revisões e Definition of Done.

**Entrada mínima:** Escopo priorizado e riscos de execução.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: issues pequenas, dependências, estimativas, disponibilidade, marcos, revisões e Definition of Done.
3. Executar as [verificações da fase 10](checklist-mestre-desenvolvimento-software.md#fase-10), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** plano-desenvolvimento.md e issues. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pelo projeto confronta planejamento com disponibilidade; desenvolvedor detalha o trabalho.

**Critério para avançar:** Próximo incremento executável com critérios de aceite, responsável e capacidade disponível.

**O que impede avançar:** Trabalho sem critério de aceite, sem capacidade de execução ou com dependência impeditiva.

**Relação com outras etapas:** Organiza o próximo incremento; replanejar a partir de evidência e capacidade real.

### Fase 11 — Preparação do ambiente e repositório

**Objetivo:** obter e validar execução reproduzível, configuração, testes, automação proporcional e separação de ambientes.

**Entrada mínima:** Decisões técnicas mínimas e ações autorizadas.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: execução reproduzível, configuração, testes, automação proporcional e separação de ambientes.
3. Executar as [verificações da fase 11](checklist-mestre-desenvolvimento-software.md#fase-11), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** README, configuração e evidências. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor prepara e verifica o ambiente; responsável pelo projeto autoriza ações com efeitos.

**Critério para avançar:** Instalação e execução verificadas; testes e build aplicáveis funcionam; nenhum segredo versionado.

**O que impede avançar:** Ambiente não reproduzível, segredo exposto ou verificações essenciais sem funcionamento.

**Relação com outras etapas:** Habilita implementação e validação; manter instruções conforme o ambiente evolui.

### Fase 12 — Ciclo de implementação

**Objetivo:** obter e validar implementação, revisão, testes, documentação e aprendizagem por funcionalidade.

**Entrada mínima:** Issue pronta e alteração autorizada.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: implementação, revisão, testes, documentação e aprendizagem por funcionalidade.
3. Executar as [verificações da fase 12](checklist-mestre-desenvolvimento-software.md#fase-12), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** issue, alterações e evidências. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor implementa e verifica; revisor avalia quando disponível; responsável pelo produto valida o resultado.

**Critério para avançar:** Critérios de aceite e DoD atendidos; autorização de integração respeitada.

**O que impede avançar:** Critério de aceite não atendido, regressão crítica, autorização ausente ou dúvida que muda o comportamento esperado.

**Relação com outras etapas:** Repetir por funcionalidade; retornar a requisitos e decisão técnica quando houver dúvida relevante.

### Fase 13 — Qualidade e testes do sistema

**Objetivo:** obter e validar testes por risco, verificação de requisitos, defeitos e evidências reproduzíveis.

**Entrada mínima:** Estratégia definida antes da execução e incremento testável.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: testes por risco, verificação de requisitos, defeitos e evidências reproduzíveis.
3. Executar as [verificações da fase 13](checklist-mestre-desenvolvimento-software.md#fase-13), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** plano-testes.md e resultados. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor ou testador executa verificações; responsável pelo produto avalia limitações e impacto dos defeitos.

**Critério para avançar:** Requisitos críticos cobertos; defeitos impeditivos resolvidos; limitações aceitas registradas.

**O que impede avançar:** Defeito impeditivo ou ausência de evidência para um requisito crítico.

**Relação com outras etapas:** Planejar junto aos requisitos; executar por incremento e antes da release.

### Fase 14 — Dados e preparação para produção

**Objetivo:** obter e validar migração ensaiada, integridade, cópia de segurança, restauração e recuperação.

**Entrada mínima:** Versão candidata, ambiente e fontes de dados.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: migração ensaiada, integridade, cópia de segurança, restauração e recuperação.
3. Executar as [verificações da fase 14](checklist-mestre-desenvolvimento-software.md#fase-14), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** plano-migracao.md e procedimentos. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pelos dados valida integridade; desenvolvedor ensaia; responsável pela operação confere recuperação.

**Critério para avançar:** Ensaio demonstra integridade e recuperação; condições para implantação atendidas.

**O que impede avançar:** Migração sem reconciliação ou impossibilidade de recuperação após uma mudança crítica.

**Relação com outras etapas:** Alimenta homologação e implantação; repetir ensaios quando dados ou scripts mudarem.

### Fase 15 — Documentação para entrega

**Objetivo:** obter e validar instruções técnicas e de uso, suporte, limites e procedimentos de recuperação.

**Entrada mínima:** Comportamento e operação reais da versão.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: instruções técnicas e de uso, suporte, limites e procedimentos de recuperação.
3. Executar as [verificações da fase 15](checklist-mestre-desenvolvimento-software.md#fase-15), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** README, guia-usuario.md e operacao.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Desenvolvedor documenta; usuário e operador conferem as instruções que utilizarão.

**Critério para avançar:** Documentação permite executar, usar e recuperar a versão; instruções conferidas.

**O que impede avançar:** Instrução essencial de execução ou recuperação não corresponde à versão real.

**Relação com outras etapas:** Acompanha implementação; consolidar antes da homologação e manter durante operação.

### Fase 16 — Pré-release e homologação

**Objetivo:** obter e validar aceitação pelo usuário, riscos, decisão de implantação e critérios de reversão.

**Entrada mínima:** Versão identificada e evidências técnicas.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: aceitação pelo usuário, riscos, decisão de implantação e critérios de reversão.
3. Executar as [verificações da fase 16](checklist-mestre-desenvolvimento-software.md#fase-16), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** registro-release.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Usuário homologa; responsável pelo produto aceita a versão; responsável pela implantação autoriza sua execução.

**Critério para avançar:** Responsável aprova implantação com critérios de aceite atendidos e pendências aceitáveis.

**O que impede avançar:** Aceite ou autorização ausente; risco impeditivo, teste crítico falho ou recuperação inviável.

**Relação com outras etapas:** Autoriza a decisão de implantação; falhas retornam ao trabalho necessário, não a uma aprovação automática.

### Fase 17 — Deploy e entrada em operação

**Objetivo:** obter e validar publicação controlada, migração, testes de fumaça, comunicação e reversão.

**Entrada mínima:** Autorização específica e plano de implantação.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: publicação controlada, migração, testes de fumaça, comunicação e reversão.
3. Executar as [verificações da fase 17](checklist-mestre-desenvolvimento-software.md#fase-17), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** registro-release.md e logs operacionais. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pela implantação executa; responsável pela operação acompanha e decide recuperação conforme o plano.

**Critério para avançar:** Fluxos críticos e integridade conferidos; versão disponível ou reversão executada e registrada.

**O que impede avançar:** Falha em um critério de entrada em operação, integridade comprometida ou autorização ausente.

**Relação com outras etapas:** Entrega à operação; falha relevante aciona recuperação e registro de incidente.

### Fase 18 — Pós-deploy e validação real

**Objetivo:** obter e validar adoção, resultados, feedback, defeitos e retrospectiva.

**Entrada mínima:** Versão em uso e referência inicial de resultados.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: adoção, resultados, feedback, defeitos e retrospectiva.
3. Executar as [verificações da fase 18](checklist-mestre-desenvolvimento-software.md#fase-18), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** avaliacao-release.md e issues. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Usuário relata uso; responsável pelo produto avalia resultados e prioriza ajustes.

**Critério para avançar:** Resultado confrontado com objetivo; ações e responsáveis registrados.

**O que impede avançar:** Não há evidência suficiente para afirmar o resultado; manter a avaliação aberta e investigar.

**Relação com outras etapas:** Informa manutenção e próxima descoberta; objetivos não atendidos geram investigação.

### Fase 19 — Operação, manutenção e evolução

**Objetivo:** obter e validar disponibilidade, incidentes, restauração, custos, atualizações, suporte e melhorias.

**Entrada mínima:** Produto ativo e responsável pela operação.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: disponibilidade, incidentes, restauração, custos, atualizações, suporte e melhorias.
3. Executar as [verificações da fase 19](checklist-mestre-desenvolvimento-software.md#fase-19), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** operacao.md e issues. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pela operação acompanha serviços; desenvolvedor mantém; responsável pelo produto prioriza evolução.

**Critério para avançar:** Ciclo operacional revisado na periodicidade definida; melhorias voltam à análise de necessidade.

**O que impede avançar:** Incidente crítico, backup sem recuperação viável ou falta de responsável pela continuidade.

**Relação com outras etapas:** Recorrente enquanto o produto estiver ativo; novas funcionalidades retornam ao ciclo de descoberta.

### Fase 20 — Encerramento da versão ou projeto

**Objetivo:** obter e validar aceite, transferência de responsabilidade e, se houver desativação, exportação, retenção e revogação de acessos.

**Entrada mínima:** Entregas e pendências avaliadas.

**Como conduzir:**

1. Conferir os registros existentes e delimitar o incremento ou ciclo de trabalho.
2. Desenvolver o conteúdo específico desta fase: aceite, transferência de responsabilidade e, se houver desativação, exportação, retenção e revogação de acessos.
3. Executar as [verificações da fase 20](checklist-mestre-desenvolvimento-software.md#fase-20), registrando evidência, pendência ou não aplicabilidade justificada.
4. Submeter o resultado à validação indicada e registrar a decisão, revisão e ressalvas.

**Saída e local de registro:** encerramento.md ou registro-release.md. Para registros futuros, escolher o caminho na issue ao iniciar a fase; não criar arquivo vazio antecipadamente.

**Quem valida:** Responsável pelo projeto aceita encerramento; responsável pelos dados e operador confirmam continuidade ou retirada segura.

**Critério para avançar:** Resultado e responsabilidades aceitos; continuidade ou encerramento seguro definido; nenhuma pendência sem destino.

**O que impede avançar:** Dados, acessos, suporte ou pendências sem destino; encerramento não aceito pelo responsável.

**Relação com outras etapas:** Fechar uma versão não desativa o produto. Se ele continuar, manter Fase 19 e backlog; se retirar, cumprir o plano de transição.

## Responsabilidades e decisões

- Responsável pelo produto: decide prioridade, escopo e aceite. No AgroGest, o responsável pelo projeto exerce esse papel; outras delegações precisam ser registradas.
- Usuário ou conhecedor da atividade: valida se o relato, o fluxo e a solução representam a operação real. Não presumir que todas as pessoas terão o mesmo papel.
- Desenvolvedor: propõe alternativas, analisa impactos, implementa e verifica; explica decisões no contexto de aprendizagem.
- Revisor e responsável pela operação: funções a definir por entrega. Uma mesma pessoa pode acumular funções; registrar isso e evitar apresentar autorrevisão como avaliação independente.
- O assistente apoia análise, documentação e execução autorizada. Não substitui a decisão do usuário nem preenche informações de negócio sem fonte.

Validar o entendimento, aprovar requisitos, aceitar uma versão e autorizar publicação são decisões diferentes. Registrar objeto, revisão, responsável, data e ressalvas. Nenhum portão autoriza sozinho commit, push, alteração de dados ou implantação.

## Rastreabilidade e mudança

Manter o vínculo necessidade → capacidade → requisito → issue → implementação → teste → validação em uso. IDs e links bastam; não copiar conteúdo entre ferramentas. Usar os [modelos de registros](modelos-registros.md) quando a informação surgir.

Quando algo mudar, registrar o motivo e analisar impacto em escopo, dados, interfaces, testes, custo e prazo. O responsável decide aprovar, rejeitar ou adiar. Atualizar os registros dependentes e conservar o histórico. Não manter uma decisão antiga como se ainda fosse vigente.

## Como verificar a cobertura

Para cada incremento, revisar negócio e usuários; produto e fronteiras; processos e regras; dados e interfaces; qualidades; segurança e privacidade; UX e acessibilidade; viabilidade e planejamento; verificação e validação; implantação e recuperação; suporte e encerramento. Cada dimensão recebe uma resposta sustentada, uma justificativa de não aplicabilidade ou uma pendência com responsável e momento de resolução.

Uma dúvida é bloqueadora quando impede decidir o próximo trabalho com risco aceitável: por exemplo, não saber qual problema se quer resolver antes de aprovar a visão, ou não saber recuperar os dados antes de uma migração crítica. Registrar essa avaliação, não exigir que todas as dúvidas futuras sejam resolvidas agora.

## Registros e visibilidade

Checklist e roteiro em Markdown são as fontes vigentes desta revisão. Os arquivos Word existentes no projeto permanecem como versões anteriores e não estão sincronizados com esta revisão. Gerar uma nova cópia Word somente quando necessária e após revisão visual; não editar formatos paralelos como fontes independentes.

Cartões: estado do trabalho e links. Registro da discovery: evidências e relatos. Visão: síntese do produto e da necessidade. Contexto inicial: origem das premissas; quando revisadas, referenciar a decisão atual. Aprovação do método não significa aprovação da visão nem conclusão do checklist.

Repositório público: publicar apenas informações apropriadas. Não adicionar credenciais, planilhas reais ou dados privados. Evidências podem ser referenciadas por descrição e responsável sem expor o conteúdo.

## Situação atual

Fase 0: infraestrutura e documentação inicial existentes; checklist não foi retroativamente marcado como concluído. Fase 01: em levantamento; visão em rascunho e decisões de negócio pendentes. Demais fases: previstas, ainda não executadas. Projetos do GitHub: quadro visual pendente de acesso; issues disponíveis. Não calcular porcentagem de conclusão pela quantidade de arquivos ou perguntas respondidas.
