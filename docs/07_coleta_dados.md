# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 20/10/2026  
**Status:** 🟩 concluída  
**Responsabilidade:** soluções individuais + técnicas distintas; questionário entre as técnicas

## Objetivo da atividade

Planejar os dados necessários para compreender melhor os usuários, suas atividades, necessidades e requisitos de IHC, selecionar técnicas de coleta coerentes com as dúvidas existentes no projeto e produzir instrumentos que possam ser aplicados de forma reproduzível.

Nesta entrega, os instrumentos são **planejados e documentados para eventual aplicação**. Não são apresentados resultados empíricos fictícios e nenhuma hipótese é considerada validada apenas pela elaboração do questionário ou da entrevista.

O projeto já possui hipóteses sobre o usuário prioritário, a organização do fluxo de trabalho e a forma de apresentar os resultados. A Entrega 7 procura transformar essas hipóteses em perguntas de investigação que possam futuramente ser respondidas com evidências.

---

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

| ID | Hipótese/lacuna | Evidência atual | Decisão que depende da resposta | Prioridade |
|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | Entregas 2 e 3 reforçaram a plausibilidade do perfil por meio da análise de ferramentas profissionais e da construção das proto-personas P01 e P02. A Entrega 6 aplicou o protótipo V0 em um walkthrough formativo e produziu observações relacionadas à interação e ao nível de conhecimento técnico exigido. O perfil prioritário representado por P01 e P02, entretanto, permanece como hipótese sujeita a investigação adicional. | Definição do público prioritário, vocabulário utilizado, grau de detalhamento técnico e características das personas. | alta |
| H02 | Organizar a interação em definição do cenário, configuração, execução/acompanhamento e análise facilita a realização dos experimentos. | Entregas 3–5 detalharam a jornada, cenários e tarefas. A Entrega 6 materializou essa hipótese nos fluxos PF01 — Preparar experimento, PF02 — Validar, executar e acompanhar e PF03 — Localizar e analisar resultados. | Organização do fluxo principal, agrupamento das configurações, feedback durante a execução e quantidade de informações apresentadas em cada etapa. | alta |
| H03 | Uma apresentação consolidada e comparativa das métricas facilita a interpretação do desempenho das estratégias. | Entregas 2–5 indicaram a necessidade de relacionar métricas ao contexto experimental e verificar comparabilidade. Na Entrega 6, PP06 representa o histórico e a seleção de execuções e PP07 representa a análise individual dos resultados. A comparação entre execuções é atualmente realizada manualmente fora da interface. | Seleção e hierarquia das métricas, forma de comparação, necessidade de histórico, gráficos, síntese ou detalhamento adicional. | alta |

---

# Parte A — necessidades e requisitos de IHC

> **Responsabilidade:** solução individual por integrante.

---

# A01 — Gabriel Koiama de Rocha Lira

**Autor(a):** Gabriel Koiama de Rocha Lira — 22.125.067-3

## Objetivo da investigação individual

A investigação de Gabriel procura reduzir principalmente as incertezas associadas a H01, H02 e H03.

O foco não é perguntar se o participante “gosta” da interface existente, mas compreender:

- quem realiza ou poderia realizar atividades semelhantes;
- quais ferramentas e processos utiliza;
- quais informações precisa configurar;
- quais erros considera relevantes;
- o que precisa acompanhar durante processamento;
- quais resultados utiliza;
- como realiza comparações;
- quais conceitos e termos são familiares.

Essas informações poderão sustentar ou provocar revisão das proto-personas, tarefas, fluxos e decisões de interface já documentadas.

---

## Que dados coletar?

A coleta foi estruturada a partir das categorias trabalhadas na disciplina: informações sobre o próprio usuário, relação com tecnologia, conhecimento do domínio, tarefas e motivações/valores.

| Categoria | Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|---|
| Usuário | Área de formação ou atuação relacionada a mobilidade, engenharia, computação, simulação ou análise de dados. | H01 | Permite verificar se o perfil priorizado possui correspondência com pessoas que realizam atividades próximas às consideradas pelo projeto. | Refinamento de P01/P02 e definição do público prioritário. |
| Usuário | Papel exercido em atividades de análise, pesquisa, simulação ou tomada de decisão. | H01 | Diferentes papéis podem possuir objetivos e necessidades distintas. | Priorização de funcionalidades e distinção entre persona primária e secundária. |
| Tecnologia | Experiência com ferramentas de simulação, análise, planilhas, scripts ou softwares técnicos. | H01, H02 | O nível de experiência influencia terminologia, necessidade de ajuda e quantidade de detalhes técnicos que podem ser apresentados diretamente. | Complexidade da interface, ajuda contextual e vocabulário. |
| Tecnologia | Ferramentas utilizadas atualmente para realizar atividades semelhantes. | H01, H02 | Permite conhecer referências e processos já utilizados pelos potenciais usuários. | Organização da navegação, padrões de interação e integração com atividades existentes. |
| Domínio | Familiaridade com simulação, experimentação, controle de tráfego ou análise de métricas. | H01 | É necessário distinguir conhecimento do domínio de conhecimento da implementação interna do TCC. | Quantidade de explicações, termos técnicos e informações exibidas. |
| Domínio | Vocabulário utilizado para conceitos como cenário, execução, controlador, simulação visual e processamento sem interface gráfica. | H01, H02 | A interface deve utilizar linguagem compreensível ao usuário e não apenas nomes internos do código. | Rótulos, mensagens e signos das Entregas 9–11. |
| Tarefas | Forma atual de preparar uma análise ou experimento. | H02 | Permite verificar se o fluxo PF01 corresponde a uma organização plausível da atividade. | Ordem das etapas e organização da configuração. |
| Tarefas | Informações verificadas antes de iniciar uma execução. | H02 | Configurações incorretas podem comprometer comparabilidade e gerar retrabalho. | Resumo de configuração, validações e prevenção de erros. |
| Tarefas | Parâmetros ou condições considerados importantes em uma execução. | H02 | Nem todo parâmetro interno do sistema precisa necessariamente ser exposto ao usuário. | Conteúdo de PP02 e futuras telas de configuração. |
| Tarefas | Erros ou inconsistências considerados mais críticos. | H02 | Permite priorizar validações e mensagens de recuperação. | PP03, prevenção e recuperação de erros. |
| Tarefas | Informações necessárias durante uma execução demorada. | H02 | O usuário precisa reconhecer se o sistema está funcionando e qual execução está ativa. | PP04, feedback, progresso e cancelamento. |
| Tarefas | Informações consultadas primeiro após uma execução. | H03 | Permite identificar quais resultados merecem maior destaque. | Hierarquia de PP07 e futuras telas de resultados. |
| Tarefas | Forma atual de comparar diferentes execuções ou alternativas. | H03 | Permite compreender se a comparação acontece por planilhas, gráficos, scripts, relatórios ou outro processo. | PP06/PP07 e comparação manual externa no fluxo PF03. |
| Tarefas | Condições consideradas necessárias para que duas execuções sejam comparáveis. | H02, H03 | Comparações sem equivalência podem produzir conclusões inadequadas. | Critérios de comparabilidade e contexto apresentado junto aos resultados. |
| Tarefas | Forma utilizada para localizar resultados ou execuções anteriores. | H03 | Permite investigar se existe necessidade real de histórico, busca ou filtros. | Decisão sobre histórico e mecanismos de recuperação de execuções. |
| Motivações/valores | Prioridade entre rapidez, rastreabilidade, controle detalhado e facilidade de interpretação. | H02, H03 | Usuários diferentes podem valorizar controle técnico ou síntese de maneira distinta. | Equilíbrio entre detalhamento e simplicidade. |
| Motivações/valores | Principal dificuldade percebida ao trabalhar com experimentos ou análises semelhantes. | H01, H02, H03 | Pergunta exploratória pode revelar necessidades não antecipadas pela equipe. | Possível revisão de tarefas, fluxos, signos e protótipo. |

---

## Minimização dos dados

Embora dados demográficos possam ser utilizados em pesquisas de usuários, nesta investigação não existe justificativa para coletar informações como:

- nome completo;
- CPF;
- endereço;
- renda;
- sexo;
- data de nascimento;
- empresa específica, quando não for necessária;
- outros dados pessoais não relacionados aos objetivos da pesquisa.

A coleta prioriza características diretamente relacionadas à interação, como formação, papel, experiência e familiaridade com ferramentas.

---

## De quem coletar?

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Pesquisador ou profissional relacionado à mobilidade, tráfego ou simulação | Possuir experiência acadêmica ou profissional com estudos, simulações, análise de mobilidade ou experimentos semelhantes. | Perfil mais próximo de P01 — Marina Ribeiro. |
| Analista, engenheiro ou pesquisador que trabalhe com ferramentas técnicas ou análise experimental | Realizar configuração, execução ou interpretação de processos computacionais com parâmetros e resultados. | Pode fornecer evidências sobre H01 e H02 mesmo quando não utiliza exatamente o mesmo simulador do TCC. |
| Gestor/coordenador que consulte resultados técnicos | Utilizar resultados consolidados de análises ou estudos para apoiar decisões. | Aproxima-se de P02 — Carlos Mendes e pode contribuir principalmente para H03. |
| Participante proxy com experiência acadêmica em computação, engenharia, simulação ou análise de dados | Possuir familiaridade com experimentação ou ferramentas técnicas, mesmo sem atuação profissional em mobilidade. | Alternativa metodológica quando o acesso ao público especializado for inviável. Deve ser identificada explicitamente como proxy e não tratada como equivalente ao usuário final. |

---

## Limitação de recrutamento

O público prioritário definido pelo projeto possui caráter especializado. A equipe não possui, neste momento, acesso direto garantido a pesquisadores ou profissionais de mobilidade urbana.

Caso o instrumento seja aplicado futuramente, participantes proxy poderão ser utilizados quando necessário, desde que:

- o perfil real seja descrito corretamente;
- não sejam apresentados como especialistas quando não forem;
- a limitação seja registrada;
- as conclusões sejam restritas ao tipo de participante efetivamente recrutado.

---

## Aspectos éticos — A01

Qualquer futura aplicação do instrumento deve considerar voluntariedade, consentimento, privacidade, minimização de dados e possibilidade de desistência.

### Voluntariedade

A participação deverá ser voluntária.

O participante deverá ser informado de que pode:

- recusar o convite;
- deixar perguntas opcionais sem resposta;
- interromper sua participação a qualquer momento;
- desistir sem necessidade de justificativa.

### Consentimento

Antes do início do questionário, o participante deverá receber uma explicação breve contendo:

- objetivo acadêmico da atividade;
- responsáveis pela coleta;
- tipo de informação solicitada;
- duração aproximada;
- forma de utilização dos dados;
- condição voluntária da participação.

O prosseguimento para as perguntas deverá ocorrer somente após manifestação de concordância.

### Minimização de dados

Serão solicitadas somente informações relacionadas aos objetivos da investigação.

O questionário não necessita de:

- CPF;
- endereço;
- telefone;
- dados financeiros;
- dados sensíveis;
- identificação pessoal completa.

Caso seja utilizado Google Forms ou ferramenta semelhante, a coleta automática de endereço de e-mail deverá permanecer **desabilitada**, salvo necessidade posterior explicitamente justificada.

### Anonimização

Caso os dados sejam analisados ou apresentados, os participantes deverão ser representados por identificadores como:

`Q01`, `Q02`, `Q03`...

Respostas abertas não deverão ser publicadas juntamente com informações que permitam identificar o participante.

### Gravação

O questionário não necessita de gravação de áudio, vídeo ou tela.

Caso uma técnica futura envolva gravação, deverá existir autorização específica para esse registro.

### Armazenamento

Caso o questionário seja aplicado:

- os dados brutos deverão permanecer em pasta privada acessível somente à equipe;
- versões publicadas no repositório deverão conter apenas dados anonimizados e consolidados;
- os dados identificáveis, caso excepcionalmente existentes, não deverão ser publicados.

### Descarte

Os dados brutos de eventual aplicação deverão ser mantidos apenas durante o período necessário à disciplina e à consolidação acadêmica.

Após o encerramento da atividade e quando não houver necessidade institucional de preservação, dados identificáveis deverão ser eliminados.

### Risco da participação

O instrumento possui risco reduzido, pois trata principalmente de experiência profissional/acadêmica, ferramentas, atividades e opiniões sobre processos de trabalho.

Mesmo assim, o participante não deverá ser pressionado a revelar:

- informações confidenciais de empresas ou instituições;
- projetos sigilosos;
- dados de clientes;
- credenciais;
- informações pessoais desnecessárias.

---

# A02 — João Pedro Lopes Santana Villas Bôas

**Autor(a):** João Pedro Lopes Santana Villas Bôas — 22.125.065-7

## Objetivo da investigação individual

A investigação de João complementa a abordagem estruturada do questionário de Gabriel utilizando uma técnica qualitativa capaz de aprofundar **como as atividades realmente seriam realizadas, quais decisões acontecem durante o processo e por que determinadas informações são consideradas importantes**.

O foco principal está em H02 e H03, sem deixar de produzir evidências relacionadas a H01.

A investigação pretende compreender principalmente:

- como o participante organiza uma atividade técnica do início ao fim;
- que decisões precisa tomar antes e durante uma execução;
- quais informações utiliza para detectar erros;
- como interpreta resultados;
- como decide se resultados são comparáveis;
- qual nível de detalhamento considera necessário;
- qual vocabulário utiliza;
- como comunica uma conclusão técnica para outra pessoa;
- quais dificuldades não foram antecipadas pela equipe.

A entrevista não será utilizada para apresentar o protótipo V0 e perguntar se o participante “gosta” das telas. Seu objetivo é investigar o trabalho, o raciocínio e as necessidades do participante antes de avaliar uma solução específica.

---

## Que dados coletar?

| Categoria | Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|---|
| Usuário | Papel do participante em atividades técnicas, acadêmicas ou de análise. | H01 | Permite compreender em que contexto suas respostas devem ser interpretadas. | Refinamento das personas e definição dos papéis prioritários. |
| Usuário | Grau de autonomia para configurar, executar e interpretar análises. | H01 | Pessoas responsáveis apenas por consultar resultados podem possuir necessidades diferentes de quem realiza todo o processo. | Separação entre necessidades de P01 e P02. |
| Tecnologia | Ferramentas utilizadas e motivo de sua escolha. | H01, H02 | O motivo de uso revela necessidades que não aparecem apenas em uma lista de softwares. | Padrões de interação, compatibilidade com expectativas e terminologia. |
| Domínio | Conceitos e termos utilizados espontaneamente pelo participante. | H01 | Permite identificar a linguagem natural utilizada no domínio ou em atividades técnicas próximas. | Signos, rótulos e mensagens das Entregas 9–11. |
| Tarefas | Descrição passo a passo de uma atividade real ou semelhante de configuração e análise. | H02 | Permite comparar o fluxo real com PF01, PF02 e PF03. | Estrutura geral da navegação e ordem das interações. |
| Tarefas | Decisões tomadas antes de iniciar uma execução. | H02 | Ajuda a identificar quais informações precisam estar disponíveis antes da confirmação. | PP02, validação e resumo da configuração. |
| Tarefas | Forma de perceber se uma execução está correta ou apresentou problema. | H02 | Ajuda a entender quais feedbacks possuem significado para o usuário. | PP03 e PP04. |
| Tarefas | Ações tomadas diante de erro ou resultado inesperado. | H02 | Permite modelar recuperação, retorno e reexecução. | Estados de erro, mensagens e caminhos de recuperação. |
| Tarefas | Processo utilizado para interpretar uma execução concluída. | H03 | Permite identificar sequência de leitura e importância relativa das informações. | PP07 e hierarquia das métricas. |
| Tarefas | Critérios utilizados para comparar duas alternativas. | H03 | Ajuda a distinguir métricas importantes de condições necessárias para comparação. | PP06/PP07, comparação manual externa e critérios de comparabilidade. |
| Tarefas | Forma de recuperar resultados anteriores. | H03 | Permite avaliar a necessidade real de histórico, busca, filtros ou organização por pastas. | PP06, histórico e recuperação de execuções. |
| Comunicação | Forma de explicar um resultado a outra pessoa. | H03 | Um pesquisador e um gestor podem necessitar de níveis distintos de síntese. | Relatórios, visualizações e sínteses. |
| Motivações/valores | Situações em que o participante prefere controle detalhado ou simplicidade. | H02, H03 | Ajuda a evitar tanto simplificação excessiva quanto exposição desnecessária de detalhes. | Hierarquia de informação e recursos avançados. |
| Dificuldades | Exemplo concreto de dificuldade, erro ou retrabalho em ferramenta técnica. | H02, H03 | Experiências reais podem revelar problemas não previstos pela equipe. | Revisão dos requisitos e fluxos. |
| Necessidades abertas | Recurso ou informação que faria diferença no processo do participante. | H01, H02, H03 | Mantém espaço para necessidades não previstas nas hipóteses iniciais. | Revisão de qualquer artefato afetado. |

---

## De quem coletar?

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Pesquisador ou profissional que configure e analise experimentos, simulações ou estudos técnicos | Possuir experiência concreta em preparação, execução e interpretação de processos experimentais. | Perfil mais próximo de P01. |
| Analista ou engenheiro que utilize indicadores para interpretar resultados | Ter experiência com resultados quantitativos, comparação ou análise técnica. | Contribui para H02 e H03. |
| Professor, pesquisador ou estudante de pós-graduação relacionado a simulação ou análise experimental | Participar de atividades que envolvam configuração, processamento e análise de resultados. | Aproximação acadêmica do contexto de P01. |
| Gestor/coordenador técnico | Utilizar resultados produzidos por outras pessoas para apoiar avaliações ou decisões. | Perfil próximo de P02. |
| Participante proxy de Computação ou Engenharia | Possuir experiência com softwares técnicos, experimentos ou análise de dados. | Alternativa quando o público especializado não puder ser recrutado, com limitação explícita. |

---

## Estratégia de amostragem planejada

A entrevista busca **profundidade**, e não representação estatística.

Caso fosse aplicada, seria priorizado inicialmente um pequeno número de participantes com experiência relevante para as perguntas da pesquisa.

A quantidade exata dependeria:

- da disponibilidade do público;
- da diversidade dos perfis encontrados;
- do tempo disponível;
- do objetivo específico da aplicação.

Uma entrevista isolada não seria utilizada para afirmar que uma necessidade é universal.

Da mesma forma, entrevistas com participantes proxy seriam interpretadas apenas dentro das limitações de seu perfil.

---

## Aspectos éticos — A02

A entrevista envolve maior interação com o participante do que o questionário e, caso exista gravação, exige cuidados adicionais.

### Voluntariedade

A participação deve ser inteiramente voluntária.

O entrevistado poderá:

- recusar o convite;
- não responder a uma pergunta;
- solicitar interrupção temporária;
- encerrar a entrevista a qualquer momento;
- pedir que determinada resposta não seja utilizada.

### Consentimento

Antes da entrevista, o participante deverá receber informações sobre:

- objetivo acadêmico;
- duração aproximada;
- assuntos abordados;
- responsáveis pela atividade;
- forma de registro;
- anonimização;
- armazenamento;
- direito de desistência.

O início da entrevista deverá ocorrer somente após o consentimento.

### Gravação

A gravação de áudio **não é obrigatória**.

Caso seja utilizada, deverá existir consentimento específico.

O participante deverá poder aceitar:

- participar e permitir gravação;
- participar sem gravação;
- recusar a participação.

Se não houver gravação, o entrevistador poderá trabalhar apenas com anotações estruturadas.

Não há necessidade prevista de gravação de vídeo.

### Anonimização

Participantes deverão ser identificados por códigos:

`E01`, `E02`, `E03`...

No documento público poderão ser registrados apenas dados gerais relevantes, por exemplo:

> E01 — estudante de pós-graduação com experiência em simulação.

Não deverão ser publicados nome, instituição ou informações capazes de identificar a pessoa sem necessidade e autorização.

### Confidencialidade profissional

O roteiro deverá deixar claro que o participante não precisa fornecer:

- informações confidenciais;
- nomes de clientes;
- dados internos de empresas;
- códigos proprietários;
- resultados sigilosos;
- qualquer informação protegida.

Caso uma resposta contenha acidentalmente informação confidencial, essa parte deverá ser excluída da documentação pública.

### Armazenamento

Notas ou gravações deverão permanecer em área privada da equipe.

O GitHub público deverá receber apenas:

- sínteses;
- dados anonimizados;
- categorias de análise;
- trechos anonimizados quando realmente necessários.

### Descarte

Gravações e dados identificáveis deverão ser descartados após sua finalidade acadêmica, salvo exigência institucional diferente.

---

# Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**, conforme o enunciado da disciplina.

A equipe definiu duas técnicas complementares:

| ID | Integrante | Técnica | Principal contribuição |
|---|---|---|---|
| I01 | Gabriel Koiama de Rocha Lira | Questionário | Coleta estruturada e comparável sobre perfil, atividades, ferramentas, execução e resultados. |
| I02 | João Pedro Lopes Santana Villas Bôas | Entrevista semiestruturada | Aprofundamento qualitativo do processo de trabalho, decisões, dificuldades, linguagem e critérios de análise. |

---

# Instrumento I01 — Questionário exploratório sobre atividades de simulação e análise

**Autor(a):** Gabriel Koiama de Rocha Lira — 22.125.067-3  
**Técnica:** Questionário  
**Hipóteses relacionadas:** H01, H02 e H03  
**Situação atual:** instrumento planejado para eventual aplicação; ainda não aplicado.

## Objetivo

Investigar características relevantes dos potenciais usuários e de suas atividades, com foco em:

- experiência com ferramentas técnicas;
- familiaridade com simulações ou análises experimentais;
- preparação de execuções;
- parâmetros e condições consideradas importantes;
- necessidades de acompanhamento;
- tratamento de erros;
- métricas consultadas;
- processo de comparação;
- recuperação de resultados anteriores;
- linguagem e conceitos utilizados.

O questionário deverá produzir evidências que possam futuramente sustentar, refutar ou refinar H01, H02 e H03.

---

## Público

### Público ideal

Pesquisadores, analistas, engenheiros, professores, estudantes de pós-graduação ou profissionais que possuam experiência com:

- mobilidade urbana;
- tráfego;
- simulação;
- experimentação computacional;
- análise de dados;
- ferramentas técnicas com configuração, processamento e interpretação de resultados.

### Participantes proxy

Caso não seja possível acessar o público especializado, poderão participar pessoas com experiência em computação, engenharia, análise experimental ou utilização de softwares técnicos.

A utilização de proxies deverá ser explicitada durante a análise e não permitirá generalizar os resultados como se fossem provenientes de especialistas em mobilidade.

---

## Duração planejada

**Aproximadamente 5 a 8 minutos.**

O questionário foi mantido relativamente curto para reduzir abandono e evitar coleta de informações que não possuem consequência clara para o projeto.

---

## Meio de aplicação previsto

Preferencialmente formulário digital, como Google Forms ou ferramenta equivalente.

Uma eventual versão on-line deverá:

- não exigir autenticação desnecessária;
- não coletar e-mail automaticamente;
- apresentar consentimento antes das perguntas;
- permitir respostas anônimas;
- manter perguntas abertas opcionais quando envolverem descrição pessoal.

---

## Procedimento padronizado de aplicação

### 1. Preparação

Antes de divulgar o questionário:

1. revisar todas as perguntas;
2. confirmar que não existem perguntas duplicadas ou indutivas;
3. desabilitar coleta automática de e-mail;
4. testar o formulário em computador e celular;
5. realizar uma aplicação piloto apenas para verificar clareza do instrumento;
6. corrigir erros de redação antes da divulgação definitiva.

### 2. Apresentação e consentimento

A primeira página deverá apresentar:

- título;
- objetivo acadêmico;
- responsáveis;
- duração aproximada;
- caráter voluntário;
- política de privacidade;
- informação sobre anonimização;
- possibilidade de abandonar a participação.

O participante deverá selecionar:

`( ) Li as informações acima e concordo voluntariamente em participar.`

Caso não concorde, o formulário deverá ser encerrado.

### 3. Aplicação

O participante responde individualmente às perguntas.

Não deverão ser fornecidas explicações adicionais que direcionem respostas, exceto quando houver dúvida sobre o significado literal de uma pergunta.

### 4. Encerramento

Ao final, deverá ser exibida uma mensagem de agradecimento e um campo opcional para comentários adicionais.

### 5. Armazenamento e anonimização

Caso aplicado:

- exportar respostas para arquivo de análise;
- atribuir IDs `Q01`, `Q02` etc.;
- remover qualquer identificação não necessária;
- manter dados brutos em local privado;
- utilizar somente resultados anonimizados em documentos públicos.

---

# Instrumento — questionário completo

## Texto de abertura

### Questionário sobre atividades de simulação e análise de resultados

Este questionário faz parte de uma atividade acadêmica da disciplina de Interação Humano-Computador do Centro Universitário FEI.

O objetivo é compreender como pessoas que trabalham ou estudam áreas técnicas realizam atividades relacionadas a configuração, execução e análise de experimentos ou simulações.

Não estamos avaliando o conhecimento do participante.

A participação é voluntária, leva aproximadamente **5 a 8 minutos** e pode ser interrompida a qualquer momento.

Não é necessário informar nome completo, CPF, endereço ou qualquer outro dado pessoal desnecessário.

Os dados, caso coletados, serão utilizados somente para fins acadêmicos e apresentados de forma anonimizada.

### Consentimento

**Q00. Você concorda voluntariamente em participar deste questionário nos termos apresentados acima?**

- ( ) Sim
- ( ) Não

**Regra:** se a resposta for “Não”, encerrar o formulário.

---

## Seção 1 — Perfil e experiência

### Q01. Qual opção melhor descreve sua área de formação, estudo ou atuação?

**Tipo:** múltipla escolha com seleção de uma ou mais opções.

- [ ] Mobilidade urbana / transportes
- [ ] Engenharia de tráfego
- [ ] Engenharia em outra área
- [ ] Ciência da Computação / Sistemas de Informação / área de software
- [ ] Ciência de dados / análise de dados
- [ ] Pesquisa acadêmica
- [ ] Gestão ou coordenação técnica
- [ ] Outra área técnica
- [ ] Nenhuma das anteriores
- [ ] Outro: ________

**Relação:** H01.

---

### Q02. Qual opção melhor descreve sua experiência com softwares técnicos, simulações ou análise computacional?

**Tipo:** escolha única.

- ( ) Nunca utilizei
- ( ) Já tive contato pontual
- ( ) Utilizo eventualmente
- ( ) Utilizo com frequência
- ( ) Trabalho ou pesquiso diretamente com esse tipo de ferramenta

**Relação:** H01.

---

### Q03. Quais tipos de ferramentas você já utilizou em atividades técnicas ou acadêmicas?

**Tipo:** múltipla escolha.

- [ ] Planilhas
- [ ] Ferramentas de análise de dados
- [ ] Scripts ou programas próprios
- [ ] Simuladores
- [ ] Dashboards ou ferramentas de BI
- [ ] Softwares de engenharia
- [ ] Ferramentas específicas de mobilidade/tráfego
- [ ] Nunca utilizei ferramentas desse tipo
- [ ] Outro: ________

**Relação:** H01 e H02.

---

### Q04. Caso já tenha utilizado simuladores ou ferramentas especializadas, quais?

**Tipo:** resposta curta ou aberta.  
**Obrigatoriedade:** opcional.

**Relação:** H01.

---

## Seção 2 — Preparação e configuração

### Q05. Em uma atividade que envolve executar uma simulação, análise ou experimento, quais informações você considera importante revisar antes de iniciar?

**Tipo:** múltipla escolha.

- [ ] Cenário ou conjunto de dados utilizado
- [ ] Parâmetros configurados
- [ ] Método, algoritmo ou estratégia selecionada
- [ ] Condição de entrada ou demanda
- [ ] Seed ou outra condição de reprodutibilidade
- [ ] Duração ou horizonte da execução
- [ ] Local em que os resultados serão armazenados
- [ ] Versão ou configuração do método utilizado
- [ ] Normalmente não faço esse tipo de verificação
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ________

**Relação:** H02.

---

### Q06. Qual situação seria mais problemática em uma execução técnica?

**Tipo:** escolha única.

- ( ) Utilizar parâmetros incorretos
- ( ) Utilizar cenário ou entrada incorretos
- ( ) Executar método diferente do planejado
- ( ) Não saber exatamente quais condições produziram um resultado
- ( ) Descobrir o erro somente após o processamento
- ( ) Não conseguir identificar se a execução falhou
- ( ) Não tenho experiência suficiente para responder
- ( ) Outro: ________

**Relação:** H02.

---

### Q07. Quando existem muitos parâmetros técnicos, qual abordagem costuma ser mais útil para você?

**Tipo:** escolha única.

- ( ) Ver todos os parâmetros ao mesmo tempo
- ( ) Ver primeiro os parâmetros principais e acessar os avançados quando necessário
- ( ) Utilizar configurações pré-definidas e alterar somente alguns parâmetros
- ( ) Depende da atividade
- ( ) Não tenho experiência suficiente para responder
- ( ) Outro: ________

**Relação:** H02.

---

## Seção 3 — Execução e acompanhamento

### Q08. Durante uma execução que demora algum tempo, quais informações você considera mais importantes?

**Tipo:** múltipla escolha.

- [ ] Indicação clara de que a execução está ativa
- [ ] Percentual ou progresso
- [ ] Tempo decorrido
- [ ] Estimativa de tempo restante
- [ ] Cenário ou entrada em execução
- [ ] Método/algoritmo atualmente executado
- [ ] Parâmetros principais da execução
- [ ] Mensagens de erro
- [ ] Logs ou detalhes técnicos
- [ ] Opção de cancelar
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ________

**Relação:** H02.

---

### Q09. Quando uma execução apresenta erro, qual informação é mais importante para você?

**Tipo:** escolha única.

- ( ) Saber apenas que houve erro
- ( ) Saber em qual etapa ocorreu
- ( ) Entender a provável causa
- ( ) Receber orientação sobre como corrigir
- ( ) Acessar detalhes técnicos completos
- ( ) Uma combinação das alternativas anteriores
- ( ) Não tenho experiência suficiente para responder
- ( ) Outro: ________

**Relação:** H02.

---

## Seção 4 — Resultados e comparação

### Q10. Quando uma execução termina, quais informações você normalmente procura primeiro?

**Tipo:** múltipla escolha.

- [ ] Resultado principal da execução
- [ ] Indicadores ou métricas de desempenho
- [ ] Condições/parâmetros utilizados
- [ ] Ocorrência de erros ou alertas
- [ ] Gráficos
- [ ] Dados detalhados
- [ ] Comparação com outra execução
- [ ] Local dos arquivos completos
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ________

**Relação:** H03.

---

### Q11. Em uma análise de tráfego ou simulação semelhante, quais indicadores você consideraria relevantes?

**Tipo:** múltipla escolha.

- [ ] Tempo médio de espera
- [ ] Tempo médio de viagem
- [ ] Tamanho das filas
- [ ] Throughput / quantidade de veículos processados
- [ ] Veículos que não concluíram a execução
- [ ] Trocas de fase
- [ ] Duração das fases verdes
- [ ] Erros, colisões ou teleports
- [ ] Não conheço essas métricas suficientemente
- [ ] Outro: ________

**Relação:** H03.

> A pergunta permite a opção de desconhecimento para evitar presumir que todo participante possui domínio especializado em tráfego.

---

### Q12. Quando você precisa comparar diferentes execuções ou alternativas, como costuma realizar essa comparação?

**Tipo:** múltipla escolha.

- [ ] Comparação manual dos valores
- [ ] Planilha
- [ ] Gráficos
- [ ] Relatório
- [ ] Script ou análise automatizada
- [ ] Dashboard
- [ ] Ferramenta específica do domínio
- [ ] Não costumo realizar esse tipo de comparação
- [ ] Outro: ________

**Relação:** H03.

---

### Q13. Quais condições você considera que precisam permanecer identificáveis ao comparar duas execuções?

**Tipo:** múltipla escolha.

- [ ] Cenário
- [ ] Entrada/demanda
- [ ] Parâmetros principais
- [ ] Seed
- [ ] Duração/horizonte
- [ ] Método ou algoritmo
- [ ] Versão da configuração
- [ ] Data da execução
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ________

**Relação:** H02 e H03.

---

### Q14. Quando precisa consultar uma execução antiga, como normalmente a localiza?

**Tipo:** escolha única.

- ( ) Pela pasta/estrutura de arquivos
- ( ) Pelo nome do experimento
- ( ) Pela data
- ( ) Por uma planilha ou registro separado
- ( ) Por histórico dentro da própria ferramenta
- ( ) Por busca ou filtros
- ( ) Não costumo consultar execuções antigas
- ( ) Outro: ________

**Relação:** H03.

> Esta pergunta investiga a necessidade de histórico sem pressupor que um histórico avançado seja obrigatoriamente necessário.

---

## Seção 5 — Linguagem e necessidades

### Q15. Que termos você utilizaria para diferenciar uma execução que mostra visualmente a simulação de outra executada apenas em processamento, sem interface gráfica?

**Tipo:** resposta aberta.  
**Obrigatoriedade:** opcional.

**Relação:** H01 e H02.

---

### Q16. Pensando em ferramentas técnicas ou de análise que você já utilizou, qual dificuldade mais atrapalha sua experiência?

**Tipo:** resposta aberta.  
**Obrigatoriedade:** opcional.

**Relação:** H01, H02 e H03.

---

### Q17. Existe alguma informação ou recurso que você considera importante em uma ferramenta de configuração, execução e análise e que não apareceu nas perguntas anteriores?

**Tipo:** resposta aberta.  
**Obrigatoriedade:** opcional.

**Relação:** H01, H02 e H03.

---

## Mensagem de encerramento

Obrigado pela participação.

As respostas, caso coletadas, serão utilizadas somente para fins acadêmicos e analisadas de forma anonimizada.

---

## Como os dados do I01 seriam analisados

A análise deverá combinar resultados quantitativos simples das perguntas fechadas com categorização qualitativa das respostas abertas.

Não há necessidade de inferência estatística complexa, especialmente se a amostra for pequena ou composta por participantes proxy.

### Perguntas fechadas

Serão calculadas:

- frequências absolutas;
- proporção de participantes por alternativa;
- alternativas predominantes;
- padrões de coocorrência quando forem relevantes.

Exemplo hipotético:

```text
Q08 — informações durante execução

6 participantes marcaram progresso
5 marcaram método ativo
5 marcaram mensagens de erro
2 marcaram logs completos
