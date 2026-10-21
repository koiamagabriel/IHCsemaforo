# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

No projeto desta equipe, a interface já fazia parte da intenção de desenvolvimento do TCC e, na Entrega 6, foi formalmente tratada como **protótipo digital V0** para fins de análise formativa de IHC.

As evidências visuais e o walkthrough da Entrega 6 permitiram refinar a descrição da V0, identificar possíveis rupturas de interação e propor decisões de evolução para uma V1 conceitual.

A análise também permitiu corrigir uma descrição anterior importante: a interface possui catálogo, configuração, validação, execução, histórico e análise individual de resultados, mas **não realiza comparação automática entre duas execuções**. Essa comparação é atualmente feita manualmente fora da aplicação a partir dos resultados consultados individualmente.

Na Entrega 7, as principais hipóteses ainda abertas foram transformadas em um **plano de investigação reproduzível**, composto por questionário e entrevista semiestruturada. Como esses instrumentos não foram aplicados, as hipóteses H01, H02 e H03 permanecem abertas.

---

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated em ambiente de simulação. | TCC1 — título, introdução e metodologia. | definido |
| Resultado técnico esperado | Algoritmo híbrido de controle semafórico acompanhado de avaliação experimental em ambiente de simulação. | TCC1 — objetivos e metodologia. | definido |
| O TCC previa interface? | sim, parcialmente definida | A equipe já considerava o desenvolvimento de uma interface antes da disciplina de IHC. Na Entrega 6, essa intenção passou a ser representada pelo protótipo digital funcional V0. | definido |
| Capacidade/contribuição central | Selecionar dinamicamente os movimentos semafóricos prioritários e controlar a permanência ou troca do verde de acordo com o estado observado do tráfego. | TCC1 — proposta do algoritmo Max Pressure + lógica actuated. | definido |
| Possíveis beneficiários/stakeholders | Pesquisadores de mobilidade, analistas/engenheiros de tráfego, gestores de mobilidade, órgãos responsáveis pelo trânsito e, indiretamente, usuários das vias. | Entrega 1. A Entrega 7 definiu instrumentos capazes de investigar esses perfis. | H |
| Usuário escolhido para IHC | Pesquisador ou analista de mobilidade urbana. | H01 — perfil possui relação plausível com configuração, execução e análise de experimentos. | H |
| Objetivo principal do usuário | Avaliar diferentes estratégias de controle semafórico por meio da configuração, execução, análise e comparação de experimentos. | Entregas 1, 3, 4 e 5; V0 e walkthrough da Entrega 6. | H |
| Contexto de uso adotado | Ambiente computacional acadêmico, laboratorial ou profissional voltado à experimentação e análise. | Entregas 1, 3 e 6. | H |
| Interface/recorte de IHC | Seleção de cenário, configuração, validação, execução/acompanhamento, recuperação e análise individual dos resultados, com comparação manual externa quando necessária. | Entregas 1–6 e evidências visuais da V0. | proposta materializada em V0 |
| Relação com o TCC | parte prevista | A interface já era planejada no TCC e passou a ser analisada e refinada a partir dos métodos de IHC. | definido |

---

# 2. Registro de hipóteses e lacunas

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência acumulada | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | H | O perfil influencia tarefas, linguagem, contexto e decisões de interação. | Entregas 2, 3 e 7; avaliações posteriores | Entrega 2 analisou ferramentas profissionais. Entrega 3 estruturou P01/P02. Entrega 6 aplicou essas personas ao protótipo e identificou questões de linguagem técnica. Entrega 7 planejou I01/Q01–Q04 e I02/E01–E02. | aberta | Personas, linguagem e nível de detalhamento continuam sujeitos a refinamento. |
| H02 | Organizar a interação em definição da malha, configuração/execução e análise dos resultados facilita a realização dos experimentos. | H | Esse fluxo constitui a estrutura inicial da interface. | Entregas 3–7; avaliações posteriores | Entregas 3–5 detalharam jornada e tarefas. Entrega 6 materializou PF01–PF03. O walkthrough mostrou compreensão geral do fluxo, mas apontou densidade técnica, necessidade de melhor recuperação de erro e maior clareza do estado de execução. | aberta | Estrutura geral foi preservada, com propostas de refinamento V1. |
| H03 | Uma apresentação consolidada e comparativa das métricas facilita a interpretação do desempenho dos métodos. | H | A forma de apresentar resultados influencia análise e decisão. | Entregas 2–7; Entregas 12–14 | Entrega 6 mostrou que a V0 oferece histórico, resultado individual e gráfico, mas não comparação automática. O walkthrough identificou trabalho adicional para alternar entre execuções e comparar externamente. Entrega 7 planejou investigar métricas, comparação, histórico e síntese. | aberta | Apoio à comparação permanece oportunidade de evolução, ainda não requisito definitivamente validado. |

### Situação atual

H01, H02 e H03 permanecem abertas.

A Entrega 6 gerou evidências sobre **a organização e o funcionamento do protótipo V0** e decisões de revisão.

A Entrega 7 forneceu instrumentos adicionais para investigação, mas eles ainda não foram aplicados.

---

# 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário | Objetivo/tarefa | HTA/GOMS/CTT | Protótipo E6 | Coleta E7 | Cenário de interação / signos | MoLIC | Figma | Heurística | Teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Diferentes malhas/cenários. | Definir onde o experimento será realizado. | P01 | C01 | T01 | PENDENTE | PF01 / PP01 | I01 Q05; I02 E03/E04 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O01 — manter separação entre cenário e configuração. |
| R02 | Configuração de parâmetros. | Definir condições antes da execução. | P01 | C01 | T02 | HTA T02 | PF01 / PP02 / PP03 | I01 Q05–Q07; I02 E03–E05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O02–O05 — ajuda contextual, parâmetros avançados separados e melhor recuperação de erro. |
| R03 | Estratégias de controle. | Selecionar claramente a estratégia. | P01 | C01 | T03 | GOMS T03 | PF01 / PP02 | I01 Q05/Q06; I02 E04/E05 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O02 — explicar termos técnicos sem retirar precisão. |
| R04 | Execução automatizada. | Iniciar e reconhecer o estado da execução. | P01 | C01 | T04/T05 | CTT T04/T05 | PF02 / PP03 / PP04 / PP05 | I01 Q08/Q09; I02 E06–E08 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O04–O07 — preservar validação e modo Visual; destacar estado principal dos logs. |
| R05 | Métricas experimentais. | Consultar uma execução e interpretar seus resultados. | P01, P02 | C02 | T06 | GOMS T06 | PF03 / PP06 / PP07 | I01 Q10/Q11; I02 E09/E10/E13 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O08–O09 — preservar contexto da execução e hierarquizar resultados. |
| R06 | Comparação entre estratégias. | Comparar execuções sob condições equivalentes. | P01, P02 | C02 | T07 | HTA T07; CTT T07/T08 | PF03 / PP06 / PP07 + comparação manual externa | I01 Q12/Q13; I02 E11–E13 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O10 — investigar futuramente apoio à comparação lado a lado. |
| R07 | Organização dos resultados. | Produzir uma síntese da análise. | P01, P02 | C02 | T08 | CTT T07/T08 | PF03 / PP07 + síntese externa | I01 Q10–Q17; I02 E14–E20 | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | E6/O09–O10 — melhorar hierarquia e reduzir esforço para síntese comparativa. |

---

# 4. Observação sobre a Entrega 5

A tarefa T01 permanece sem um artefato específico de HTA, GOMS ou CTT na Entrega 5.

A Entrega 5 aprofundou:

- T02 por HTA;
- T03 por GOMS;
- T04/T05 por CTT;
- T06 por GOMS;
- T07 por HTA e pelo CTT T07/T08;
- T08 pelo CTT T07/T08.

---

# 5. Observação sobre a Entrega 6

A Entrega 6 foi concluída com o protótipo digital V0 organizado em três fluxos:

- **PF01 — Preparar experimento:** T01, T02 e T03;
- **PF02 — Validar, executar e acompanhar:** T04 e T05;
- **PF03 — Localizar e analisar resultados:** T06, T07 e T08.

Os estados documentados são:

- **PP01:** catálogo e seleção do cenário;
- **PP02:** configuração principal, modo de execução e configuração avançada;
- **PP03:** validação e confirmação pré-execução;
- **PP04:** inicialização e feedback da execução;
- **PP05:** execução Visual no SUMO-GUI;
- **PP06:** histórico/listagem e seleção de uma execução;
- **PP07:** análise individual dos resultados e gráfico/diagnóstico.

A comparação prevista em T07 **não é uma função automática da V0**.

A interface apoia T07 ao permitir recuperar execuções individualmente e consultar suas informações. A comparação é realizada manualmente fora da aplicação.

A Entrega 6 possui doze evidências visuais armazenadas em:

```text
assets/06_prototipos/
