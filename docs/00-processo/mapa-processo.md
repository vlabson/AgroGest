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

A estrutura das 21 fases está preparada em docs/fases/, com guias e registros específicos. Os modelos aguardam levantamento e validação; sua existência não representa trabalho concluído. Os nomes de entregáveis abaixo indicam o conteúdo a consolidar no registro da fase ou em arquivos específicos vinculados a ele.

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

## Guias detalhados por fase

O detalhamento está organizado em [pastas por fase](../fases/README.md), com atividades, registros e cartões vinculados.

- [Fase 00 — Iniciação e organização](../fases/00-iniciacao-e-organizacao/README.md)
- [Fase 01 — Descoberta e visão do projeto](../fases/01-descoberta-e-visao-do-projeto/README.md)
- [Fase 02 — Levantamento e análise dos processos](../fases/02-levantamento-e-analise-dos-processos/README.md)
- [Fase 03 — Requisitos e regras de negócio](../fases/03-requisitos-e-regras-de-negocio/README.md)
- [Fase 04 — Escopo, MVP e priorização](../fases/04-escopo-mvp-e-priorizacao/README.md)
- [Fase 05 — Modelagem do domínio](../fases/05-modelagem-do-dominio/README.md)
- [Fase 06 — Experiência do usuário e fluxos](../fases/06-experiencia-do-usuario-e-fluxos/README.md)
- [Fase 07 — Modelagem de dados](../fases/07-modelagem-de-dados/README.md)
- [Fase 08 — Arquitetura e decisões técnicas](../fases/08-arquitetura-e-decisoes-tecnicas/README.md)
- [Fase 09 — Segurança e privacidade](../fases/09-seguranca-e-privacidade/README.md)
- [Fase 10 — Planejamento do desenvolvimento](../fases/10-planejamento-do-desenvolvimento/README.md)
- [Fase 11 — Preparação do ambiente e repositório](../fases/11-preparacao-do-ambiente-e-repositorio/README.md)
- [Fase 12 — Ciclo de implementação](../fases/12-ciclo-de-implementacao/README.md)
- [Fase 13 — Qualidade e testes do sistema](../fases/13-qualidade-e-testes-do-sistema/README.md)
- [Fase 14 — Dados e preparação para produção](../fases/14-dados-e-preparacao-para-producao/README.md)
- [Fase 15 — Documentação para entrega](../fases/15-documentacao-para-entrega/README.md)
- [Fase 16 — Pré-release e homologação](../fases/16-pre-release-e-homologacao/README.md)
- [Fase 17 — Deploy e entrada em operação](../fases/17-deploy-e-entrada-em-operacao/README.md)
- [Fase 18 — Pós-deploy e validação real](../fases/18-pos-deploy-e-validacao-real/README.md)
- [Fase 19 — Operação, manutenção e evolução](../fases/19-operacao-manutencao-e-evolucao/README.md)
- [Fase 20 — Encerramento da versão ou projeto](../fases/20-encerramento-da-versao-ou-projeto/README.md)

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

Fase 00: condições iniciais conferidas e conclusão aprovada por Vlabson em 19/10/2026 para a beta local; evidências em [registro de resultados](../fases/00-iniciacao-e-organizacao/registro-resultados.md). Atualização dos cartões remotos pendente de autorização específica. Fase 01: em levantamento; visão em rascunho e decisões de negócio pendentes. Demais fases: previstas, ainda não executadas. Projetos do GitHub: quadro visual pendente de acesso; issues disponíveis. Não calcular porcentagem de conclusão pela quantidade de arquivos ou perguntas respondidas.

## Organização publicada em 2026-10-19

Por solicitação do responsável, todas as fases e suas atividades foram estruturadas previamente em Markdown e issues. A revisão organiza o processo completo sem preencher resultados de negócio ainda desconhecidos. O GitHub Projects continua opcional e pendente de acesso; a hierarquia de issues e os índices permitem navegar pelo processo.
