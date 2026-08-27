# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated em ambiente de simulação. | TCC1 — título, introdução e metodologia. | definido |
| Resultado técnico esperado | Algoritmo híbrido de controle semafórico acompanhado de avaliação experimental em ambiente de simulação. | TCC1 — objetivos e metodologia. | definido |
| O TCC previa interface? | parcialmente | A equipe já considerava o desenvolvimento de uma interface antes da disciplina de IHC, porém ela ainda não está formalmente detalhada no documento atual do TCC1. | definido |
| Capacidade/contribuição central | Selecionar dinamicamente os movimentos semafóricos prioritários e controlar a permanência ou troca do verde de acordo com o estado observado do tráfego. | TCC1 — proposta do algoritmo Max Pressure + lógica actuated. | definido |
| Possíveis beneficiários/stakeholders | Pesquisadores de mobilidade, analistas/engenheiros de tráfego, gestores de mobilidade, órgãos responsáveis pelo trânsito e, indiretamente, usuários das vias. | Entrega 1 — Seção 2. Os perfis profissionais ainda precisam ser investigados. | H |
| Usuário escolhido para IHC | Pesquisador ou analista de mobilidade urbana. | H01 — perfil possui relação plausível com configuração, execução e análise de experimentos de controle semafórico. | H |
| Objetivo principal do usuário | Avaliar diferentes estratégias de controle semafórico por meio da configuração, execução e comparação de experimentos em diferentes cenários de tráfego. | Entrega 1 — Seções 3 e 7. | H |
| Contexto de uso adotado | Ambiente computacional acadêmico, laboratorial ou profissional voltado à experimentação e análise de estratégias de controle de tráfego. | Entrega 1 — Seção 5. | H |
| Interface/recorte de IHC | Fluxo inicial composto por definição da malha viária, configuração e execução da simulação e análise/comparação dos resultados. | Deriva das atividades identificadas na Entrega 1 e da discussão inicial realizada com o professor. | proposta |
| Relação com o TCC | parte prevista | A equipe já possuía intenção de desenvolver uma interface antes da disciplina, mas seu usuário, fluxo e requisitos de interação ainda não estavam formalmente definidos. A disciplina aprofunda essa proposta. | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

---

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | H | O perfil escolhido influencia tarefas, linguagem, contexto, personas e decisões de interação. | Entregas 2, 3 e 7 | PENDENTE | aberta | Pode confirmar ou exigir revisão do usuário prioritário e dos artefatos derivados desse perfil. |
| H02 | Organizar a interação em definição da malha, configuração/execução e análise dos resultados facilita a realização dos experimentos em relação à interação direta com as ferramentas técnicas. | H | Esse fluxo constitui a estrutura inicial do projeto de interface e precisa ser validado. | Entregas 3, 5, 6 e 7 | PENDENTE | aberta | Pode confirmar, reorganizar, simplificar ou ampliar o fluxo principal da interface. |
| H03 | Uma apresentação comparativa das métricas por meio de dashboard ou relatório facilita a interpretação do desempenho dos métodos. | H | A forma de apresentação influencia a compreensão e comparação dos resultados produzidos pelos experimentos. | Entregas 2, 6, 7 e 12–14 | PENDENTE | aberta | Pode determinar quais informações, visualizações e formas de comparação serão utilizadas no protótipo. |

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Utilização de diferentes malhas e cenários no ambiente experimental. | Definir corretamente onde e em quais condições o experimento será realizado. | PENDENTE | PENDENTE | T01 — definir ou selecionar a malha viária. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R02 | Configuração dos parâmetros utilizados nos experimentos. | Definir corretamente as condições da simulação antes da execução. | PENDENTE | PENDENTE | T02 — configurar parâmetros do experimento. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R03 | Execução de diferentes estratégias de controle semafórico. | Selecionar claramente qual estratégia será utilizada em cada experimento. | PENDENTE | PENDENTE | T03 — selecionar a estratégia de controle. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R04 | Execução automatizada do ambiente experimental. | Realizar o experimento configurado e compreender seu estado de execução. | PENDENTE | PENDENTE | T04 — iniciar uma simulação; T05 — verificar o estado da execução. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R05 | Produção de métricas de desempenho das simulações. | Compreender o desempenho obtido em cada experimento. | PENDENTE | PENDENTE | T06 — consultar as métricas obtidas. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R06 | Comparação experimental entre tempo fixo, Max Pressure e Max Pressure + actuated. | Comparar o comportamento das estratégias sob condições equivalentes. | PENDENTE | PENDENTE | T07 — comparar resultados. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R07 | Geração e organização dos resultados experimentais. | Registrar e comunicar os resultados obtidos em uma execução ou comparação. | PENDENTE | PENDENTE | T08 — consultar ou gerar uma síntese dos resultados. | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |

---

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

Neste momento, ainda não existem telas de Figma definidas. Por isso, os IDs `F01`, `F02` etc. permanecerão reservados para quando os fluxos e telas forem efetivamente modelados.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| PENDENTE | Entrada/seleção da malha | T01 | Definir a malha ou cenário no qual a simulação será realizada. | H02 / discussão inicial do recorte com o professor | R01 |
| PENDENTE | Configuração/parametrização | T02 e T03 | Definir parâmetros experimentais e selecionar a estratégia de controle. | H02 / metodologia experimental do TCC | R02, R03 |
| PENDENTE | Acompanhamento de processamento | T04 e T05 | Iniciar a simulação e compreender seu estado de execução. | Hipótese inicial da Entrega 1 | R04 |
| PENDENTE | Dashboard/visão de resultados | T06 e T07 | Visualizar métricas e comparar o desempenho dos experimentos. | H03 | R05, R06 |
| PENDENTE | Relatório/resultados | T06, T07 e T08 | Consultar, sintetizar e comunicar os resultados obtidos. | H03 | R05, R06, R07 |
| PENDENTE | Histórico com busca/filtros | PENDENTE | Recuperar e comparar experimentos anteriores, caso essa necessidade seja confirmada. | PENDENTE — necessidade ainda não validada | PENDENTE |

> Dashboard, histórico, relatório e outros padrões permanecem como possibilidades enquanto suas necessidades não forem confirmadas. A presença nesta tabela não significa que todos serão implementados.

---

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| — | Nenhuma mudança de escopo registrada até o momento. | — | — | — |

---

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.

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
