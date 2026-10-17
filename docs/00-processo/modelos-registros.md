# Modelos mínimos de registros

Preencher quando a necessidade surgir. Campos sem informação recebem “A definir”, com responsável e condição de retomada. Não transformar exemplo, hipótese ou preferência em requisito aprovado. Os registros podem viver em uma seção de documento ou issue; escolher uma fonte principal.

## Evidência e necessidade

EV-001: data; participante ou fonte; relato; exemplo disponível; distinção entre observado, relatado e suposto; limitações da evidência; confirmação do entendimento.

NEC-001: pessoa ou papel; necessidade; consequência ou oportunidade; EV vinculada; prioridade; situação de validação. Não usar esses identificadores como necessidades reais antes de preenchê-los.

## Capacidade, requisito e teste

CAP-001: o que o produto deverá permitir; necessidade vinculada; usuário; abrangência; situação proposta ou aprovada.

RF-001 ou RNF-001: comportamento ou qualidade exigida; fonte e capacidade; ator; precondição; entrada; resultado; exceções; critério mensurável ou observável; prioridade; dependências; responsável; situação e versão. Regras de negócio usam RN-001 e podem existir independentemente da automação.

TST-001: requisito; cenário; ambiente; dados adequados à publicação; passos; resultado esperado; resultado observado; data; executor; defeito associado. Planejar antes da implementação, executar quando houver comportamento testável.

Para cobertura, manter uma tabela simples: necessidade | capacidade | requisito | issue | teste | resultado de aceitação. Qualquer lacuna crítica deve ter destino explícito antes da entrega.

## Processo, interface e dados

Processo: início e fim; responsável; entradas; etapas; decisões; saídas; exceções; ferramentas; situação atual e desejada; mudanças para o usuário.

Interface: pessoa ou sistema externo; direção da troca; informação; momento; formato quando conhecido; permissão; comportamento em falha; dono da decisão. Não presumir integração automática com uma planilha.

Dados: significado; origem; responsável; identificação; regras; sensibilidade; qualidade; retenção e exclusão; preservação do histórico; necessidades de migração. Detalhar tipos e estruturas na modelagem.

## Dúvida, risco, decisão e alteração

PEN-001: pergunta; por que importa; próximo passo afetado; quem esclarece; data ou condição de retomada; situação; referência da resposta.

RIS-001: causa; evento possível; impacto; probabilidade qualitativa justificada; prioridade; mitigação; responsável; gatilho; risco residual; decisão de aceitar ou bloquear. Um risco não é um fato ocorrido.

DEC-001: questão; alternativas; critérios; escolha; motivo; consequências; responsável e data; situação. Uma decisão substituída permanece histórica e aponta para a nova.

MUD-001: mudança solicitada; motivo; registros e código afetados; impactos; alternativas; decisão do responsável; atualização dos requisitos, testes e plano.

## Issue de trabalho e aprendizagem

Título com resultado esperado. Corpo: contexto já conhecido; lacuna; dependências; entregável; critério de aceite; responsável; evidência de conclusão. Para implementação, incluir requisito de origem e riscos. Acrescentar objetivo de aprendizagem quando pertinente e verificar se o responsável consegue explicar a decisão ou resolver uma variação.

Definition of Ready: próximo trabalho compreendido, entradas disponíveis, critério verificável e impedimentos resolvidos. Definition of Done: critério atendido, revisão e testes pertinentes realizados, documentação atualizada, risco tratado, resultado rastreável e autorizações respeitadas. Adaptar por tipo de atividade; uma entrevista não exige build e um documento não exige testes de código.

## Release, operação e encerramento

Release: versão; escopo; requisitos e testes; aceite do usuário; pendências aceitas; plano de implantação; autorização; backup e recuperação; critérios de reversão; verificação em produção; responsável.

Operação: serviço e dono; rotina de acompanhamento; indicadores; resposta a falhas; backup e ensaio de restauração; custos; suporte; atualização de dependências; revisão periódica. Definir a periodicidade com base na criticidade.

Encerramento: versão ou sistema abrangido; resultado; pendências transferidas; responsável futuro; documentação; acesso aos dados. Se desativar o sistema: comunicação, exportação, retenção, revogação de acessos e desligamento de recursos com autorização específica.

## Aprovação

Objeto e revisão | decisão (aprovado, reprovado ou aprovado com ressalvas) | responsável | data | evidência | ressalvas e impacto.

Não preencher “aprovado” a partir de silêncio, existência de arquivo ou autorização para organizar o processo.
