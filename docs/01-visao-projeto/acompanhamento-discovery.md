# Acompanhamento da descoberta e visão do projeto

Processo revisão 0.3. A visão está em rascunho; nenhum critério de negócio foi concluído apenas pela revisão do processo.

[Consultar issues](https://github.com/vlabson/AgroGest/issues?q=is%3Aissue%20label%3Afase-01). Os cartões D01 a D07 estão alinhados aos critérios abaixo. D07 explicita a definição do sistema. A discovery ainda não foi iniciada; os cartões permanecem a levantar. As demais fases também estão estruturadas, conforme solicitação do responsável; preparar cartões não significa iniciar sua execução.

[Guia da Fase 01](../fases/01-descoberta-e-visao-do-projeto/README.md) · [Cartão principal](https://github.com/vlabson/AgroGest/issues/12) · [Todas as fases](../fases/README.md)

## Cartões e cobertura

| Cartão | Resultado esperado | Itens do checklist |
|---|---|---|
| [D01](https://github.com/vlabson/AgroGest/issues/1) | Descrever contexto, atividade e pessoas envolvidas | P01-01, P01-03 |
| [D02](https://github.com/vlabson/AgroGest/issues/2) | Registrar necessidades, exemplos e tratamento atual | P01-02 |
| [D03](https://github.com/vlabson/AgroGest/issues/3) | Escolher a necessidade prioritária | P01-04 |
| [D04](https://github.com/vlabson/AgroGest/issues/4) | Definir objetivo e avaliação do resultado | P01-05 |
| [D05](https://github.com/vlabson/AgroGest/issues/5) | Revisar condições, viabilidade, riscos e limites | P01-08, P01-09, P01-10, P01-11 |
| [D06](https://github.com/vlabson/AgroGest/issues/6) | Consolidar e aprovar a visão do sistema | P01-12 |
| [D07](https://github.com/vlabson/AgroGest/issues/7) | Definir produto, capacidades, fronteiras e interações | P01-06, P01-07 |

## Critérios e localização das respostas

| Item | O que precisa estar esclarecido | Cartão | Seção de visao-projeto.md |
|---|---|---|---|
| P01-01 | Descrever o negócio, a atividade e o contexto de uso com fonte das informações | D01 | 2 |
| P01-02 | Registrar problema ou oportunidade, exemplos, frequência conhecida, consequências e tratamento atual; separar fatos relatados de hipóteses | D02 | 3 |
| P01-03 | Identificar usuários, pessoas afetadas, decisor, responsável pela validação e futura operação; permitir que uma pessoa acumule papéis | D01 | 4 |
| P01-04 | Selecionar o problema ou oportunidade prioritário e justificar sua importância | D03 | 3 |
| P01-05 | Definir a melhoria desejada e como avaliar o resultado, incluindo referência atual, sinal de sucesso, momento e responsável | D04 | 8 |
| P01-06 | Descrever o produto proposto e suas capacidades gerais, ligando cada capacidade a uma necessidade; distinguir propostas de decisões aprovadas | D07 | 5 |
| P01-07 | Definir fronteiras do sistema, responsabilidades humanas, interações externas, informações trocadas e relação com controles atuais | D07 | 6 |
| P01-08 | Registrar condições de uso e necessidades iniciais de qualidade: dispositivos, conectividade, acesso, dados críticos, continuidade e acessibilidade; deixar valores desconhecidos como pendentes | D05 | 7 |
| P01-09 | Revisar premissas e restrições; avaliar viabilidade inicial, alternativas, disponibilidade, custos e riscos que possam impedir a proposta | D05 | 9 |
| P01-10 | Delimitar abrangência inicial, exclusões e ideias futuras; não confundir visão de produto com compromisso de funcionalidades do MVP | D05 | 10 |
| P01-11 | Registrar dúvidas com responsável, condição de retomada e efeito sobre a próxima decisão | D05 | 11 |
| P01-12 | Consolidar a visão, conferir a cobertura dos itens P01-01 a P01-11 e obter validação e aprovação explícita para orientar o próximo incremento | D06 | 12 |

## Fluxo de acompanhamento

A levantar → Em levantamento → A validar → Concluído. Manter uma etiqueta de situação por cartão. Bloqueio é uma condição adicional com motivo e responsável; não equivale a conclusão. Adiamento requer destino e não satisfaz o portão afetado. Fechar uma issue só após comprovar seu critério.

D01 e D02 sustentam D03; D03 orienta D04. D07 desenvolve o conceito do produto e interage com D05. D06 depende dos seis trabalhos anteriores, incluindo D07. Retornar a uma etapa é permitido quando surgirem novas informações.

## Fontes principais

- [Mapa completo do processo](../00-processo/mapa-processo.md): entradas, saídas, responsabilidades e critérios até a operação e o encerramento.
- [Checklist mestre](../00-processo/checklist-mestre-desenvolvimento-software.md): verificações do ciclo completo.
- [Contexto inicial](contexto-inicial-projeto.md): ponto de partida das condições conhecidas.
- [Roteiro](roteiro-discovery-fase-1.md): apoio à investigação, incluindo produto e interfaces.
- [Registro](registro-discovery.md): relatos, evidências, hipóteses e dúvidas.
- [Visão](visao-projeto.md): síntese em rascunho a ser completada e aprovada.

Depois de cada conversa, registrar data, fonte e conteúdo; apresentar uma síntese para validação; atualizar decisões e dependências quando necessário. Não duplicar todas as respostas nas issues. Publicação e outras operações seguem o acordo de autorização; o processo não concede aprovação automática.

## Quadro visual e privacidade

Quadro do GitHub Projects ainda pendente de acesso. Os cartões existentes permanecem utilizáveis pela lista de issues. O repositório é público; dados privados e planilhas reais ficam fora dele. Um quadro privado não muda a visibilidade de uma issue pública.
