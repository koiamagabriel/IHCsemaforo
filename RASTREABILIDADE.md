# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da contribuição técnica do TCC para um cenário de uso plausível e desse cenário para as decisões de interação.

No projeto desta equipe, a interface já fazia parte da intenção de desenvolvimento do TCC e, na Entrega 6, foi formalmente tratada como **protótipo digital V0** para fins de análise formativa de IHC.

As evidências visuais da Entrega 6 permitiram refinar a descrição da V0: a interface possui catálogo, configuração, validação, execução, histórico e análise individual de resultados, mas **não realiza comparação automática entre duas execuções**. Essa comparação é feita manualmente fora da aplicação a partir dos resultados recuperados individualmente.

Na Entrega 7, as principais hipóteses ainda abertas foram transformadas em um **plano de investigação reproduzível**, composto por um questionário e uma entrevista semiestruturada. Como esses instrumentos não foram aplicados nesta etapa, sua elaboração não é tratada como evidência empírica e as hipóteses permanecem abertas.

---

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated em ambiente de simulação. | TCC1 — título, introdução e metodologia. | definido |
| Resultado técnico esperado | Algoritmo híbrido de controle semafórico acompanhado de avaliação experimental em ambiente de simulação. | TCC1 — objetivos e metodologia. | definido |
| O TCC previa interface? | sim, parcialmente definida | A equipe já considerava o desenvolvimento de uma interface antes da disciplina de IHC. Na Entrega 6, essa intenção passou a ser representada por um protótipo digital funcional pré-existente do TCC, denominado V0 para fins da disciplina. | definido |
| Capacidade/contribuição central | Selecionar dinamicamente os movimentos semafóricos prioritários e controlar a permanência ou troca do verde de acordo com o estado observado do tráfego. | TCC1 — proposta do algoritmo Max Pressure + lógica actuated. | definido |
| Possíveis beneficiários/stakeholders | Pesquisadores de mobilidade, analistas/engenheiros de tráfego, gestores de mobilidade, órgãos responsáveis pelo trânsito e, indiretamente, usuários das vias. | Entrega 1. A Entrega 7 definiu instrumentos capazes de investigar esses perfis, mas ainda não houve coleta empírica. | H |
| Usuário escolhido para IHC | Pesquisador ou analista de mobilidade urbana. | H01 — perfil possui relação plausível com configuração, execução e análise de experimentos de controle semafórico. | H |
| Objetivo principal do usuário | Avaliar diferentes estratégias de controle semafórico por meio da configuração, execução e comparação de experimentos. | Entregas 1, 3, 4 e 5; Entrega 6 materializa parte desse fluxo. | H |
| Contexto de uso adotado | Ambiente computacional acadêmico, laboratorial ou profissional voltado à experimentação e análise. | Entregas 1, 3 e 6. | H |
| Interface/recorte de IHC | Seleção de cenário, configuração, validação, execução/acompanhamento, recuperação e análise individual dos resultados, com comparação manual externa quando necessária. | Entregas 1–6 e evidências visuais da V0. | proposta materializada em V0 |
| Relação com o TCC | parte prevista | A equipe já possuía intenção de desenvolver uma interface antes da disciplina. A Entrega 6 aproveitou o protótipo funcional existente e o reinterpretou a partir dos métodos de IHC. | definido |

---

## 2. Registro de hipóteses e lacunas da Entrega 1

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida / instrumento planejado | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | H | O perfil influencia tarefas, linguagem, contexto e decisões de interação. | Entregas 2, 3 e 7; avaliações posteriores | Entrega 2 analisou ferramentas profissionais; Entrega 3 estruturou P01/P02; Entrega 6 relacionou a V0 a essas tarefas; Entrega 7 planejou I01/Q01–Q04 e I02/E01–E02. | aberta | Personas e vocabulário permanecem sujeitos a refinamento. |
| H02 | Organizar a interação em definição da malha, configuração/execução e análise dos resultados facilita os experimentos. | H | Esse fluxo constitui a estrutura inicial do projeto de interface. | Entregas 3–7; avaliações posteriores | Entregas 3–5 detalharam jornada e tarefas. Entrega 6 materializou PF01, PF02 e PF03 e documentou evidências visuais. Entrega 7 planejou investigar preparação, parâmetros, feedback e erros. | aberta | A V0 demonstra o fluxo, mas ainda não valida sua adequação a usuários. |
| H03 | Uma apresentação consolidada e comparativa das métricas facilita a interpretação do desempenho dos métodos. | H | A forma de apresentar resultados influencia análise e decisão. | Entregas 2–7; Entregas 12–14 | Entrega 6 mostrou que a V0 oferece análise individual e gráfico, mas não comparação automática. Entrega 7 planejou investigar métricas, comparação, histórico e síntese. | aberta | H03 deve considerar que a comparação hoje é manual e externa à V0. |

### Situação atual

H01, H02 e H03 permanecem abertas.

As capturas da Entrega 6 constituem evidência sobre **o funcionamento da V0**, não sobre a adequação da interface aos usuários.

A Entrega 7 tornou as hipóteses investigáveis, mas seus instrumentos não foram aplicados.

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário | Objetivo/tarefa | HTA/GOMS/CTT | Protótipo E6 | Coleta E7 | Cenário de interação / signos | MoLIC | Figma | Heurística | Teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Diferentes malhas/cenários. | Definir onde o experimento será realizado. | P01 | C01 | T01 | PENDENTE | PF01 / PP01 | I01 Q05; I02 E03/E04 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R02 | Configuração de parâmetros. | Definir condições antes da execução. | P01 | C01 | T02 | HTA T02 | PF01 / PP02 / PP03 | I01 Q05–Q07; I02 E03–E05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R03 | Estratégias de controle. | Selecionar claramente a estratégia. | P01 | C01 | T03 | GOMS T03 | PF01 / PP02 | I01 Q05/Q06; I02 E04/E05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R04 | Execução automatizada. | Iniciar e reconhecer o estado da execução. | P01 | C01 | T04/T05 | CTT T04/T05 | PF02 / PP03 / PP04 / PP05 | I01 Q08/Q09; I02 E06–E08 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R05 | Métricas experimentais. | Consultar uma execução e interpretar seus resultados. | P01, P02 | C02 | T06 | GOMS T06 | PF03 / PP06 / PP07 | I01 Q10/Q11; I02 E09/E10/E13 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R06 | Comparação entre estratégias. | Comparar execuções sob condições equivalentes. | P01, P02 | C02 | T07 | HTA T07; CTT T07/T08 | PF03 / PP06 / PP07 + comparação manual externa | I01 Q12/Q13; I02 E11–E13 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R07 | Organização dos resultados. | Produzir uma síntese da análise. | P01, P02 | C02 | T08 | CTT T07/T08 | PF03 / PP07 + síntese externa | I01 Q10–Q17; I02 E14–E20 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |

---

## 4. Observação sobre a Entrega 5

A tarefa T01 permanece sem um artefato específico de HTA, GOMS ou CTT na Entrega 5. Isso não representa ausência da tarefa no projeto.

A Entrega 5 aprofundou:

- T02 por HTA;
- T03 por GOMS;
- T04/T05 por CTT;
- T06 por GOMS;
- T07 por HTA e pelo CTT T07/T08;
- T08 pelo CTT T07/T08.

---

## 5. Observação sobre a Entrega 6

A Entrega 6 organiza a V0 em três fluxos:

- **PF01 — Preparar experimento:** T01, T02 e T03;
- **PF02 — Validar, executar e acompanhar:** T04 e T05;
- **PF03 — Localizar e analisar resultados:** T06, T07 e T08.

Estados documentados:

- **PP01:** catálogo e seleção do cenário;
- **PP02:** configuração da simulação, modo de execução e configuração avançada;
- **PP03:** validação e confirmação pré-execução;
- **PP04:** inicialização e feedback da execução;
- **PP05:** execução Visual no SUMO-GUI;
- **PP06:** histórico/listagem e seleção de uma execução;
- **PP07:** análise individual dos resultados e gráfico/diagnóstico.

A comparação prevista em T07 **não é uma função automática da V0**.

A interface apoia T07 ao permitir recuperar duas execuções individualmente e consultar suas informações. A comparação é realizada manualmente fora da aplicação.

As evidências visuais estão documentadas em `assets/06_prototipos/`.

O walkthrough com participante ainda precisa ser documentado antes de a Entrega 6 ser marcada como completamente concluída.

---

## 6. Observação sobre a Entrega 7

A Entrega 7 produziu dois instrumentos completos e complementares:

- **I01 — Questionário exploratório**, de Gabriel Koiama de Rocha Lira;
- **I02 — Entrevista semiestruturada**, de João Pedro Lopes Santana Villas Bôas.

Os instrumentos estão prontos para eventual aplicação, mas não foram executados.

Consequentemente, H01, H02 e H03 permanecem abertas.

---

## 7. Rastreabilidade de padrões de interface

| Estado/fluxo | Padrão | Objetivo/tarefa | Informação/ação principal | Situação |
|---|---|---|---|---|
| PF01 / PP01 | Seleção de cenário | T01 | Escolher infraestrutura/cenário. | Implementado na V0. |
| PF01 / PP02 | Configuração | T02/T03 | Definir parâmetros, controlador e modo de execução. | Implementado na V0. |
| PF02 / PP03 | Validação/confirmação | T02/T04 | Bloquear condições inadequadas e confirmar execução. | Implementado na V0. |
| PF02 / PP04/PP05 | Acompanhamento | T04/T05 | Informar inicialização e permitir inspeção Visual. | Implementado na V0. |
| PF03 / PP06 | Histórico/listagem | T06/T07 | Localizar e selecionar execução anterior. | Implementado na V0. |
| PF03 / PP07 | Resultado individual | T06/T08 | Consultar informações e gráfico da execução. | Implementado na V0. |
| Externo à V0 | Comparação | T07/T08 | Comparar resultados de execuções consultadas individualmente. | Manual/externo. |
| PENDENTE | Administração | PENDENTE | Não há tarefa que justifique. | Não adotado. |

---

## 8. Decisões de interação até a Entrega 7

As entregas realizadas sustentam, como decisões ou hipóteses a serem avaliadas:

- manter cenário, parâmetros, controlador e seed associados à execução;
- permitir seleção explícita de cenário;
- agrupar configuração principal e avançada;
- validar condições antes da execução;
- confirmar a execução aceita;
- diferenciar modo Visual e Headless;
- fornecer feedback sobre inicialização/processamento;
- permitir recuperar execuções anteriores;
- manter os resultados ligados ao contexto que os produziu;
- permitir análise individual das métricas e gráficos;
- reconhecer explicitamente que a comparação entre execuções ainda é manual;
- não representar como interna uma funcionalidade que ocorre fora da aplicação;
- não introduzir administração ou CRUDs sem necessidade rastreável.

---

## 9. Questões formalizadas pela Entrega 7

A Entrega 7 não adicionou novas conclusões sobre usuários. Ela formalizou perguntas que poderão orientar revisões futuras:

- qual perfil realmente realiza atividades semelhantes às assumidas para P01 e P02;
- quais ferramentas e termos são familiares;
- quais parâmetros precisam estar visíveis;
- quais configurações devem ser verificadas antes da execução;
- quais erros são mais críticos;
- que feedback é necessário durante processamento;
- quais métricas são consultadas primeiro;
- como diferentes resultados são comparados;
- quais condições definem comparabilidade;
- se histórico, busca ou filtros são necessários;
- qual equilíbrio entre síntese e detalhamento é mais apropriado;
- como resultados são comunicados.

---

## 10. Registro de mudanças/refinamentos

| Data | O que mudou | Evidência/feedback | Artefatos afetados |
|---|---|---|---|
| 20/10/2026 | Protótipo digital pré-existente foi adotado como V0. | Orientação docente e existência da GUI funcional. | Entrega 6, rastreabilidade. |
| 21/10/2026 | A descrição de resultados/comparação foi corrigida: PP06 passou a representar histórico/seleção; PP07, análise individual; comparação passou a ser registrada como manual e externa. | Capturas reais da V0 e revisão do comportamento efetivo da interface. | Entrega 6, R05–R07, padrões de interface, README. |

Esse refinamento **não altera o escopo do usuário ou das tarefas**. Ele corrige a representação da implementação atual.

---

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `PF01`, `PP01`, `I01`, `M01`, `F01`, `UT01`).
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Diferencie funcionalidade implementada de atividade externa/manual.
- Não trate instrumento planejado como dado coletado.
- Não trate protótipo funcional como interface validada.
- Preserve histórico de mudanças quando evidências posteriores corrigirem a documentação.

---

## Convenção de identificadores adotada

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
