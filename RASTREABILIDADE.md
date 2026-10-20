# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated em ambiente de simulação. | TCC1 — título, introdução e metodologia. | definido |
| Resultado técnico esperado | Algoritmo híbrido de controle semafórico acompanhado de avaliação experimental em ambiente de simulação. | TCC1 — objetivos e metodologia. | definido |
| O TCC previa interface? | sim, parcialmente definida | A equipe já considerava o desenvolvimento de uma interface antes da disciplina de IHC, porém ela ainda não está formalmente detalhada no documento atual do TCC1. | definido |
| Capacidade/contribuição central | Selecionar dinamicamente os movimentos semafóricos prioritários e controlar a permanência ou troca do verde de acordo com o estado observado do tráfego. | TCC1 — proposta do algoritmo Max Pressure + lógica actuated. | definido |
| Possíveis beneficiários/stakeholders | Pesquisadores de mobilidade, analistas/engenheiros de tráfego, gestores de mobilidade, órgãos responsáveis pelo trânsito e, indiretamente, usuários das vias. | Entrega 1 — Seção 2. Os perfis profissionais ainda precisam ser investigados diretamente. | H |
| Usuário escolhido para IHC | Pesquisador ou analista de mobilidade urbana. | H01 — perfil possui relação plausível com configuração, execução e análise de experimentos de controle semafórico. | H |
| Objetivo principal do usuário | Avaliar diferentes estratégias de controle semafórico por meio da configuração, execução e comparação de experimentos em diferentes cenários de tráfego. | Entrega 1 — Seções 3 e 7; aprofundado nas Entregas 3, 4 e 5. | H |
| Contexto de uso adotado | Ambiente computacional acadêmico, laboratorial ou profissional voltado à experimentação e análise de estratégias de controle de tráfego. | Entrega 1 — Seção 5; Entrega 3 — contexto de uso consolidado. | H |
| Interface/recorte de IHC | Fluxo composto por definição da malha viária, configuração da simulação e da estratégia, execução e acompanhamento e análise/comparação dos resultados. | Deriva das atividades da Entrega 1, das personas e jornada da Entrega 3, dos cenários da Entrega 4 e das tarefas aprofundadas na Entrega 5. | proposta |
| Relação com o TCC | parte prevista | A equipe já possuía intenção de desenvolver uma interface antes da disciplina, mas seu usuário, fluxo e requisitos de interação ainda não estavam formalmente definidos. A disciplina aprofunda essa proposta. | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

---

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | H | O perfil escolhido influencia tarefas, linguagem, contexto, personas e decisões de interação. | Entregas 2, 3 e 7 | Entrega 2 — A análise do Aimsun Next e do PTV Vissim identificou ferramentas profissionais que materializam atividades de configuração, execução e análise de simulações de transporte semelhantes às previstas para o projeto. Entrega 3 — P01 foi estruturada como proto-persona primária, consolidando objetivos, necessidades, dores e contexto de uso compatíveis com esse perfil. Essas evidências reforçam a plausibilidade do usuário priorizado, mas ainda não representam validação direta com usuários reais. | aberta | As Entregas 2 e 3 reforçam a plausibilidade do perfil escolhido, mas H01 permanece aberta e deverá ser investigada diretamente com usuários ou especialistas na Entrega 7. |
| H02 | Organizar a interação em definição da malha, configuração/execução e análise dos resultados facilita a realização dos experimentos em relação à interação direta com as ferramentas técnicas. | H | Esse fluxo constitui a estrutura inicial do projeto de interface e precisa ser validado. | Entregas 3, 4, 5, 6 e 7 | Entrega 3 — A jornada de P01 organizou o fluxo entre definição do estudo, preparação do cenário, configuração, execução e análise. Entrega 4 — C01 aprofundou as rupturas relacionadas à preparação e execução de experimentos sob condições comparáveis. Entrega 5 — HTA T02, GOMS T03 e CTT T04/T05 detalharam as tarefas humanas de configuração, seleção da estratégia, início e acompanhamento da execução, evidenciando necessidades de validação, feedback e rastreabilidade. Esses artefatos aprofundam a hipótese, mas ainda não constituem validação direta com usuários. | aberta | H02 permanece aberta. A análise de tarefas indica requisitos e rupturas que deverão orientar a prototipação e posterior avaliação com usuários. |
| H03 | Uma apresentação comparativa das métricas por meio de dashboard ou relatório facilita a interpretação do desempenho dos métodos. | H | A forma de apresentação influencia a compreensão e comparação dos resultados produzidos pelos experimentos. | Entregas 2, 3, 4, 5, 6, 7 e 12–14 | Entrega 2 — Aimsun Next e PTV Vissim utilizam resumos, listas, séries de dados e gráficos para apresentar e comparar resultados de simulações. Entrega 3 — P01 e P02 indicaram necessidades relacionadas à interpretação e comparação dos resultados. Entrega 4 — C02 aprofundou as dificuldades de contextualizar métricas, verificar comparabilidade e construir uma síntese dos resultados. Entrega 5 — GOMS T06, HTA T07 e CTT T07/T08 mostraram que a interpretação depende do contexto da execução, da equivalência das condições e da análise conjunta dos indicadores. Essas evidências ainda não confirmam qual formato de apresentação será mais adequado ao usuário. | aberta | H03 permanece aberta para validação por prototipação e avaliação com usuários. A análise de tarefas reforça a necessidade de preservar contexto, comparação e síntese sem definir antecipadamente uma solução visual específica. |

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Utilização de diferentes malhas e cenários no ambiente experimental. | Definir corretamente onde e em quais condições o experimento será realizado. | P01 | C01 | T01 — definir ou selecionar a malha viária. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R02 | Configuração dos parâmetros utilizados nos experimentos. | Definir corretamente as condições da simulação antes da execução. | P01 | C01 | T02 — configurar parâmetros do experimento. | HTA — T02 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R03 | Execução de diferentes estratégias de controle semafórico. | Selecionar claramente qual estratégia será utilizada em cada experimento. | P01 | C01 | T03 — selecionar a estratégia de controle. | GOMS — T03 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R04 | Execução automatizada do ambiente experimental. | Realizar o experimento configurado e compreender seu estado de execução. | P01 | C01 | T04 — iniciar uma simulação; T05 — verificar o estado da execução. | CTT — T04/T05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R05 | Produção de métricas de desempenho das simulações. | Compreender o desempenho obtido em cada experimento. | P01, P02 | C02 | T06 — consultar as métricas obtidas. | GOMS — T06 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R06 | Comparação experimental entre tempo fixo, Max Pressure e Max Pressure + actuated. | Comparar o comportamento das estratégias sob condições equivalentes. | P01, P02 | C02 | T07 — comparar resultados. | HTA — T07; CTT — T07/T08 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R07 | Geração e organização dos resultados experimentais. | Registrar e comunicar os resultados obtidos em uma execução ou comparação. | P01, P02 | C02 | T08 — consultar ou gerar uma síntese dos resultados. | CTT — T07/T08 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |

### Observação sobre a Entrega 5

A tarefa T01 permanece sem um artefato específico de HTA, GOMS ou CTT nesta entrega. Isso não representa ausência da tarefa no projeto: T01 continua como parte do fluxo principal e como pré-requisito para as atividades seguintes.

A Entrega 5 aprofundou especificamente:

- T02 por meio de HTA;
- T03 por meio de GOMS;
- T04/T05 por meio de CTT;
- T06 por meio de GOMS;
- T07 por meio de HTA e também no CTT T07/T08;
- T08 por meio do CTT T07/T08.

Os campos das entregas futuras permanecem como `PENDENTE` enquanto seus respectivos artefatos ainda não existirem.

---

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

Neste momento, ainda não existem telas de Figma definidas. Por isso, os IDs `F01`, `F02` etc. permanecerão reservados para quando os fluxos e telas forem efetivamente modelados.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| PENDENTE | Entrada/seleção da malha | T01 | Definir a malha ou cenário no qual a simulação será realizada. | H02 / discussão inicial do recorte com o professor; Entregas 1 e 4 — definição do cenário permanece como etapa necessária antes da configuração do experimento. | R01 |
| PENDENTE | Configuração/parametrização | T02 e T03 | Definir parâmetros experimentais e selecionar a estratégia de controle. | H02 + Entrega 5: HTA T02 evidenciou necessidade de verificar completude, validade e equivalência da configuração; GOMS T03 evidenciou caminhos e verificações para seleção da estratégia. | R02, R03 |
| PENDENTE | Acompanhamento de processamento | T04 e T05 | Iniciar a simulação e compreender seu estado de execução. | Entrega 1 + Entrega 2: controles de execução e feedback de estado observados no Aimsun Next e no PTV Vissim; Entrega 5: CTT T04/T05 evidenciou validação prévia, feedback de inconsistência, acompanhamento concorrente ao processamento e confirmação do estado final. | R04 |
| PENDENTE | Dashboard/visão de resultados | T06 e T07 | Visualizar métricas e comparar o desempenho dos experimentos. | H03 + Entrega 2: Aimsun Next e PTV Vissim utilizam resumos, listas e visualizações gráficas de resultados; Entrega 5: GOMS T06 e HTA T07 reforçaram a necessidade de relacionar métricas, contexto experimental e comparabilidade. | R05, R06 |
| PENDENTE | Relatório/resultados | T06, T07 e T08 | Consultar, sintetizar e comunicar os resultados obtidos. | H03 + Entrega 2: resultados vinculados às execuções e diferentes formas de visualização observadas no Aimsun Next e no PTV Vissim; Entrega 5: CTT T07/T08 demonstrou que a síntese deve ocorrer depois da interpretação contextualizada das métricas. | R05, R06, R07 |
| PENDENTE | Histórico com busca/filtros | PENDENTE | Recuperar e comparar experimentos anteriores, caso essa necessidade seja confirmada. | PENDENTE — a Entrega 5 mostrou a necessidade de localizar e distinguir execuções, especialmente no GOMS T06, mas ainda não existe evidência suficiente para definir um histórico avançado com busca e filtros como requisito. | PENDENTE |

> Dashboard, histórico, relatório e outros padrões permanecem como possibilidades enquanto suas necessidades não forem confirmadas. A presença nesta tabela não significa que todos serão implementados.

### Decisões de interação derivadas até a Entrega 5

As entregas realizadas até o momento indicam algumas necessidades que deverão ser consideradas nas etapas de prototipação, sem ainda definir telas específicas:

- manter cenário, demanda, parâmetros e estratégia claramente associados à execução;
- validar parâmetros relevantes antes de iniciar a simulação;
- impedir ou sinalizar configurações incompletas ou inconsistentes;
- apresentar feedback sobre início, processamento, erro e conclusão da execução;
- permitir que o usuário reconheça qual estratégia está sendo executada;
- manter os resultados ligados às condições experimentais que os produziram;
- permitir a interpretação conjunta de tempo médio de espera, tamanho médio das filas, throughput e número de trocas de fase;
- verificar a comparabilidade das execuções antes de apresentar uma conclusão comparativa;
- preservar contexto suficiente para justificar uma síntese dos resultados;
- não introduzir recursos administrativos, permissões ou histórico avançado enquanto sua necessidade não estiver suficientemente sustentada.

---

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| — | Nenhuma mudança formal de escopo registrada até o momento. | As Entregas 2–5 aprofundaram usuários, cenários e tarefas sem alterar o recorte principal definido na Entrega 1. | — | — |

> Refinamentos de conhecimento dentro do mesmo recorte não são tratados como mudança de escopo. Caso uma entrega futura altere usuário, objetivo principal, fluxo central ou funcionalidades consideradas essenciais, a mudança deverá ser registrada nesta seção.

---

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
- A existência de uma persona, cenário ou análise de tarefa não transforma automaticamente uma hipótese em fato validado.
- Ao concluir uma nova entrega, atualize somente as colunas e hipóteses para as quais houve nova evidência.
- Preserve `PENDENTE` quando um artefato futuro ainda não tiver sido produzido.

---

## Convenção de identificadores adotada

Para manter a rastreabilidade consistente ao longo do semestre, serão utilizados os seguintes identificadores:

| Prefixo | Artefato |
|---|---|
| H | Hipótese ou lacuna relevante |
| P | Persona |
| C | Cenário |
| T | Tarefa/objetivo do usuário |
| M | Modelo/MoLIC |
| F | Tela ou fluxo do protótipo no Figma |
| UT | Tarefa utilizada em teste com usuário |
| R | Linha de rastreabilidade |

Os identificadores serão criados somente quando o respectivo artefato existir. Até lá, os campos permanecerão como `PENDENTE`.
