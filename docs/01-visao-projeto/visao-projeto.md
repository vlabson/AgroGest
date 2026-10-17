# Visão do projeto AgroGest

Status: RASCUNHO — definição inicial incompleta, não aprovada.
Revisão: 2026-10-16. Fonte inicial: [contexto do projeto](contexto-inicial-projeto.md) e decisões já registradas. [Evidências e relatos](registro-discovery.md) serão complementados durante a descoberta.

## 1 Identificação e propósito

AgroGest é o nome do projeto de aplicação web para apoiar a administração rural. O primeiro uso será na Fazenda Garrote. Utilidade real e desenvolvimento profissional do responsável são objetivos declarados. A utilidade específica da primeira entrega ainda precisa ser definida.

## 2 Contexto e atividade

Conhecido: existe uma planilha utilizada pela fazenda com registros reais.
Pendente: atividade a investigar, fluxo resumido, frequência, participantes e documentos usados. A planilha ainda não foi analisada nesta discovery. Não há conclusão de que ela cause erros ou prejuízo.

## 3 Problema ou oportunidade prioritário

A definir com base em relatos e exemplos. Registrar descrição, evidência, consequência, forma atual de lidar com a situação, alternativas já tentadas e justificativa de prioridade. Nenhum problema específico está aprovado.

## 4 Pessoas e responsabilidades

Conhecido: o desenvolvedor responsável será o usuário inicial; existe intenção de uso futuro pelo pai. O responsável pelo projeto decide sua direção.
Pendente: quem realiza cada atividade, quem valida informações de negócio, quem será afetado e quem responderá pela operação. Não presumir que o pai exerce um papel de operação ou aprovação antes de confirmar.

## 5 Definição do produto e capacidades

Definição inicial: aplicação web independente para apoiar a administração rural, com uso inicial em computador. Não pretende simplesmente copiar a estrutura da planilha.
Pendente: capacidades que devem resolver as necessidades identificadas. Para cada capacidade, registrar nome, necessidade, usuário, resultado esperado e situação proposta ou aprovada. Ainda não há módulos ou funcionalidades definidos para o MVP.

## 6 Fronteiras e interações

Conhecido: o usuário inicial interagirá com a aplicação. Há dados históricos na planilha cuja preservação é obrigatória.
Pendente: o que o sistema assumirá, o que continuará humano ou externo, informações de entrada e saída, relação futura com a planilha e eventuais integrações. Preservar histórico não implica importar tudo nem integrar automaticamente.

## 7 Condições de uso e qualidades iniciais

Conhecido: aplicação web com uso inicial em computador; múltiplos níveis de permissão e operação offline não possuem necessidade confirmada.
Pendente: conectividade, local e frequência de uso, acesso e autenticação, sensibilidade dos dados, acessibilidade, volume, disponibilidade e recuperação esperadas. Não confundir ausência de múltiplos perfis com dispensa de proteção de acesso. Qualidades quantitativas serão especificadas nos requisitos quando houver fundamento.

## 8 Objetivos e avaliação do resultado

Objetivos gerais declarados: uso real na administração da fazenda e aprendizagem profissional.
Pendente: objetivo de negócio do primeiro incremento, situação atual de referência, melhoria esperada, indicador ou sinal observável, momento de avaliação e responsável. Não há metas numéricas acordadas.

## 9 Premissas, restrições, viabilidade e riscos

As condições iniciais constam no contexto. Angular e Spring Boot são direcionamentos preliminares; PostgreSQL é candidato. Hospedagem, orçamento disponível, tempo e viabilidade do primeiro incremento precisam ser avaliados. Aprendizagem é um critério legítimo, mas não substitui a análise de utilidade e esforço.

A regra de não alterar a planilha permanece vigente. Seu significado operacional precisa ser esclarecido antes de qualquer alteração nela: impedir alterações pelo projeto não necessariamente significa interromper registros normais da fazenda. Nenhuma mudança foi autorizada por esta observação.

Pendente: comparar alternativas relevantes, avaliar riscos que inviabilizem a proposta e registrar medidas ou aceitação. Referenciar decisões, sem presumir que software é a única alternativa para cada problema.

## 10 Abrangência, exclusões e evolução

Conhecido: entregas incrementais e controle de novas ideias. Outras propriedades, offline, módulos configuráveis e perfis diferentes são possibilidades futuras, sem inclusão automática no MVP.
Pendente: delimitar a primeira atividade e as responsabilidades excluídas. O escopo detalhado e a seleção final de funcionalidades serão consolidados na Fase 04.

## 11 Pendências e riscos para a próxima decisão

| Pendência | Quem deve esclarecer | Momento | Efeito |
|---|---|---|---|
| Atividade, problema, evidências e prioridade | Responsável pelo projeto e conhecedor da atividade | D01 a D03 | Impede aprovar a necessidade prioritária |
| Objetivo e avaliação do resultado | Responsável pelo produto com apoio da análise | D04 | Impede avaliar sucesso |
| Capacidades, fronteiras e interações | Responsável pelo produto com proposta técnica fundamentada | D07 | Impede aprovar a definição inicial do produto |
| Condições de uso, limites, viabilidade e regra da planilha | Responsável pelo projeto; outras fontes a identificar | D05 | Resolver as que afetarem a próxima decisão antes da aprovação |

## 12 Validação e aprovação

Ainda não realizada. A preparação deste rascunho não representa aceite.
Critério: conferir os itens P01-01 a P01-11, validar com as pessoas relevantes e registrar responsável, data, revisão e decisão. Uma pendência não bloqueadora pode permanecer se tiver responsável e condição de retomada; dúvida que impeça compreender produto, necessidade, viabilidade inicial ou objetivo deve ser resolvida.
