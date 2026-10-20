# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

No projeto desta equipe, a interface já fazia parte da intenção de desenvolvimento do TCC e, na Entrega 6, foi formalmente tratada como **protótipo digital V0** para fins de análise formativa de IHC.

---

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated em ambiente de simulação. | TCC1 — título, introdução e metodologia. | definido |
| Resultado técnico esperado | Algoritmo híbrido de controle semafórico acompanhado de avaliação experimental em ambiente de simulação. | TCC1 — objetivos e metodologia. | definido |
| O TCC previa interface? | sim, parcialmente definida | A equipe já considerava o desenvolvimento de uma interface antes da disciplina de IHC. Na Entrega 6, essa intenção passou a ser representada por um protótipo digital funcional pré-existente do TCC, denominado V0 para fins da disciplina. | definido |
| Capacidade/contribuição central | Selecionar dinamicamente os movimentos semafóricos prioritários e controlar a permanência ou troca do verde de acordo com o estado observado do tráfego. | TCC1 — proposta do algoritmo Max Pressure + lógica actuated. | definido |
| Possíveis beneficiários/stakeholders | Pesquisadores de mobilidade, analistas/engenheiros de tráfego, gestores de mobilidade, órgãos responsáveis pelo trânsito e, indiretamente, usuários das vias. | Entrega 1 — Seção 2. Os perfis profissionais ainda precisam ser investigados diretamente. | H |
| Usuário escolhido para IHC | Pesquisador ou analista de mobilidade urbana. | H01 — perfil possui relação plausível com configuração, execução e análise de experimentos de controle semafórico. | H |
| Objetivo principal do usuário | Avaliar diferentes estratégias de controle semafórico por meio da configuração, execução e comparação de experimentos em diferentes cenários de tráfego. | Entrega 1 — Seções 3 e 7; aprofundado nas Entregas 3, 4 e 5 e materializado no protótipo V0 da Entrega 6. | H |
| Contexto de uso adotado | Ambiente computacional acadêmico, laboratorial ou profissional voltado à experimentação e análise de estratégias de controle de tráfego. | Entrega 1 — Seção 5; Entrega 3 — contexto de uso consolidado; Entrega 6 — protótipo desktop utilizado como V0. | H |
| Interface/recorte de IHC | Fluxo composto por definição da malha viária, configuração da simulação e da estratégia, execução e acompanhamento e análise/comparação dos resultados. | Deriva das atividades da Entrega 1, das personas e jornada da Entrega 3, dos cenários da Entrega 4, das tarefas aprofundadas na Entrega 5 e dos fluxos PF01–PF03 da Entrega 6. | proposta materializada em V0 |
| Relação com o TCC | parte prevista | A equipe já possuía intenção de desenvolver uma interface antes da disciplina. A Entrega 6 aproveitou o protótipo digital funcional existente no TCC como V0 e o reinterpretou a partir dos métodos de IHC. | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

---

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | H | O perfil escolhido influencia tarefas, linguagem, contexto, personas e decisões de interação. | Entregas 2, 3 e 7 | Entrega 2 — A análise do Aimsun Next e do PTV Vissim identificou ferramentas profissionais que materializam atividades de configuração, execução e análise de simulações de transporte semelhantes às previstas para o projeto. Entrega 3 — P01 foi estruturada como proto-persona primária, consolidando objetivos, necessidades, dores e contexto de uso compatíveis com esse perfil. Entrega 6 — o protótipo V0 foi mapeado para tarefas coerentes com esse perfil, mas isso ainda não representa validação direta com usuários reais. | aberta | H01 permanece aberta e deverá ser investigada diretamente na Entrega 7 e nas avaliações posteriores. |
| H02 | Organizar a interação em definição da malha, configuração/execução e análise dos resultados facilita a realização dos experimentos em relação à interação direta com as ferramentas técnicas. | H | Esse fluxo constitui a estrutura inicial do projeto de interface e precisa ser validado. | Entregas 3, 4, 5, 6 e 7 | Entrega 3 — A jornada de P01 organizou o fluxo entre definição do estudo, preparação do cenário, configuração, execução e análise. Entrega 4 — C01 aprofundou as rupturas relacionadas à preparação e execução de experimentos sob condições comparáveis. Entrega 5 — HTA T02, GOMS T03 e CTT T04/T05 detalharam as tarefas humanas de configuração, seleção da estratégia, início e acompanhamento da execução. Entrega 6 — o protótipo digital V0 foi organizado nos fluxos PF01 — Preparar experimento, PF02 — Executar e acompanhar e PF03 — Analisar e comparar, com estados PP01–PP07. O walkthrough ainda não foi realizado. | aberta | A Entrega 6 materializa H02 em um protótipo real, mas ainda não a valida. O walkthrough e a investigação com usuários deverão verificar se o fluxo é compreensível e adequado. |
| H03 | Uma apresentação comparativa das métricas por meio de dashboard ou relatório facilita a interpretação do desempenho dos métodos. | H | A forma de apresentação influencia a compreensão e comparação dos resultados produzidos pelos experimentos. | Entregas 2, 3, 4, 5, 6, 7 e 12–14 | Entrega 2 — Aimsun Next e PTV Vissim utilizam resumos, listas, séries de dados e gráficos para apresentar e comparar resultados de simulações. Entrega 3 — P01 e P02 indicaram necessidades relacionadas à interpretação e comparação dos resultados. Entrega 4 — C02 aprofundou as dificuldades de contextualizar métricas, verificar comparabilidade e construir uma síntese. Entrega 5 — GOMS T06, HTA T07 e CTT T07/T08 mostraram que a interpretação depende do contexto da execução, da equivalência das condições e da análise conjunta dos indicadores. Entrega 6 — PP06 e PP07 formalizaram, respectivamente, consulta de resultados e comparação de execuções no protótipo V0. Ainda não há evidência do walkthrough. | aberta | H03 permanece aberta. A V0 implementa uma possibilidade de apresentação, mas somente avaliações posteriores poderão indicar se essa representação realmente facilita a interpretação para o perfil de usuário escolhido. |

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Protótipo E6 | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Utilização de diferentes malhas e cenários no ambiente experimental. | Definir corretamente onde e em quais condições o experimento será realizado. | P01 | C01 | T01 — definir ou selecionar a malha viária. | PENDENTE | PF01 / PP01 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R02 | Configuração dos parâmetros utilizados nos experimentos. | Definir corretamente as condições da simulação antes da execução. | P01 | C01 | T02 — configurar parâmetros do experimento. | HTA — T02 | PF01 / PP02 / PP03 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R03 | Execução de diferentes estratégias de controle semafórico. | Selecionar claramente qual estratégia será utilizada em cada experimento. | P01 | C01 | T03 — selecionar a estratégia de controle. | GOMS — T03 | PF01 / PP02 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R04 | Execução automatizada do ambiente experimental. | Realizar o experimento configurado e compreender seu estado de execução. | P01 | C01 | T04 — iniciar uma simulação; T05 — verificar o estado da execução. | CTT — T04/T05 | PF02 / PP03 / PP04 / PP05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R05 | Produção de métricas de desempenho das simulações. | Compreender o desempenho obtido em cada experimento. | P01, P02 | C02 | T06 — consultar as métricas obtidas. | GOMS — T06 | PF03 / PP06 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R06 | Comparação experimental entre tempo fixo, Max Pressure e Max Pressure + actuated. | Comparar o comportamento das estratégias sob condições equivalentes. | P01, P02 | C02 | T07 — comparar resultados. | HTA — T07; CTT — T07/T08 | PF03 / PP07 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R07 | Geração e organização dos resultados experimentais. | Registrar e comunicar os resultados obtidos em uma execução ou comparação. | P01, P02 | C02 | T08 — consultar ou gerar uma síntese dos resultados. | CTT — T07/T08 | PF03 / PP06 / PP07 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |

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

Os campos das entregas futuras permanecem como `PENDENTE` enquanto seus respectivos artefatos ainda não existirem.

---

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

Ainda não existem telas de Figma definidas. Os identificadores `F01`, `F02` etc. permanecem reservados para a Entrega 11.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| PF01 / PP01 | Entrada/seleção da malha | T01 | Definir a malha ou cenário no qual a simulação será realizada. | H02 + Entregas 1, 3 e 4; Entrega 6 formalizou esse passo como primeiro estado do fluxo de preparação. | R01 |
| PF01 / PP02 / PP03 | Configuração/parametrização | T02 e T03 | Definir parâmetros experimentais, selecionar estratégia e prevenir configurações inválidas. | H02 + Entrega 5: HTA T02 e GOMS T03; Entrega 6: PP02 materializa a configuração e PP03 explicita validação/prevenção de erro. | R02, R03 |
| PF02 / PP04 / PP05 | Acompanhamento de processamento | T04 e T05 | Iniciar a simulação, acompanhar estado/progresso e inspecionar a execução Visual. | Entrega 2: padrões semelhantes em Aimsun Next e PTV Vissim; Entrega 5: CTT T04/T05; Entrega 6: PP04 e PP05 materializam processamento e acompanhamento. | R04 |
| PF03 / PP06 | Resultados/visão de métricas | T06 e T08 | Consultar resultados mantendo cenário, controlador, seed e demais condições associados. | H03 + Entregas 4 e 5; Entrega 6 formalizou PP06 como estado de consulta de resultados. | R05, R07 |
| PF03 / PP07 | Comparação | T07 e T08 | Comparar execuções compatíveis e interpretar diferenças entre estratégias. | H03 + Entrega 5: HTA T07 e CTT T07/T08; Entrega 6 formalizou PP07 como estado de comparação. | R06, R07 |
| Apoio a PP06/PP07 | Histórico | T06 e T07 | Recuperar execuções anteriores quando necessário à análise e comparação. | GOMS T06 mostrou a necessidade de localizar execuções. A Entrega 6 reconhece o histórico existente como recurso de apoio, sem tratá-lo como objetivo principal. | R05, R06 |
| PENDENTE | Administração | PENDENTE | Não existe atividade de administração de usuários/permissões identificada no escopo atual. | Não há evidência que justifique essa família de interface. | PENDENTE |

> A presença de um padrão na interface existente não significa que ele esteja validado. A Entrega 6 apenas formaliza sua relação com as tarefas. Walkthroughs e avaliações posteriores deverão verificar sua adequação.

### Decisões de interação derivadas até a Entrega 6

As entregas realizadas até o momento sustentam as seguintes necessidades de interação:

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

---

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| — | Nenhuma mudança formal de escopo registrada até o momento. | As Entregas 2–6 aprofundaram usuários, cenários, tarefas e interface sem alterar o recorte principal definido na Entrega 1. | — | — |

### Refinamento registrado na Entrega 6

A utilização do protótipo digital funcional pré-existente do TCC em substituição à criação de uma nova versão física em papel **não constitui mudança de escopo**.

O protótipo existente passou a ser denominado **V0** e foi reorganizado conceitualmente segundo os fluxos PF01, PF02 e PF03 e os estados PP01–PP07.

Esse refinamento altera a forma de documentar e avaliar a solução, mas não altera:

- o usuário priorizado;
- os cenários C01 e C02;
- as tarefas T01–T08;
- o objetivo principal do projeto de IHC.

---

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `PF01`, `PP01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
- A existência de uma persona, cenário, análise de tarefa ou protótipo funcional não transforma automaticamente uma hipótese em fato validado.
- Ao concluir uma nova entrega, atualize somente as colunas e hipóteses para as quais houve nova evidência.
- Preserve `PENDENTE` quando um artefato futuro ainda não tiver sido produzido.
- A presença de um estado `PPxx` indica que ele foi documentado na Entrega 6, não que já tenha sido validado por usuário.

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
| M | Modelo/MoLIC |
| F | Tela ou fluxo do protótipo no Figma |
| UT | Tarefa utilizada em teste com usuário |
| R | Linha de rastreabilidade |

Os identificadores serão criados somente quando o respectivo artefato existir. Até lá, os campos permanecerão como `PENDENTE`.
