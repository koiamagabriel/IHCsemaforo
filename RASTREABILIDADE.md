# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

No projeto desta equipe, a interface já fazia parte da intenção de desenvolvimento do TCC e, na Entrega 6, foi formalmente tratada como **protótipo digital V0** para fins de análise formativa de IHC.

Na Entrega 7, as principais hipóteses ainda abertas foram transformadas em um **plano de investigação reproduzível**, composto por um questionário e uma entrevista semiestruturada. Como esses instrumentos não foram aplicados nesta etapa, sua elaboração não é tratada como evidência empírica e as hipóteses permanecem abertas.

---

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated em ambiente de simulação. | TCC1 — título, introdução e metodologia. | definido |
| Resultado técnico esperado | Algoritmo híbrido de controle semafórico acompanhado de avaliação experimental em ambiente de simulação. | TCC1 — objetivos e metodologia. | definido |
| O TCC previa interface? | sim, parcialmente definida | A equipe já considerava o desenvolvimento de uma interface antes da disciplina de IHC. Na Entrega 6, essa intenção passou a ser representada por um protótipo digital funcional pré-existente do TCC, denominado V0 para fins da disciplina. | definido |
| Capacidade/contribuição central | Selecionar dinamicamente os movimentos semafóricos prioritários e controlar a permanência ou troca do verde de acordo com o estado observado do tráfego. | TCC1 — proposta do algoritmo Max Pressure + lógica actuated. | definido |
| Possíveis beneficiários/stakeholders | Pesquisadores de mobilidade, analistas/engenheiros de tráfego, gestores de mobilidade, órgãos responsáveis pelo trânsito e, indiretamente, usuários das vias. | Entrega 1 — Seção 2. A Entrega 7 definiu instrumentos capazes de investigar esses perfis, mas ainda não houve coleta empírica. | H |
| Usuário escolhido para IHC | Pesquisador ou analista de mobilidade urbana. | H01 — perfil possui relação plausível com configuração, execução e análise de experimentos de controle semafórico. A Entrega 7 planejou investigação específica dessa hipótese. | H |
| Objetivo principal do usuário | Avaliar diferentes estratégias de controle semafórico por meio da configuração, execução e comparação de experimentos em diferentes cenários de tráfego. | Entrega 1 — Seções 3 e 7; aprofundado nas Entregas 3, 4 e 5; materializado no protótipo V0 da Entrega 6; investigável pelos instrumentos da Entrega 7. | H |
| Contexto de uso adotado | Ambiente computacional acadêmico, laboratorial ou profissional voltado à experimentação e análise de estratégias de controle de tráfego. | Entrega 1 — Seção 5; Entrega 3 — contexto de uso consolidado; Entrega 6 — protótipo desktop utilizado como V0; Entrega 7 — público e critérios de coleta planejados. | H |
| Interface/recorte de IHC | Fluxo composto por definição da malha viária, configuração da simulação e da estratégia, execução e acompanhamento e análise/comparação dos resultados. | Deriva das atividades da Entrega 1, das personas e jornada da Entrega 3, dos cenários da Entrega 4, das tarefas aprofundadas na Entrega 5 e dos fluxos PF01–PF03 da Entrega 6. A Entrega 7 definiu como investigar as premissas que sustentam esse recorte. | proposta materializada em V0 |
| Relação com o TCC | parte prevista | A equipe já possuía intenção de desenvolver uma interface antes da disciplina. A Entrega 6 aproveitou o protótipo digital funcional existente no TCC como V0 e o reinterpretou a partir dos métodos de IHC. | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

---

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida / instrumento planejado | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | H | O perfil escolhido influencia tarefas, linguagem, contexto, personas e decisões de interação. | Entregas 2, 3 e 7; avaliações posteriores | Entrega 2 — A análise do Aimsun Next e do PTV Vissim identificou ferramentas profissionais que materializam atividades de configuração, execução e análise de simulações de transporte semelhantes às previstas. Entrega 3 — P01 e P02 foram estruturadas como proto-personas. Entrega 6 — o protótipo V0 foi relacionado a tarefas compatíveis com esses perfis. Entrega 7 — I01/Q01–Q04 e I02/E01–E02 foram planejados para investigar área, papel, experiência e ferramentas. Os instrumentos não foram aplicados. | aberta | A plausibilidade do perfil foi reforçada documentalmente, mas ainda não existe validação direta. Personas e vocabulário permanecem sujeitos a refinamento futuro. |
| H02 | Organizar a interação em definição da malha, configuração/execução e análise dos resultados facilita a realização dos experimentos em relação à interação direta com as ferramentas técnicas. | H | Esse fluxo constitui a estrutura inicial do projeto de interface e precisa ser validado. | Entregas 3, 4, 5, 6 e 7; avaliações posteriores | Entrega 3 — jornada organizada entre definição, preparação, execução e análise. Entrega 4 — C01 aprofundou rupturas de preparação e execução. Entrega 5 — HTA T02, GOMS T03 e CTT T04/T05 detalharam as tarefas. Entrega 6 — materialização em PF01, PF02 e PF03. Entrega 7 — I01/Q05–Q09 e I02/E03–E08 foram planejados para investigar preparação, parâmetros, validação, feedback, erros e recuperação. Os instrumentos não foram aplicados. | aberta | H02 permanece como hipótese de design. A Entrega 7 definiu como investigá-la sem transformar o fluxo existente em fato validado. |
| H03 | Uma apresentação comparativa das métricas por meio de dashboard ou relatório facilita a interpretação do desempenho dos métodos. | H | A forma de apresentação influencia a compreensão e comparação dos resultados produzidos pelos experimentos. | Entregas 2, 3, 4, 5, 6 e 7; Entregas 12–14 | Entrega 2 — interfaces profissionais utilizam resumos, listas e visualizações de resultados. Entrega 3 — P01 e P02 possuem necessidades hipotéticas de interpretação e comparação. Entrega 4 — C02 aprofundou contextualização e comparabilidade. Entrega 5 — GOMS T06, HTA T07 e CTT T07/T08 aprofundaram análise e síntese. Entrega 6 — PP06 e PP07 formalizaram resultados e comparação. Entrega 7 — I01/Q10–Q17 e I02/E09–E20 foram planejados para investigar métricas, comparação, histórico, rastreabilidade, linguagem e síntese. Os instrumentos não foram aplicados. | aberta | H03 permanece aberta. A Entrega 7 evita assumir previamente que dashboard, histórico, gráficos ou filtros sejam necessários e fornece meios para investigar essas possibilidades. |

### Situação após a Entrega 7

A Entrega 7 **não produziu evidência empírica nova**, pois seus instrumentos foram planejados e documentados, mas não aplicados.

Portanto:

- H01 continua **aberta**;
- H02 continua **aberta**;
- H03 continua **aberta**.

A contribuição da Entrega 7 está em tornar essas hipóteses **investigáveis por procedimentos reproduzíveis**, sem confundir planejamento de pesquisa com validação.

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Protótipo E6 | Coleta E7 | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Utilização de diferentes malhas e cenários no ambiente experimental. | Definir corretamente onde e em quais condições o experimento será realizado. | P01 | C01 | T01 — definir ou selecionar a malha viária. | PENDENTE | PF01 / PP01 | I01 — Q05; I02 — E03/E04 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R02 | Configuração dos parâmetros utilizados nos experimentos. | Definir corretamente as condições da simulação antes da execução. | P01 | C01 | T02 — configurar parâmetros do experimento. | HTA — T02 | PF01 / PP02 / PP03 | I01 — Q05–Q07; I02 — E03–E05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R03 | Execução de diferentes estratégias de controle semafórico. | Selecionar claramente qual estratégia será utilizada em cada experimento. | P01 | C01 | T03 — selecionar a estratégia de controle. | GOMS — T03 | PF01 / PP02 | I01 — Q05/Q06; I02 — E04/E05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R04 | Execução automatizada do ambiente experimental. | Realizar o experimento configurado e compreender seu estado de execução. | P01 | C01 | T04 — iniciar uma simulação; T05 — verificar o estado da execução. | CTT — T04/T05 | PF02 / PP03 / PP04 / PP05 | I01 — Q08/Q09; I02 — E06–E08 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R05 | Produção de métricas de desempenho das simulações. | Compreender o desempenho obtido em cada experimento. | P01, P02 | C02 | T06 — consultar as métricas obtidas. | GOMS — T06 | PF03 / PP06 | I01 — Q10/Q11; I02 — E09/E10/E13 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R06 | Comparação experimental entre tempo fixo, Max Pressure e Max Pressure + actuated. | Comparar o comportamento das estratégias sob condições equivalentes. | P01, P02 | C02 | T07 — comparar resultados. | HTA — T07; CTT — T07/T08 | PF03 / PP07 | I01 — Q12/Q13; I02 — E11–E13 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R07 | Geração e organização dos resultados experimentais. | Registrar e comunicar os resultados obtidos em uma execução ou comparação. | P01, P02 | C02 | T08 — consultar ou gerar uma síntese dos resultados. | CTT — T07/T08 | PF03 / PP06 / PP07 | I01 — Q10–Q17; I02 — E14–E20 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |

### Observação sobre a Entrega 5

A tarefa T01 permanece sem um artefato específico de HTA, GOMS ou CTT na Entrega 5. Isso não representa ausência da tarefa no projeto: T01 continua como parte do fluxo principal e como pré-requisito para as atividades seguintes.

A Entrega 5 aprofundou especificamente:

- T02 por meio de HTA;
- T03 por meio de GOMS;
- T04/T05 por meio de CTT;
- T06 por meio de GOMS;
- T07 por meio de HTA e também no CTT T07/T08;
- T08 por meio do CTT T07/T08.

### Observação sobre a Entrega 6

A Entrega 6 materializou as tarefas anteriores no protótipo digital V0 por meio de três fluxos:

- **PF01 — Preparar experimento:** T01, T02 e T03;
- **PF02 — Executar e acompanhar simulação:** T04 e T05;
- **PF03 — Analisar e comparar resultados:** T06, T07 e T08.

Os estados documentados são:

- **PP01:** catálogo e seleção do cenário;
- **PP02:** configuração da simulação;
- **PP03:** validação e prevenção de erro;
- **PP04:** execução em andamento;
- **PP05:** execução no modo Visual;
- **PP06:** resultados da execução;
- **PP07:** comparação de execuções.

Neste momento, esses estados representam a estrutura planejada/documentada da V0. As evidências visuais e o walkthrough ainda devem ser adicionados antes de a Entrega 6 ser marcada como concluída.

### Observação sobre a Entrega 7

A Entrega 7 produziu dois instrumentos completos e complementares:

- **I01 — Questionário exploratório sobre atividades de simulação e análise**, de Gabriel Koiama de Rocha Lira;
- **I02 — Entrevista semiestruturada sobre processos técnicos e interpretação de resultados**, de João Pedro Lopes Santana Villas Bôas.

I01 investiga de forma estruturada:

- perfil e experiência;
- preparação e configuração;
- execução e acompanhamento;
- resultados e comparação;
- linguagem e necessidades.

I02 aprofunda qualitativamente:

- contexto e experiência;
- processo de preparação;
- decisões;
- erros e recuperação;
- feedback;
- interpretação de resultados;
- critérios de comparação;
- histórico e rastreabilidade;
- comunicação e linguagem;
- necessidades não antecipadas.

Os instrumentos estão prontos para eventual aplicação, mas **não foram executados nesta entrega**. Consequentemente, sua existência não altera o estado de H01, H02 ou H03.

Os campos das entregas futuras permanecem como `PENDENTE` enquanto seus respectivos artefatos ainda não existirem.

---

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

Ainda não existem telas de Figma definidas. Os identificadores `F01`, `F02` etc. permanecem reservados para a Entrega 11.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade / investigação planejada | Artefatos relacionados |
|---|---|---|---|---|---|
| PF01 / PP01 | Entrada/seleção da malha | T01 | Definir a malha ou cenário no qual a simulação será realizada. | H02 + Entregas 1, 3 e 4; Entrega 6 formalizou esse passo como primeiro estado do fluxo. A Entrega 7 inclui questões sobre preparação e informações conferidas antes da execução. | R01 |
| PF01 / PP02 / PP03 | Configuração/parametrização | T02 e T03 | Definir parâmetros experimentais, selecionar estratégia e prevenir configurações inválidas. | H02 + Entrega 5: HTA T02 e GOMS T03; Entrega 6: PP02/PP03; Entrega 7: I01 Q05–Q07 e I02 E03–E05 investigam parâmetros, preparação e prevenção de erros. | R02, R03 |
| PF02 / PP04 / PP05 | Acompanhamento de processamento | T04 e T05 | Iniciar a simulação, acompanhar estado/progresso e inspecionar a execução Visual. | Entrega 2: padrões semelhantes em ferramentas profissionais; Entrega 5: CTT T04/T05; Entrega 6: PP04/PP05; Entrega 7: I01 Q08–Q09 e I02 E06–E08 investigam feedback, progresso, erros e cancelamento. | R04 |
| PF03 / PP06 | Resultados/visão de métricas | T06 e T08 | Consultar resultados mantendo cenário, controlador, seed e demais condições associados. | H03 + Entregas 4–6; Entrega 7: I01 Q10/Q11 e I02 E09/E10/E13 investigam prioridade e interpretação das informações. | R05, R07 |
| PF03 / PP07 | Comparação | T07 e T08 | Comparar execuções compatíveis e interpretar diferenças entre estratégias. | H03 + Entrega 5: HTA T07 e CTT T07/T08; Entrega 6: PP07; Entrega 7: I01 Q12/Q13 e I02 E11–E13 investigam formas e critérios de comparação. | R06, R07 |
| Apoio a PP06/PP07 | Histórico | T06 e T07 | Recuperar execuções anteriores quando necessário à análise e comparação. | A necessidade ainda não foi validada. A Entrega 7 deliberadamente investiga como resultados antigos são recuperados por meio de I01 Q14 e I02 E14/E15, sem pressupor que busca/filtros sejam obrigatórios. | R05, R06 |
| PENDENTE | Administração | PENDENTE | Não existe atividade de administração de usuários/permissões identificada no escopo atual. | Não há evidência nem hipótese prioritária que justifique essa família de interface. | PENDENTE |

> A existência de um padrão no protótipo atual não significa que sua necessidade ou forma de apresentação já tenha sido validada. A Entrega 7 planeja investigar essas decisões sem transformá-las antecipadamente em requisitos definitivos.

---

## 5. Decisões e questões de interação até a Entrega 7

### Decisões derivadas das Entregas 1–6

As entregas anteriores sustentaram, como hipóteses e decisões de projeto a serem posteriormente avaliadas:

- manter cenário, demanda, parâmetros, controlador e seed associados à execução;
- permitir seleção explícita de cenário/infraestrutura;
- agrupar parâmetros de forma compreensível;
- validar parâmetros relevantes antes do início da simulação;
- impedir ou sinalizar configurações incompletas ou incompatíveis;
- diferenciar claramente modo Visual e Headless;
- apresentar feedback sobre início, processamento, cancelamento, erro e conclusão;
- permitir que o usuário reconheça qual estratégia está sendo executada;
- manter os resultados ligados às condições experimentais que os produziram;
- permitir a interpretação conjunta das métricas;
- preservar o contexto da execução durante a análise;
- verificar compatibilidade antes de tratar duas execuções como comparáveis;
- permitir recuperação de execuções anteriores quando isso for necessário à análise;
- não introduzir recursos administrativos ou CRUDs genéricos sem tarefa que os justifique;
- tratar o protótipo existente como hipótese de design, e não como interface automaticamente validada.

### Questões formalizadas pela Entrega 7

A Entrega 7 não adicionou novas conclusões sobre usuários. Ela formalizou perguntas que poderão orientar revisões futuras, incluindo:

- qual perfil realmente realiza atividades semelhantes às assumidas para P01 e P02;
- quais ferramentas e termos são familiares a esse perfil;
- quais parâmetros precisam estar visíveis;
- quais configurações devem ser verificadas antes da execução;
- quais erros são considerados mais críticos;
- que feedback é necessário durante processamento;
- quais métricas são consultadas primeiro;
- como diferentes resultados são comparados;
- quais condições definem comparabilidade;
- se histórico, busca ou filtros são de fato necessários;
- qual equilíbrio entre síntese e detalhamento técnico é mais apropriado;
- como resultados são comunicados a pessoas com diferentes níveis de conhecimento.

Essas questões serão tratadas como investigação planejada, e não como evidência obtida.

---

## 6. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| — | Nenhuma mudança formal de escopo registrada até o momento. | As Entregas 2–7 aprofundaram usuários, cenários, tarefas, interface e plano de investigação sem alterar o recorte principal definido na Entrega 1. | — | — |

### Refinamento registrado na Entrega 6

A utilização do protótipo digital funcional pré-existente do TCC em substituição à criação de uma nova versão física em papel **não constitui mudança de escopo**.

O protótipo existente passou a ser denominado **V0** e foi reorganizado conceitualmente segundo os fluxos PF01, PF02 e PF03 e os estados PP01–PP07.

Esse refinamento altera a forma de documentar e avaliar a solução, mas não altera:

- o usuário priorizado;
- os cenários C01 e C02;
- as tarefas T01–T08;
- o objetivo principal do projeto de IHC.

### Refinamento registrado na Entrega 7

A Entrega 7 também **não representa mudança de escopo**.

Foram produzidos instrumentos para investigar as hipóteses existentes:

- I01 — questionário;
- I02 — entrevista semiestruturada.

A equipe também registrou a possibilidade de utilização futura de participantes proxy caso o acesso ao público profissional especializado seja inviável.

Essa possibilidade metodológica não altera automaticamente as personas nem transforma participantes proxy em representantes equivalentes do público especializado.

Como não houve aplicação dos instrumentos, nenhuma hipótese ou requisito foi alterado com base em dados de usuários nesta etapa.

---

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `PF01`, `PP01`, `I01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
- A existência de uma persona, cenário, análise de tarefa, protótipo ou instrumento de pesquisa não transforma automaticamente uma hipótese em fato validado.
- Um instrumento planejado deve ser distinguido de dados realmente coletados.
- Ao concluir uma nova entrega, atualize somente as colunas e hipóteses para as quais houve nova evidência ou novo artefato.
- Preserve `PENDENTE` quando um artefato futuro ainda não tiver sido produzido.
- A presença de um estado `PPxx` indica que ele foi documentado na Entrega 6, não que já tenha sido validado por usuário.
- A presença de `I01` ou `I02` indica que existe um instrumento planejado na Entrega 7, não que ele tenha sido aplicado.

---

## Convenção de identificadores adotada

Para manter a rastreabilidade consistente ao longo do semestre, serão utilizados os seguintes identificadores:

| Prefixo | Artefato |
|---|---|
| H | Hipótese ou lacuna relevante |
| P | Persona |
| C | Cenário |
| T | Tarefa/objetivo do usuário |
| PF | Fluxo do protótipo da Entrega 6 |
| PP | Tela/estado do protótipo da Entrega 6 |
| I | Instrumento de coleta da Entrega 7 |
| Q | Pergunta do questionário I01 |
| E | Pergunta da entrevista I02 |
| M | Modelo/MoLIC |
| F | Tela ou fluxo do protótipo no Figma |
| UT | Tarefa utilizada em teste com usuário |
| R | Linha de rastreabilidade |

Os identificadores serão criados somente quando o respectivo artefato existir. Até lá, os campos permanecerão como `PENDENTE`.
