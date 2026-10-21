# Projeto de Interação Humano-Computador (IHC) - Equipe 24

## Princípio do projeto da disciplina

A disciplina utiliza **preferencialmente o tema do TCC em andamento** como domínio para exercitar os métodos de Interação Humano-Computador.

Isso vale também quando o TCC é predominantemente técnico e **não previa o desenvolvimento de uma interface**.

- Se o TCC **já prevê interface**, ela pode ser o objeto principal das atividades de IHC.
- Se o TCC **não prevê interface**, a equipe deverá derivar um **escopo de IHC** a partir da contribuição técnica: quem poderia utilizar ou se beneficiar do resultado, o que essa pessoa precisaria fazer, em qual contexto e que interação seria necessária.
- A interface criada na disciplina **não se torna automaticamente uma obrigação do TCC**. Ela pode ser um protótipo de aprendizagem, uma extensão conceitual ou uma demonstração de aplicação potencial. Sua incorporação ao TCC depende de decisão da equipe e do orientador.

Leia obrigatoriamente o [Guia para definir o escopo de IHC a partir do tema do TCC](GUIA_ESCOPO_IHC.md).

## Identificação

**Título do projeto de IHC:** Interface para Configuração, Execução e Análise de Simulações de Controle Semafórico Inteligente  
**TCC/projeto de origem:** Algoritmo Híbrido de Controle Semafórico Baseado em Max Pressure e Lógica Actuated em Ambiente de Simulação  
**Orientador(a):** Ricardo de Carvalho Destro  
**Disciplina:** Interação Humano-Computador  
**Instituição:** Centro Universitário FEI  
**Semestre:** 2026/2

### Equipe

| Nome completo | Matrícula | GitHub | Responsabilidade principal |
|---|---:|---|---|
| Gabriel Koiama de Rocha Lira | 22.125.067-3 | @koiamagabriel | Desenvolvimento do projeto de IHC |
| João Pedro Lopes Santana Villas Bôas | 22.125.065-7 | @JPLopes05 | Desenvolvimento do projeto de IHC |

## Relação entre TCC e projeto de IHC

| Item | Descrição |
|---|---|
| Tema central do TCC | Desenvolvimento de um algoritmo híbrido de controle semafórico inteligente baseado em Max Pressure e lógica actuated. |
| Resultado técnico esperado do TCC | Sistema de controle semafórico inteligente implementado em Python e integrado ao SUMO por meio do TraCI, acompanhado de uma interface que permita configurar, executar, acompanhar e analisar as simulações. Os resultados das diferentes estratégias podem ser consultados individualmente e comparados manualmente pela equipe. |
| O TCC já previa interface? | Sim — a interface já era prevista pela equipe e atualmente existe como protótipo digital funcional do TCC. Nas etapas iniciais do TCC ela ainda não estava formalmente detalhada no documento do TCC1. |
| Capacidade técnica que pode gerar valor para pessoas | Permitir a configuração de cenários e parâmetros de simulação, a execução e o acompanhamento visual dos experimentos e a análise dos resultados produzidos pelas diferentes estratégias de controle semafórico. |
| Usuário principal adotado em IHC | Pesquisador ou analista de mobilidade urbana. |
| Objetivo principal desse usuário | Configurar uma simulação de tráfego, executá-la e acompanhar seu funcionamento, além de analisar os resultados e comparar diferentes estratégias sob condições adequadas. |
| Interface/recorte explorado na disciplina | Interface para seleção do cenário, configuração do experimento, validação, execução e acompanhamento da simulação, recuperação de execuções anteriores e análise individual dos resultados obtidos. |
| Relação com o escopo formal do TCC | A interface faz parte do escopo previsto do TCC. Na Entrega 6, o protótipo digital existente foi adotado como V0, documentado por evidências visuais e submetido a walkthrough formativo, gerando observações e decisões de evolução para uma V1 conceitual. |

> **Importante:** a tabela acima explica a relação entre os dois trabalhos. Ela não altera o compromisso formal do TCC.

## Resumo do projeto pela perspectiva do usuário

Um **pesquisador ou analista de mobilidade urbana** precisa configurar, executar, acompanhar e analisar simulações de controle semafórico. Para isso, é necessário definir o cenário de simulação, configurar seus parâmetros, escolher o método de controle, acompanhar a execução do experimento e interpretar os resultados obtidos.

O TCC investiga um algoritmo híbrido baseado em Max Pressure e lógica actuated.

Para a disciplina de IHC, é explorada a interface que permite ao usuário:

**selecionar o cenário → configurar a simulação e a estratégia → validar e confirmar as condições → executar e acompanhar o experimento → localizar uma execução → analisar seus resultados → comparar manualmente diferentes execuções quando necessário**.

Na Entrega 6, a interface funcional já existente no contexto do TCC passou a ser formalizada como **protótipo digital V0**, organizado em três fluxos:

- **PF01 — Preparar experimento**;
- **PF02 — Validar, executar e acompanhar**;
- **PF03 — Localizar e analisar resultados**.

Os estados documentados da V0 são:

- **PP01 — Catálogo e seleção do cenário**;
- **PP02 — Configuração da simulação**;
- **PP03 — Validação e confirmação pré-execução**;
- **PP04 — Inicialização e feedback da execução**;
- **PP05 — Execução no modo Visual**;
- **PP06 — Histórico e seleção de execução**;
- **PP07 — Análise individual dos resultados**.

A Entrega 6 possui **12 evidências visuais** da interface, armazenadas em `assets/06_prototipos/`.

O walkthrough formativo percorreu as tarefas W01–W04 e produziu as observações O01–O10. A análise permitiu identificar aspectos positivos, possíveis dificuldades e decisões de evolução para uma **V1 conceitual**.

Entre as principais decisões estão:

- preservar a separação entre cenário e configuração;
- manter configurações avançadas separadas do fluxo principal;
- preservar os mecanismos de validação e confirmação;
- melhorar mensagens de recuperação de erro;
- destacar o estado principal da execução em relação aos logs técnicos;
- preservar o vínculo entre execução e resultados;
- melhorar a hierarquia das informações apresentadas;
- reconhecer que a comparação entre execuções é atualmente manual e externa à interface;
- investigar futuramente apoio mais direto à comparação.

A comparação prevista em T07 não é uma função automática da V0. Atualmente, o usuário consulta cada execução individualmente e realiza a comparação manualmente fora da aplicação.

Na Entrega 7, as principais hipóteses do projeto foram transformadas em perguntas de investigação e instrumentos reproduzíveis:

- **I01 — Questionário exploratório sobre atividades de simulação e análise**, elaborado por Gabriel;
- **I02 — Entrevista semiestruturada sobre processos técnicos e interpretação de resultados**, elaborada por João.

Os instrumentos foram planejados para eventual aplicação. Como não houve aplicação nesta etapa, H01, H02 e H03 continuam explicitamente abertas.

Se alguma afirmação ainda não estiver sustentada por evidência suficiente, registre-a como hipótese na [Entrega 1](docs/01_conhecendo_o_problema.md) e acompanhe seu estado na [Matriz de rastreabilidade](RASTREABILIDADE.md).

## Por que pensar em interface mesmo em TCCs técnicos?

Algoritmos, modelos, APIs, análises de datasets e componentes de infraestrutura podem não exigir interface como resultado acadêmico do TCC. Porém, quando essas contribuições são transferidas para uma situação real, normalmente existem pessoas que:

- configuram parâmetros;
- fornecem ou selecionam dados;
- iniciam ou acompanham processamento;
- interpretam resultados;
- comparam alternativas;
- tomam decisões;
- administram usuários e permissões;
- consultam histórico;
- geram relatórios;
- investigam erros;
- auditam mudanças.

Essas atividades fornecem um campo legítimo para exercitar IHC.

Possibilidades de interface incluem **dashboards, telas administrativas, configuração, relatórios, histórico com filtros, comparação de resultados, visualização de dados, acompanhamento de processamento, gestão de perfis e permissões, CRUDs justificados pelo domínio, alertas, auditoria e ajuda contextual**.

Nenhuma dessas telas é obrigatória por si só: deve existir uma tarefa e um objetivo de usuário que a justifique.

No projeto atual, a Entrega 6 mostrou quais dessas atividades já são apoiadas pela V0 e também identificou limitações e oportunidades de evolução.

A Entrega 7 reforça esse princípio ao investigar necessidades sem presumir antecipadamente que dashboard, filtros, relatórios, comparação automática ou outras possibilidades devam necessariamente compor a solução definitiva.

## Relação com apresentação e potencial de aplicação

A reflexão sobre usuários ajuda a equipe a explicar o projeto para públicos externos, inclusive em eventos como a **INOVA**.

Em vez de comunicar apenas a técnica implementada, a equipe pode apresentar:

**problema humano → contribuição computacional → forma de uso → impacto potencial**.

No projeto, a interface permite ao usuário interagir com o ambiente de simulação desenvolvido no TCC:

**configuração do cenário e da simulação → validação → execução e acompanhamento → recuperação e análise dos resultados → comparação manual quando necessária**.

A interface faz parte da solução prevista no TCC e atualmente existe como protótipo digital funcional.

Na Entrega 6, seu funcionamento foi formalizado em PF01–PF03 e PP01–PP07. O walkthrough formativo gerou as observações O01–O10 e decisões de evolução V0→V1.

Na Entrega 7, foram produzidos instrumentos para investigar de forma estruturada as premissas relacionadas aos usuários, às atividades, à linguagem, à execução e à interpretação dos resultados.

O fato de o protótipo funcionar tecnicamente não significa, por si só, que todas as decisões de interação estejam definitivamente validadas. Da mesma forma, a existência de questionários, entrevistas, personas ou modelos não transforma automaticamente hipóteses sobre usuários em fatos.

As entregas da disciplina fornecem evidências progressivas sobre necessidades, tarefas, organização da interação e usabilidade.

## Situação das principais hipóteses

| ID | Hipótese | Situação atual |
|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário. | Aberta. A Entrega 6 identificou questões relacionadas à linguagem e ao nível técnico da interface, e a Entrega 7 criou instrumentos para investigar o perfil de usuário. |
| H02 | A organização cenário → configuração → execução/acompanhamento → análise facilita a realização dos experimentos. | Aberta. O fluxo foi materializado e analisado na V0. O walkthrough preservou a estrutura geral, mas gerou propostas de refinamento. A Entrega 7 possui investigação planejada sobre preparação, configuração, erros e feedback. |
| H03 | Uma apresentação consolidada e comparativa das métricas facilita sua interpretação. | Aberta. A V0 apresenta histórico, análise individual e gráfico, enquanto a comparação permanece manual e externa. A Entrega 7 investiga métricas, comparação, histórico e síntese. |

## Como usar este repositório

1. Leia o [Guia de uso e apresentação](GUIA_DE_USO.md).
2. Leia o [Guia de definição de escopo de IHC](GUIA_ESCOPO_IHC.md), especialmente se o TCC não previa interface.
3. Preencha as entregas na ordem em que forem trabalhadas na disciplina.
4. Em toda entrega individual, **identifique o autor**.
5. Salve imagens, diagramas e evidências em [`assets/`](assets/README.md).
6. Mantenha a [Matriz de rastreabilidade](RASTREABILIDADE.md) atualizada.
7. Na Entrega 1, diferencie **[F] fatos**, **[H] hipóteses** e **[?] lacunas de conhecimento**.
8. Antes de cada entrega, revise o checklist do arquivo e o [Checklist final](CHECKLIST_FINAL.md).
9. Sempre que uma evidência posterior contrariar uma hipótese ou descrição anterior, **revise o projeto**. IHC é um processo iterativo.
10. Diferencie funcionalidades existentes de propostas futuras e instrumentos de pesquisa planejados de dados efetivamente coletados.

## Entregas

| # | Entrega | Quantidade mínima / responsabilidade | Status |
|---:|---|---|---|
| 1 | [Conhecendo o projeto, o usuário e o problema](docs/01_conhecendo_o_problema.md) | 1 solução consolidada por equipe | 🟩 |
| 2 | [Público-alvo e análise de concorrência](docs/02_analise_concorrencia.md) | no mínimo 1 concorrente/interface representativa por integrante + síntese | 🟩 |
| 3 | [Personas, empatia, contexto e jornada](docs/03_personas_contexto_jornada.md) | 1 persona por integrante; demais artefatos consolidados | 🟩 |
| 4 | [Cenários de análise/problema](docs/04_cenarios_problema.md) | 1 solução completa por integrante | 🟩 |
| 5 | [Análise de tarefas: HTA, GOMS e CTT](docs/05_analise_tarefas.md) | cada integrante: pelo menos 1 HTA + 1 GOMS + 1 CTT | 🟩 |
| 6 | [Prototipação em papel](docs/06_prototipacao_papel.md) | 1 protótipo integrado por equipe | 🟩 |
| 7 | [Coleta de dados e aspectos éticos](docs/07_coleta_dados.md) | soluções individuais + técnicas distintas; questionário entre as técnicas | 🟩 |
| 8 | [Ciclo de vida e engenharia de usabilidade](docs/08_engenharia_usabilidade.md) | 1 solução consolidada por equipe | ⬜ |
| 9 | [Modelo conceitual e design centrado na comunicação](docs/09_modelo_conceitual.md) | soluções individuais + consolidação de objetivos/signos | ⬜ |
| 10 | [MoLIC](docs/10_molic.md) | 1 diagrama completo por integrante | ⬜ |
| 11 | [Protótipo no Figma](docs/11_figma.md) | 1 protótipo integrado por equipe, cobrindo fluxos modelados | ⬜ |
| 12 | [Planejamento da avaliação — DECIDE](docs/12_planejamento_avaliacao.md) | 1 plano consolidado por equipe | ⬜ |
| 13 | [Avaliação heurística](docs/13_avaliacao_heuristica.md) | 1 avaliação completa por integrante, todas as telas/estados e 10 heurísticas | ⬜ |
| 14 | [Avaliação por observação de usuários](docs/14_observacao_usuario.md) | avaliação consolidada; nº de participantes finais = nº de integrantes | ⬜ |

> Se o docente definir quantidade diferente para a turma/semestre, a orientação da disciplina prevalece.

## Visão de continuidade

O projeto deve formar uma cadeia de evidências:

**tema/contribuição do TCC → possível aplicação → usuários/stakeholders → objetivos → problema/contexto → alternativas → necessidades → personas → cenários → tarefas → protótipo formativo → avaliação formativa → planejamento de investigação → modelo conceitual → MoLIC → protótipo de alta fidelidade → planejamento de avaliação → inspeção → teste com usuários → melhorias**.

No nosso projeto, o fluxo principal atualmente documentado é:

**definição da malha viária → configuração da simulação e da estratégia de controle → validação e confirmação → execução e acompanhamento → recuperação da execução → análise individual dos resultados → comparação manual quando necessária**.

A Entrega 6 materializa esse fluxo no protótipo digital V0 por meio de:

**PF01 → PF02 → PF03**.

Os estados correspondentes são:

**PP01 → PP02 → PP03 → PP04/PP05 → PP06 → PP07**.

O walkthrough da Entrega 6 acrescentou uma camada de avaliação formativa:

**W01–W04 → O01–O10 → decisões V0→V1**.

A Entrega 7 acrescenta uma camada de investigação metodológica:

**H01/H02/H03 → dados necessários → público → I01/I02 → análise planejada → possível revisão futura**.

Como I01 e I02 não foram aplicados nesta etapa, a Entrega 7 não modifica automaticamente personas, tarefas ou hipóteses. Ela registra como esses elementos poderão ser confrontados com dados caso os instrumentos sejam utilizados futuramente.

Uma entrega não deve “reiniciar” o projeto. Personas, tarefas, protótipos, observações, instrumentos, modelo conceitual, MoLIC e avaliações devem permanecer coerentes com esse fluxo, salvo quando novas evidências justificarem revisão.

## Documentos de apoio

- [Guia de uso e apresentação](GUIA_DE_USO.md)
- [Guia para definir o escopo de IHC a partir do TCC](GUIA_ESCOPO_IHC.md)
- [Matriz de rastreabilidade](RASTREABILIDADE.md)
- [Checklist final](CHECKLIST_FINAL.md)
- [Bibliografia de IHC](BIBLIOGRAFIA.md)
- [Orientações de contribuição no GitHub](CONTRIBUTING.md)
- [Instrumentos reutilizáveis](instrumentos/README.md)
