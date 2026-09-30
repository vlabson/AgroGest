# Contexto Inicial do Projeto

**Projeto:** Sistema de Gestão — Fazenda Garrote  
**Repositório:** `fazenda-garrote-gestao`  
**Status:** Documento inicial evolutivo

## 1. Objetivo deste documento

Registrar as condições conhecidas no início do projeto, separando premissas, restrições, decisões técnicas preliminares, questões ainda em aberto e ideias para evolução futura.

Este documento deve ser atualizado quando uma condição inicial mudar ou quando uma questão em aberto for resolvida. Decisões detalhadas deverão ser registradas posteriormente nos documentos específicos das respectivas fases do projeto.

---

## 2. Premissas

### P01 — Uso inicial
O primeiro uso real do sistema será realizado na Fazenda Garrote.

### P02 — Problema real
O projeto deverá resultar em um sistema efetivamente utilizável na administração da fazenda, não sendo apenas um exercício acadêmico ou projeto demonstrativo.

### P03 — Desenvolvimento profissional
Além de atender às necessidades da Fazenda Garrote, o projeto será utilizado como instrumento de aprimoramento técnico e de desenvolvimento de software do desenvolvedor responsável.

### P04 — Processo atual como referência
A planilha atualmente utilizada na Fazenda Garrote será uma das principais fontes para compreender os processos, controles e dados existentes.

### P05 — Evolução incremental
O sistema será desenvolvido gradualmente, priorizando entregas menores e utilizáveis em vez de tentar construir todo o produto em uma única etapa.

### P06 — Possibilidade de produto
Embora o primeiro uso seja na Fazenda Garrote, existe interesse em avaliar futuramente a transformação da solução em um produto que possa atender outras propriedades rurais.

### P07 — Decisões justificadas
Tecnologias, arquitetura, funcionalidades e abstrações deverão ser adotadas de acordo com necessidades identificadas no projeto, evitando complexidade antecipada sem justificativa técnica ou de negócio.

### P08 — Plataforma inicial
O sistema será utilizado inicialmente em computador.

### P09 — Usuários iniciais
O desenvolvedor responsável será o usuário inicial do sistema. Futuramente, existe a intenção de que seu pai também possa utilizá-lo.

### P10 — Preservação do histórico
Os dados existentes na planilha representam informações reais da Fazenda Garrote. Esse histórico não deverá ser perdido durante a transição para o novo sistema.

---

## 3. Restrições

### R01 — Planilha existente
A planilha atualmente utilizada não deverá ser alterada durante o desenvolvimento do projeto. Ela será utilizada como fonte de análise e referência.

### R02 — Sistema independente
A solução será construída como uma aplicação independente. O objetivo não é simplesmente reproduzir a estrutura da planilha em formato de sistema.

### R03 — Desenvolvimento inicial
O desenvolvimento inicial do sistema deverá ser realizado pelo próprio responsável pelo projeto.

### R04 — Controle de versão
O código-fonte e a documentação relevante do projeto serão versionados utilizando Git e GitHub.

### R05 — Controle de escopo
Novas ideias e funcionalidades não serão automaticamente incorporadas ao escopo. Elas deverão ser analisadas e priorizadas antes de entrarem no desenvolvimento.

### R06 — Simplicidade
Padrões arquiteturais, serviços, infraestrutura, bibliotecas ou abstrações adicionais deverão possuir uma necessidade concreta antes de serem incorporados ao projeto.

---

## 4. Decisões técnicas preliminares

As decisões desta seção representam direcionamentos atuais. Elas poderão ser revisadas caso as fases posteriores revelem requisitos ou restrições que justifiquem uma mudança.

### DT01 — Frontend
Angular será utilizado como tecnologia de frontend.

### DT02 — Backend
Java com Spring Boot será utilizado como tecnologia de backend.

### DT03 — Banco de dados
PostgreSQL é o candidato preferencial neste momento, porém a escolha ainda deverá ser validada tecnicamente durante as fases de modelagem de dados e arquitetura.

### DT04 — Hospedagem
A hospedagem ainda não foi definida. Durante desenvolvimento e validação inicial, será considerada preferencialmente uma alternativa gratuita ou de baixo custo que seja tecnicamente adequada.

---

## 5. Questões em aberto

As questões abaixo não devem ser tratadas como requisitos ou decisões enquanto não forem analisadas nas fases apropriadas.

### D01 — Escopo do MVP
Quais módulos e funcionalidades deverão fazer parte da primeira versão utilizável do sistema?

### D02 — Ordem de desenvolvimento
Qual módulo ou funcionalidade deverá ser implementado primeiro?

### D03 — Relatórios e indicadores
Quais relatórios, indicadores e informações gerenciais serão essenciais para a primeira versão?

### D04 — Migração de dados
Quais dados históricos da planilha serão efetivamente importados para o novo sistema e qual será a estratégia de migração?

> O histórico existente deverá ser preservado. A forma de preservação e migração ainda será definida.

### D05 — Banco de dados
PostgreSQL é tecnicamente a escolha mais adequada para os requisitos que serão identificados?

### D06 — Hospedagem
Onde frontend, backend e banco de dados serão hospedados durante as diferentes etapas do projeto?

### D07 — Backup e recuperação
Qual será a estratégia de backup, retenção e recuperação dos dados?

---

## 6. Ideias para evolução futura

Os itens desta seção representam possibilidades de evolução. Eles **não fazem parte automaticamente do MVP** e somente deverão entrar no escopo após análise e priorização.

### PLUS-01 — Perfis e permissões
Possibilidade de criar diferentes perfis de usuário e níveis de acesso.

No uso inicial, não existe necessidade confirmada de múltiplos níveis de permissão.

### PLUS-02 — Operação offline e sincronização
Possibilidade de utilizar determinadas funcionalidades sem conexão com a internet e sincronizar os dados com a base remota quando a conexão estiver disponível.

Essa funcionalidade deverá passar por análise específica devido ao impacto potencial em armazenamento local, sincronização, resolução de conflitos e arquitetura da aplicação.

### PLUS-03 — Módulos configuráveis
Possibilidade de organizar o produto em módulos que possam ser habilitados conforme as atividades utilizadas por cada propriedade rural.

A necessidade e a complexidade dessa abordagem deverão ser avaliadas antes de qualquer implementação.

### PLUS-04 — Expansão para outras propriedades
Possibilidade de evoluir o sistema para atender propriedades rurais além da Fazenda Garrote.

Antes dessa evolução, deverá ser identificado quais comportamentos são específicos da Fazenda Garrote e quais representam necessidades comuns a outras propriedades.

---

## 7. Controle das questões em aberto

Quando uma questão for resolvida:

1. registrar a decisão no documento correspondente à fase em que ela foi analisada;
2. atualizar sua situação neste documento;
3. evitar duplicar detalhadamente uma decisão que já possua documentação própria;
4. manter a rastreabilidade entre a questão original e a decisão tomada.

---

## 8. Histórico do documento

### Versão inicial
Documento criado durante a Fase 0 — Iniciação e Organização, consolidando as condições iniciais conhecidas antes do início formal da descoberta e visão do projeto.
