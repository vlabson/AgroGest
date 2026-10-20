# CHECKLIST MESTRE DE DESENVOLVIMENTO DE SOFTWARE

Do zero à entrega, operação e evolução do produto

Versão 0.3 • Checklist evolutivo • Projeto inicial: AgroGest

Finalidade: orientar e acompanhar o desenvolvimento do projeto, com verificações proporcionais ao escopo e aos riscos. O checklist deve evoluir conforme a experiência prática e os aprendizados do projeto.

Como aplicar: as fases são uma referência iterativa. Detalhar apenas o necessário para o próximo incremento e revisar decisões conforme novas evidências surgirem. Testes, segurança, documentação e validação acompanham o trabalho desde o início.

Situação dos itens: manter ☐ para pendente; usar [C] para concluído, [NA] para não aplicável e [A] para adiado. Registrar justificativa para [NA] e, para [A], motivo, impacto e condição ou entrega de retomada. Um item adiado continua pendente e não satisfaz um portão que dependa dele.

Recorrência: reaplicar a fase 12 por funcionalidade; as fases 13 a 18 e o encerramento da fase 20 por versão, conforme aplicabilidade; e a fase 19 na periodicidade definida para cada atividade. Revisitar as demais fases quando houver mudanças relevantes. Identificar o ciclo e registrar data e evidências por referência, preservando o histórico.

Acompanhamento: usar os portões de qualidade como resumo e consultar o checklist detalhado conforme a atividade. Manter cada informação em uma fonte principal e referenciá-la em issues e documentos, evitando cópias divergentes.

Autorizações: este checklist não autoriza a execução de ações por si só. Seguir o acordo de trabalho vigente e obter autorização explícita para alterações, comandos com efeitos e operações de Git/GitHub, banco de dados e implantação quando exigida. Concluir um item não autoriza automaticamente o próximo.

Referência operacional: mapa-processo.md define entradas, saídas, responsáveis e critérios das 21 fases. Este checklist Markdown é a fonte vigente. O DOCX existente no projeto é uma versão anterior, ainda não sincronizada. Preparar o processo não significa concluir suas atividades. A adaptação usa referências de engenharia de software, sem alegação de certificação.

<a id="fase-00"></a>

## FASE 0 — INICIAÇÃO E ORGANIZAÇÃO

- [C] Registrar nome provisório do projeto

- [C] Registrar ideia/origem da necessidade

- [C] Identificar responsável pelo produto/projeto

- [C] Definir onde o projeto será versionado

- [C] Criar repositório Git

- [C] Definir estrutura inicial para documentação

- [C] Adicionar este checklist ao repositório

- [C] Definir convenção inicial de nomes e organização dos documentos

- [C] Registrar premissas, restrições e dúvidas conhecidas

- [C] Definir quem decide escopo, valida uso, desenvolve e responde pela operação; registrar disponibilidade de tempo e orçamento conhecidos

- [C] Definir como registrar riscos, decisões, alterações e aprovações e como separar dados públicos de dados privados

Artefato/saída: Repositório inicial + checklist mestre versionado.

Critério de saída: Responsável confirma condições iniciais; acesso e organização permitem registrar o trabalho. Verificar apenas o recorte do incremento ou ciclo em avaliação.

Aprovação: Vlabson, 19/10/2026, ciclo da beta local. Evidências e pendências encaminhadas no [registro da Fase 00](../fases/00-iniciacao-e-organizacao/registro-resultados.md).

<a id="fase-01"></a>

## FASE 1 — DESCOBERTA E VISÃO DO PROJETO

- [ ] P01-01 — Descrever o negócio, a atividade e o contexto de uso com fonte das informações

- [ ] P01-02 — Registrar problema ou oportunidade, exemplos, frequência conhecida, consequências e tratamento atual; separar fatos relatados de hipóteses

- [ ] P01-03 — Identificar usuários, pessoas afetadas, decisor, responsável pela validação e futura operação; permitir que uma pessoa acumule papéis

- [ ] P01-04 — Selecionar o problema ou oportunidade prioritário e justificar sua importância

- [ ] P01-05 — Definir a melhoria desejada e como avaliar o resultado, incluindo referência atual, sinal de sucesso, momento e responsável

- [ ] P01-06 — Descrever o produto proposto e suas capacidades gerais, ligando cada capacidade a uma necessidade; distinguir propostas de decisões aprovadas

- [ ] P01-07 — Definir fronteiras do sistema, responsabilidades humanas, interações externas, informações trocadas e relação com controles atuais

- [ ] P01-08 — Registrar condições de uso e necessidades iniciais de qualidade: dispositivos, conectividade, acesso, dados críticos, continuidade e acessibilidade; deixar valores desconhecidos como pendentes

- [ ] P01-09 — Revisar premissas e restrições; avaliar viabilidade inicial, alternativas, disponibilidade, custos e riscos que possam impedir a proposta

- [ ] P01-10 — Delimitar abrangência inicial, exclusões e ideias futuras; não confundir visão de produto com compromisso de funcionalidades do MVP

- [ ] P01-11 — Registrar dúvidas com responsável, condição de retomada e efeito sobre a próxima decisão

- [ ] P01-12 — Consolidar a visão, conferir a cobertura dos itens P01-01 a P01-11 e obter validação e aprovação explícita para orientar o próximo incremento

Artefato/saída: visao-projeto.md, referenciando registros de descoberta, decisões e pendências. Os cartões registram a situação de cada atividade.

Critério de saída: Visão revisada e aprovada; nenhuma dúvida impede compreender problema, produto, objetivo e limites. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-02"></a>

## FASE 2 — LEVANTAMENTO E ANÁLISE DOS PROCESSOS

- [ ] Identificar os processos de negócio envolvidos

- [ ] Mapear o fluxo atual de cada processo relevante

- [ ] Identificar responsáveis por cada etapa

- [ ] Identificar entradas e saídas de cada processo

- [ ] Identificar documentos, planilhas, sistemas e controles existentes

- [ ] Identificar regras aplicadas manualmente

- [ ] Identificar exceções e cenários alternativos

- [ ] Identificar retrabalho, duplicidade e pontos de erro

- [ ] Identificar integrações ou dependências externas

- [ ] Identificar dados históricos existentes e sua qualidade

- [ ] Validar o entendimento dos processos com quem realmente os executa

- [ ] Registrar processos que serão alterados pelo novo sistema

- [ ] Representar o processo desejado e a divisão entre ações humanas e ações do sistema; identificar transição e necessidade de orientação dos usuários

Artefato/saída: Mapa dos processos atuais (AS-IS) e, quando necessário, processos desejados (TO-BE).

Critério de saída: Responsável pela atividade valida cenários principais e exceções relevantes; mudança operacional compreendida. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-03"></a>

## FASE 3 — REQUISITOS E REGRAS DE NEGÓCIO

- [ ] Levantar requisitos funcionais

- [ ] Levantar requisitos não funcionais

- [ ] Identificar regras de negócio

- [ ] Identificar validações obrigatórias

- [ ] Identificar perfis de usuário e permissões

- [ ] Identificar requisitos de autenticação e autorização

- [ ] Identificar necessidades de auditoria e rastreabilidade

- [ ] Identificar relatórios, consultas, filtros e dashboards necessários

- [ ] Identificar notificações e alertas necessários

- [ ] Identificar requisitos de importação e exportação de dados

- [ ] Identificar integrações externas

- [ ] Identificar requisitos de segurança e privacidade

- [ ] Identificar requisitos de desempenho e disponibilidade quando aplicáveis

- [ ] Identificar requisitos de backup, recuperação e retenção de dados

- [ ] Identificar requisitos legais/regulatórios aplicáveis, quando existirem

- [ ] Definir critérios de aceite para requisitos relevantes

- [ ] Eliminar ambiguidades, conflitos e duplicidades

- [ ] Rastrear requisitos até o problema/objetivo que justificou sua existência

- [ ] Revisar e validar requisitos

- [ ] Descrever casos de uso com atores, condições, entradas, saídas, exceções e critérios de aceite

- [ ] Definir interfaces externas, formatos de informação, responsabilidades e tratamento de falhas

- [ ] Identificar origem, responsável, prioridade e situação de cada requisito; vincular a necessidade e ao teste previsto

- [ ] Revisar requisitos com usuários e análise técnica: clareza, consistência, viabilidade e possibilidade de verificação; controlar mudanças após aprovação

Artefato/saída: Documento de Requisitos + Regras de Negócio + Critérios de Aceite.

Critério de saída: Requisitos do próximo incremento são claros, consistentes, viáveis e verificáveis; lacunas bloqueadoras resolvidas. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-04"></a>

## FASE 4 — ESCOPO, MVP E PRIORIZAÇÃO

- [ ] Listar todas as funcionalidades identificadas

- [ ] Classificar funcionalidades essenciais, importantes e futuras

- [ ] Definir o MVP

- [ ] Definir explicitamente o que ficará fora do MVP

- [ ] Identificar dependências entre funcionalidades

- [ ] Priorizar funcionalidades por valor, risco e dependência

- [ ] Identificar riscos técnicos ou de negócio que precisam ser validados cedo

- [ ] Definir entregas incrementais

- [ ] Definir um objetivo de aprendizagem para cada incremento

- [ ] Definir critérios para considerar o MVP concluído

- [ ] Revisar se o MVP resolve o problema principal sem complexidade desnecessária

- [ ] Avaliar viabilidade, esforço e custo do incremento com incertezas explícitas; comparar alternativas quando houver risco relevante

- [ ] Definir um fluxo completo utilizável, sem selecionar apenas componentes técnicos isolados

Artefato/saída: Documento de Escopo/MVP + backlog inicial priorizado.

Critério de saída: Responsável aprova um incremento útil e viável com critérios de conclusão e limites explícitos. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-05"></a>

## FASE 5 — MODELAGEM DO DOMÍNIO

- [ ] Criar glossário dos termos do negócio

- [ ] Identificar entidades e conceitos centrais

- [ ] Identificar atributos relevantes dos conceitos

- [ ] Identificar relacionamentos entre entidades

- [ ] Identificar estados e transições importantes

- [ ] Identificar eventos de negócio

- [ ] Associar regras de negócio às entidades/processos correspondentes

- [ ] Identificar agregações ou limites de responsabilidade somente quando necessários

- [ ] Identificar informações que precisam de histórico

- [ ] Identificar invariantes e consistências obrigatórias

- [ ] Validar o modelo com exemplos reais

- [ ] Evitar modelar o domínio simplesmente copiando telas, planilhas ou tabelas existentes

Artefato/saída: Modelo conceitual de domínio + glossário.

Critério de saída: Exemplos reais percorrem o modelo sem contradições nas regras críticas. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-06"></a>

## FASE 6 — EXPERIÊNCIA DO USUÁRIO E FLUXOS

- [ ] Identificar jornadas principais de cada perfil de usuário

- [ ] Definir fluxo de navegação

- [ ] Definir telas necessárias para o MVP

- [ ] Definir estados vazios, carregamento e erro relevantes

- [ ] Definir validações e feedbacks de interface

- [ ] Produzir wireframes quando agregarem valor

- [ ] Validar se os fluxos suportam os processos e requisitos

- [ ] Validar os fluxos ou protótipos com usuários representativos e registrar dificuldades e ajustes necessários

- [ ] Verificar acessibilidade básica e responsividade esperada

- [ ] Evitar detalhamento visual excessivo antes da validação dos fluxos

Artefato/saída: Fluxos de usuário + wireframes/protótipos necessários.

Critério de saída: Usuário consegue compreender o fluxo principal e a recuperação de erros; observações tratadas. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-07"></a>

## FASE 7 — MODELAGEM DE DADOS

Definir dados e arquitetura (fase 8) em conjunto, conforme o próximo incremento exigir. Confirmar a escolha de persistência antes de detalhar estruturas específicas; os itens relacionais são condicionais à adoção desse modelo.

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

Artefato/saída: Modelo lógico de dados + DER ou representação equivalente + estratégia inicial de migração quando necessária.

Critério de saída: Persistência sustenta regras e consultas críticas; riscos de perda e inconsistência tratados. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-08"></a>

## FASE 8 — ARQUITETURA E DECISÕES TÉCNICAS

- [ ] Identificar drivers arquiteturais: requisitos, riscos, escala e restrições

- [ ] Escolher estilo arquitetural adequado ao estágio do projeto

- [ ] Definir fronteiras entre frontend, backend, banco e serviços externos

- [ ] Escolher tecnologias de frontend

- [ ] Escolher tecnologias de backend

- [ ] Escolher banco de dados

- [ ] Definir estratégia de acesso a dados

- [ ] Definir padrão da API e contratos

- [ ] Definir autenticação e autorização

- [ ] Definir tratamento global de erros

- [ ] Definir validação de entrada

- [ ] Definir logging e observabilidade necessários

- [ ] Definir gerenciamento de configuração e secrets

- [ ] Definir estratégia de arquivos/storage quando aplicável

- [ ] Definir estratégia de cache somente se necessária

- [ ] Definir integrações externas e tratamento de falhas

- [ ] Definir estratégia de versionamento da API quando aplicável

- [ ] Definir ambientes (desenvolvimento, teste/homologação, produção) conforme necessidade

- [ ] Definir estratégia de deploy

- [ ] Definir estratégia de backup e recuperação

- [ ] Registrar decisões arquiteturais importantes e alternativas consideradas

- [ ] Revisar se a arquitetura está proporcional ao problema e ao MVP

- [ ] Avaliar dependências externas, licenças, disponibilidade, custos e possibilidade de substituição quando relevantes

- [ ] Definir limites de responsabilidade e contratos compatíveis entre componentes e versões

Artefato/saída: Documento de Arquitetura + registros de decisões técnicas (ADRs quando úteis).

Critério de saída: Solução proporcional; riscos técnicos principais avaliados; contratos e responsabilidades compreendidos. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-09"></a>

## FASE 9 — SEGURANÇA E PRIVACIDADE

- [ ] Classificar dados sensíveis ou críticos

- [ ] Definir princípio de menor privilégio

- [ ] Revisar autenticação e autorização

- [ ] Definir armazenamento seguro de senhas/credenciais

- [ ] Definir gestão de secrets fora do código-fonte

- [ ] Definir proteção de dados em trânsito

- [ ] Definir proteção de dados armazenados quando necessária

- [ ] Revisar validação e sanitização de entradas

- [ ] Planejar proteção contra vulnerabilidades comuns da stack

- [ ] Definir logs sem exposição indevida de dados sensíveis

- [ ] Definir auditoria para operações críticas

- [ ] Definir política de dependências e atualizações de segurança

- [ ] Definir backup seguro e teste de restauração

- [ ] Registrar riscos aceitos conscientemente

- [ ] Identificar ameaças nas fronteiras e no fluxo de dados, incluindo abuso de permissões

- [ ] Definir resposta a incidentes e responsabilidades; avaliar requisitos aplicáveis de privacidade e descarte com apoio especializado quando necessário

Artefato/saída: Checklist de segurança aplicado ao projeto + riscos registrados.

Critério de saída: Riscos críticos mitigados ou impeditivos; exceções explicitamente avaliadas pelo responsável. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-10"></a>

## FASE 10 — PLANEJAMENTO DO DESENVOLVIMENTO

- [ ] Transformar escopo em épicos

- [ ] Dividir épicos em funcionalidades

- [ ] Dividir funcionalidades em tarefas/issues implementáveis

- [ ] Relacionar issues aos requisitos correspondentes

- [ ] Definir critérios de aceite das issues

- [ ] Identificar dependências entre issues

- [ ] Priorizar ordem de implementação

- [ ] Planejar primeiro os riscos/incertezas relevantes quando necessário

- [ ] Definir milestones/releases quando úteis

- [ ] Definir estratégia de branches

- [ ] Definir padrão de commits

- [ ] Definir fluxo de Pull Request e revisão

- [ ] Definir Definition of Done do projeto/equipe

- [ ] Estimar esforço com incertezas e confrontar o plano com disponibilidade, orçamento e dependências

- [ ] Planejar riscos e mudanças de escopo com responsável, impacto e revisão da prioridade

- [ ] Definir quem executa cada papel e quem aceita a entrega, mesmo quando uma única pessoa acumular funções

Artefato/saída: Backlog executável no GitHub + convenções de trabalho.

Critério de saída: Próximo incremento executável com critérios de aceite, responsável e capacidade disponível. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-11"></a>

## FASE 11 — PREPARAÇÃO DO AMBIENTE E REPOSITÓRIO

- [ ] Inicializar estrutura de frontend

- [ ] Inicializar estrutura de backend

- [ ] Configurar banco de dados local

- [ ] Configurar variáveis de ambiente

- [ ] Configurar arquivo de exemplo de ambiente sem secrets

- [ ] Configurar .gitignore

- [ ] Configurar dependências e gerenciamento de pacotes

- [ ] Configurar formatação/lint quando aplicável

- [ ] Configurar testes

- [ ] Configurar migrations

- [ ] Configurar logging básico

- [ ] Configurar documentação da API quando aplicável

- [ ] Configurar execução local do sistema

- [ ] Documentar pré-requisitos

- [ ] Documentar como instalar e executar

- [ ] Executar build limpo do projeto

- [ ] Confirmar que outro ambiente conseguiria reproduzir a configuração a partir da documentação

- [ ] Preparar verificações automatizadas de integração e entrega quando proporcionais ao projeto; testar seu funcionamento antes de depender delas

Artefato/saída: Projeto executável localmente + README inicial confiável.

Critério de saída: Instalação e execução verificadas; testes e build aplicáveis funcionam; nenhum segredo versionado. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-12"></a>

## FASE 12 — CICLO PADRÃO DE IMPLEMENTAÇÃO DE CADA FUNCIONALIDADE

- [ ] Selecionar uma issue priorizada

- [ ] Confirmar problema/requisito que a issue resolve

- [ ] Revisar critérios de aceite

- [ ] Revisar regras de negócio relacionadas

- [ ] Revisar o objetivo de aprendizagem e explicar o conceito e sua finalidade antes da implementação

- [ ] Propor a solução ou realizar uma tentativa própria, com revisão orientada do raciocínio e da implementação

- [ ] Identificar componentes/arquivos afetados

- [ ] Analisar impactos em dados, API, interface, segurança e funcionalidades existentes

- [ ] Definir a solução mais simples adequada

- [ ] Registrar decisão técnica relevante quando necessário

- [ ] Criar/usar branch conforme convenção adotada e autorização exigida pelo acordo de trabalho

- [ ] Implementar alteração de banco/migration quando necessária

- [ ] Implementar domínio/regra de negócio

- [ ] Implementar backend/API quando necessário

- [ ] Implementar frontend/interface quando necessário

- [ ] Implementar integrações quando necessárias

- [ ] Tratar validações e erros

- [ ] Aplicar autorização/permissões

- [ ] Adicionar ou atualizar testes

- [ ] Executar testes automatizados

- [ ] Executar teste manual do fluxo principal

- [ ] Testar cenários de erro e limites relevantes

- [ ] Revisar código e remover código temporário/debug

- [ ] Revisar legibilidade e consistência com padrões existentes

- [ ] Revisar segurança da alteração

- [ ] Revisar possíveis regressões

- [ ] Atualizar documentação afetada

- [ ] Confirmar todos os critérios de aceite

- [ ] Explicar a decisão adotada e verificar a aprendizagem reproduzindo sua aplicação ou resolvendo uma pequena variação pertinente

- [ ] Revisar diff antes do commit

- [ ] Criar commit claro e focado somente com a autorização exigida pelo acordo de trabalho

- [ ] Enviar alterações ao remoto somente quando autorizado

- [ ] Abrir Pull Request quando aplicável e com a autorização exigida pelo acordo de trabalho

- [ ] Realizar revisão e corrigir apontamentos

- [ ] Integrar alteração somente após aprovação e validação

- [ ] Encerrar issue vinculando evidências/resultados quando aplicável

- [ ] Conferir vínculo entre necessidade, requisito, alteração e evidência de teste; registrar impactos de mudanças nas decisões aprovadas

Artefato/saída: Funcionalidade implementada, testada, documentada e rastreável.

Critério de saída: Critérios de aceite e DoD atendidos; autorização de integração respeitada. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-13"></a>

## FASE 13 — QUALIDADE E TESTES DO SISTEMA

- [ ] Definir estratégia de testes proporcional aos riscos

- [ ] Executar testes unitários

- [ ] Executar testes de integração

- [ ] Executar testes de API

- [ ] Executar testes de interface/E2E quando justificáveis

- [ ] Executar testes de regressão dos fluxos críticos

- [ ] Validar regras de negócio críticas

- [ ] Validar permissões e acessos

- [ ] Validar mensagens e tratamento de erros

- [ ] Validar comportamento com dados inválidos

- [ ] Validar concorrência/consistência quando relevante

- [ ] Validar desempenho dos fluxos críticos quando necessário

- [ ] Validar responsividade e navegadores/dispositivos suportados

- [ ] Validar acessibilidade relevante

- [ ] Executar análise de dependências/vulnerabilidades quando disponível

- [ ] Registrar defeitos encontrados

- [ ] Corrigir defeitos bloqueadores

- [ ] Reexecutar testes após correções

- [ ] Registrar limitações conhecidas

- [ ] Planejar os testes junto aos requisitos, antes de implementar; distinguir verificação técnica de validação do valor para o usuário

- [ ] Registrar requisito coberto, ambiente, dados de teste, resultado esperado, resultado observado e defeitos associados

Artefato/saída: Evidências de testes + bugs conhecidos controlados.

Critério de saída: Requisitos críticos cobertos; defeitos impeditivos resolvidos; limitações aceitas registradas. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-14"></a>

## FASE 14 — DADOS, MIGRAÇÃO E PREPARAÇÃO PARA PRODUÇÃO

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

Artefato/saída: Plano de migração + ambiente preparado para implantação.

Critério de saída: Ensaio demonstra integridade e recuperação; condições para implantação atendidas. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-15"></a>

## FASE 15 — DOCUMENTAÇÃO PARA ENTREGA

- [ ] Atualizar README

- [ ] Documentar arquitetura atual

- [ ] Documentar configuração e variáveis de ambiente

- [ ] Documentar banco/migrations quando necessário

- [ ] Documentar endpoints/API quando aplicável

- [ ] Documentar integrações externas

- [ ] Documentar processo de build

- [ ] Documentar processo de deploy

- [ ] Documentar backup e restauração

- [ ] Documentar procedimentos operacionais importantes

- [ ] Documentar limitações conhecidas

- [ ] Documentar funcionalidades entregues na versão

- [ ] Preparar manual rápido do usuário quando necessário

- [ ] Confirmar que documentação corresponde ao estado real do código

- [ ] Definir responsável por suporte e operação e orientar os usuários sobre a mudança do processo

Artefato/saída: Documentação técnica e operacional da versão.

Critério de saída: Documentação permite executar, usar e recuperar a versão; instruções conferidas. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-16"></a>

## FASE 16 — PRÉ-RELEASE E HOMOLOGAÇÃO

- [ ] Congelar escopo da release

- [ ] Confirmar que todas as funcionalidades previstas estão concluídas ou conscientemente removidas

- [ ] Confirmar critérios de aceite

- [ ] Executar build de release

- [ ] Executar suíte completa de testes aplicável

- [ ] Executar testes de regressão

- [ ] Executar homologação dos principais fluxos

- [ ] Validar dados e migrations

- [ ] Validar configurações de ambiente

- [ ] Validar segurança básica

- [ ] Validar backup/rollback

- [ ] Registrar bugs conhecidos aceitos para a versão

- [ ] Definir número/tag da versão

- [ ] Preparar release notes

- [ ] Obter aprovação para implantação

- [ ] Registrar aceite do usuário para a versão e decisão de seguir ou adiar; distinguir esse aceite da aprovação da visão e da autorização de publicação

Artefato/saída: Release candidata aprovada para produção.

Critério de saída: Responsável aprova implantação com critérios de aceite atendidos e pendências aceitáveis. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-17"></a>

## FASE 17 — DEPLOY E GO-LIVE

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

Artefato/saída: Sistema disponível em produção e versão registrada.

Critério de saída: Fluxos críticos e integridade conferidos; versão disponível ou reversão executada e registrada. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-18"></a>

## FASE 18 — PÓS-DEPLOY E VALIDAÇÃO REAL

- [ ] Monitorar erros após implantação

- [ ] Monitorar comportamento dos fluxos críticos

- [ ] Coletar feedback dos usuários

- [ ] Comparar uso real com os objetivos do projeto

- [ ] Registrar bugs encontrados em produção

- [ ] Priorizar correções

- [ ] Registrar necessidades não previstas

- [ ] Verificar se o sistema realmente substitui/melhora o processo anterior

- [ ] Medir indicadores definidos na visão do projeto quando aplicável

- [ ] Realizar retrospectiva da release

- [ ] Registrar aprendizados técnicos e de processo

- [ ] Comparar os aprendizados com os objetivos do incremento e registrar dúvidas ou conceitos a retomar

Artefato/saída: Feedback real + retrospectiva + backlog atualizado.

Critério de saída: Resultado confrontado com objetivo; ações e responsáveis registrados. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-19"></a>

## FASE 19 — OPERAÇÃO, MANUTENÇÃO E EVOLUÇÃO

- [ ] Manter dependências atualizadas de forma controlada

- [ ] Monitorar vulnerabilidades relevantes

- [ ] Monitorar backups

- [ ] Testar restauração periodicamente quando necessário

- [ ] Monitorar logs, erros e disponibilidade conforme criticidade

- [ ] Corrigir bugs

- [ ] Revisar débitos técnicos relevantes

- [ ] Reavaliar desempenho quando o uso crescer

- [ ] Reavaliar segurança conforme o produto evoluir

- [ ] Reavaliar arquitetura quando houver motivação concreta

- [ ] Priorizar novas funcionalidades com base em valor e evidência

- [ ] Retornar novas funcionalidades ao ciclo de descoberta/requisitos/implementação

- [ ] Atualizar documentação a cada mudança relevante

- [ ] Manter changelog/releases quando útil

- [ ] Definir rotina e responsável por suporte, incidentes, custos e capacidade; registrar causa e ações preventivas de incidentes relevantes

- [ ] Revisar retenção, exportação e descarte de dados e continuidade quando houver mudança de fornecedor ou infraestrutura

Artefato/saída: Produto mantido e roadmap evolutivo.

Critério de saída: Ciclo operacional revisado na periodicidade definida; melhorias voltam à análise de necessidade. Verificar apenas o recorte do incremento ou ciclo em avaliação.

<a id="fase-20"></a>

## FASE 20 — ENCERRAMENTO DA VERSÃO / PROJETO

- [ ] Confirmar que objetivos da versão foram avaliados

- [ ] Confirmar que itens pendentes estão registrados no backlog

- [ ] Confirmar documentação final atualizada

- [ ] Confirmar código versionado e identificável por tag/release quando adotado

- [ ] Confirmar ambiente de produção documentado

- [ ] Confirmar backups e acessos essenciais

- [ ] Registrar decisões pendentes e riscos conhecidos

- [ ] Registrar lições aprendidas

- [ ] Registrar próximos passos do produto

- [ ] Declarar formalmente a versão concluída

- [ ] Distinguir encerramento de versão, encerramento do projeto e retirada do sistema de operação

- [ ] Quando houver retirada de operação, planejar comunicação, exportação e retenção dos dados, transição, revogação de acessos e cancelamento de recursos autorizados

Artefato/saída: Versão encerrada com rastreabilidade e próximos passos claros.

Critério de saída: Resultado e responsabilidades aceitos; continuidade ou encerramento seguro definido; nenhuma pendência sem destino. Verificar apenas o recorte do incremento ou ciclo em avaliação.

## CHECKLIST RÁPIDO — PORTÕES DE QUALIDADE

Usar estes portões como resumo de acompanhamento do incremento ou da versão em avaliação. Consultar o checklist detalhado quando necessário. Registrar a evidência de conclusão ou a justificativa de não aplicabilidade; resolver adiamentos que impeçam a passagem pelo portão.

Antes de aprovar a visão do projeto

- [ ] Problema ou oportunidade, produto proposto, capacidades e limites compreendidos

- [ ] Usuários, interações, condições de uso e restrições identificados

- [ ] Resultado esperado e viabilidade inicial avaliados

- [ ] Pendências bloqueadoras resolvidas e aprovação da visão registrada

Antes de modelar/arquitetar

- [ ] O problema e o objetivo estão claros

- [ ] Os usuários e processos principais são conhecidos

- [ ] Os requisitos essenciais foram levantados

- [ ] O MVP foi delimitado

Antes de começar a implementar

- [ ] O requisito da primeira entrega está claro

- [ ] As regras de negócio necessárias estão documentadas

- [ ] O modelo de domínio/dados necessário para o próximo incremento foi entendido

- [ ] A arquitetura mínima foi decidida

- [ ] O backlog possui itens pequenos e verificáveis

- [ ] O ambiente local está reproduzível

Antes de considerar uma funcionalidade pronta

- [ ] Critérios de aceite atendidos

- [ ] Testes executados

- [ ] Erros e permissões revisados

- [ ] Documentação afetada atualizada

- [ ] Objetivo de aprendizagem avaliado e dúvidas pendentes registradas

- [ ] Diff revisado

- [ ] Alteração rastreável no Git/GitHub

Antes de colocar uma versão em produção

- [ ] Escopo da release definido

- [ ] Testes e homologação concluídos

- [ ] Migrations e dados validados

- [ ] Configurações e secrets revisados

- [ ] Backup/rollback preparados

- [ ] Documentação e release notes atualizadas

- [ ] Autorização de implantação obtida

Antes de declarar a versão concluída

- [ ] Produção validada

- [ ] Feedback inicial coletado

- [ ] Bugs e pendências registrados

- [ ] Documentação corresponde ao sistema

- [ ] Aprendizados registrados

- [ ] Próximos passos definidos

## CONTROLE DE EVOLUÇÃO DO CHECKLIST

- [ ] Registrar no Git toda alteração relevante deste checklist

- [ ] Descrever no commit por que o processo foi alterado

- [ ] Evitar adicionar etapas burocráticas sem benefício prático

- [ ] Remover ou simplificar etapas que não agregarem valor

- [ ] Incorporar aprendizados obtidos em projetos reais

- [ ] Revisar este checklist ao final de cada projeto ou release relevante

Versão 0.1: primeiro checklist mestre. Deve ser refinado a partir da aplicação prática no AgroGest e em projetos futuros.

Versão 0.2: aplicação incremental; estados distintos dos itens; acompanhamento por ciclo; validação antecipada com usuários; objetivos e verificação de aprendizagem; autorizações conforme o acordo de trabalho; modelagem de dados integrada à arquitetura; referências sem duplicação de conteúdo.

Versão 0.3 — 2026-10-16: definição explícita do produto, critérios de saída por fase, rastreabilidade, responsabilidades, viabilidade, gestão de mudanças, operação e retirada de serviço. Referências e adaptação documentadas em mapa-processo.md.
