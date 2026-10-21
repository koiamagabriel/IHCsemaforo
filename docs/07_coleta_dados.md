# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 20/10/2026  
**Status:** 🟩 concluída  
**Responsabilidade:** soluções individuais + técnicas distintas; questionário entre as técnicas

## Objetivo da atividade

Identificar quais informações sobre usuários, tarefas, tecnologias e contexto ainda precisam ser investigadas e produzir instrumentos de coleta adequados às hipóteses do projeto. A Entrega 7 foi desenvolvida como **planejamento de investigação**, com instrumentos prontos para eventual aplicação, e não como relatório de pesquisa empírica já realizada.

A equipe não aplicou o questionário nem a entrevista nesta etapa. Por isso, não são apresentados participantes, respostas ou resultados observados, e H01–H03 permanecem hipóteses abertas. As referências à V0 dizem respeito às evidências e ao walkthrough formativo da Entrega 6, não a um teste com usuários externos.

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

| ID | Hipótese a investigar | Evidência documental disponível | Decisões que dependem de investigação |
|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário. | E1–E3 estabeleceram o público e as proto-personas P01/P02; E6 examinou a V0 de forma formativa. | Perfil prioritário, linguagem, nível de ajuda e detalhamento técnico. |
| H02 | Organizar a interação em cenário → configuração → execução/acompanhamento → análise facilita os experimentos. | E3–E5 modelaram atividades; E6 documentou PF01–PF03 e observações O01–O07. | Navegação, distribuição dos parâmetros, validação, feedback e recuperação de erros. |
| H03 | Uma apresentação consolidada e comparativa das métricas facilitaria a interpretação. | E6 mostra PP06 como histórico/seleção e PP07 como análise individual; comparação entre duas execuções segue manual e externa. | Hierarquia das métricas, identificação de condições comparáveis, síntese e eventual apoio à comparação. |

As hipóteses orientam as perguntas, mas não devem induzir os participantes a confirmar decisões já imaginadas pela equipe.

---

# Parte A — Necessidades e requisitos de IHC

A aula **Identificação de Necessidades — Parte A** orienta considerar dados sobre o usuário, sua relação com a tecnologia, seu conhecimento do domínio, suas tarefas, motivações e valores. Cada integrante organizou essas categorias de acordo com seu instrumento.

## A01 — Gabriel Koiama de Rocha Lira

**Autor:** Gabriel Koiama de Rocha Lira — RA 22.125.067-3  
**Instrumento associado:** I01 — Questionário exploratório.

### Objetivo da investigação individual

Caracterizar potenciais usuários de ferramentas técnicas e descobrir como preparam experimentos, acompanham execução e interpretam resultados. O levantamento visa identificar preferências e dificuldades que possam revisar P01/P02, T01–T08 e os fluxos PF01–PF03; não pretende avaliar a pessoa ou provar que a V0 é a melhor solução.

### Que dados coletar?

| Categoria | Informação necessária | Hipótese | Consequência possível para IHC |
|---|---|---|---|
| Usuário | Área de formação/atuação, papel em estudos e análises. | H01 | Refino de P01/P02 e do perfil prioritário. |
| Relação com tecnologia | Experiência com softwares técnicos, planilhas, simuladores e scripts. | H01/H02 | Ajuda contextual, vocabulário e densidade dos controles. |
| Conhecimento do domínio | Familiaridade com simulação, tráfego e métricas. | H01 | Distinção entre conceitos do domínio e detalhes internos da implementação. |
| Preparação | Parâmetros e verificações antes da execução. | H02 | Organização de PP02, validação e confirmação em PP03. |
| Execução | Informações necessárias para acompanhar processamento. | H02 | Estado principal, progresso e logs de PP04. |
| Erros | Ocorrências críticas e informações de recuperação. | H02 | Mensagens e caminhos para corrigir uma configuração. |
| Resultados | Métricas consultadas primeiro e condições para comparar. | H03 | Hierarquia dos resultados, contexto experimental e PF03. |
| Histórico | Forma de localizar análises antigas. | H03 | Avaliar necessidades reais de busca ou filtragem, sem impor solução. |
| Linguagem | Termos utilizados espontaneamente para execução visual e sem interface gráfica. | H01/H02 | Rótulos, signos e ajuda das E9–E11. |
| Motivações/valores | Prioridade entre controle, rapidez, rastreabilidade e facilidade de interpretação. | H02/H03 | Equilíbrio entre simplicidade e detalhamento. |

### De quem coletar?

O público ideal reúne pesquisadores, analistas e engenheiros de tráfego ou mobilidade e pessoas que conduzam simulações e análises experimentais. Coordenadores que interpretam relatórios podem contribuir para H03. Se esse público especializado não estiver disponível, participantes *proxy* com experiência em Computação, Engenharia ou análise de dados poderão responder; nessa situação, a limitação deve ser identificada, sem tratá-los como especialistas em mobilidade.

### Minimização dos dados e aspectos éticos — A01

- **Voluntariedade:** convite sem pressão, possibilidade de recusa, de deixar questões abertas opcionais e de interromper a participação.
- **Consentimento:** informação prévia sobre objetivo, equipe, duração, uso acadêmico, privacidade e desistência; sem aceite, encerrar o formulário.
- **Dados necessários:** formação/área e experiência pertinente. Não solicitar nome completo, CPF, endereço, renda, dados de saúde, credenciais ou informações comerciais confidenciais.
- **Privacidade:** desabilitar coleta automática de e-mails e limitar acesso à planilha bruta à equipe.
- **Identificadores:** registros hipotéticos de respondentes serão `UQ01`, `UQ02` etc., para não confundir participantes com as perguntas `Q01`–`Q17`.
- **Gravação:** não é necessária para o questionário; gravações em outra atividade exigiriam consentimento específico.
- **Armazenamento e descarte:** manter registros apenas pelo período justificado para a atividade e eliminar identificação desnecessária ao término, respeitando eventuais normas institucionais.
- **Riscos:** evitar exposição de dados pessoais, de projetos profissionais ou instituições; permitir que o participante pule questões sensíveis ao contexto.

---

## A02 — João Pedro Lopes Santana Villas Bôas

**Autor:** João Pedro Lopes Santana Villas Bôas — RA 22.125.065-7  
**Instrumento associado:** I02 — Entrevista semiestruturada.

### Objetivo da investigação individual

Investigar qualitativamente **como** uma pessoa organiza uma tarefa técnica, **por que** confere determinadas condições, **como** percebe falhas e **como** interpreta/comunica resultados. Complementa o questionário I01, sobretudo em H02 e H03, explorando exemplos concretos e decisões espontâneas, sem apresentar a V0 como solução que deva ser aprovada.

### Que dados coletar?

| Categoria | Informação desejada | Hipótese | Consequência possível para IHC |
|---|---|---|---|
| Papel e autonomia | Se configura, executa, analisa ou apenas utiliza conclusões. | H01 | Diferenciar atividades de P01/P02. |
| Experiência tecnológica | Ferramentas usadas e razões para escolhê-las. | H01/H02 | Compatibilidade com modelos mentais e expectativas. |
| Preparação da tarefa | Sequência real, verificações e parâmetros importantes. | H02 | Revisão de PF01, PP02 e PP03. |
| Acompanhamento | Como percebe progresso, erro e interrupção. | H02 | Feedback e recuperação em PF02. |
| Interpretação | Como decide quais métricas examinar e se confia no resultado. | H03 | Hierarquia de PP07 e relação entre execução e configuração. |
| Comparação | Como verifica equivalência e compara alternativas. | H02/H03 | Apoio atual e futuro à T07, sem atribuir comparador à V0. |
| Histórico | Como recupera e identifica análises antigas. | H03 | Organização de PP06. |
| Comunicação e valores | Como explica conclusões e que precisão precisa preservar. | H01/H03 | Nomes dos signos e estrutura de síntese. |
| Dificuldades não previstas | Incidentes, retrabalho e oportunidades espontâneas. | H01/H02/H03 | Revisões justificadas de quaisquer artefatos afetados. |

### De quem coletar e estratégia de amostragem

O público ideal inclui pesquisadores, engenheiros, analistas, docentes ou pós-graduandos que já preparem e interpretem simulações ou análises. Gestores técnicos podem contribuir para compreensão da síntese de resultados. Participantes *proxy* são possíveis apenas com justificativa explícita. Uma amostra pequena permite aprofundamento, mas não generalização estatística; quantidade e perfis exatos dependerão do recrutamento futuro.

### Aspectos éticos — A02

- **Participação voluntária:** o entrevistado pode não responder, interromper ou solicitar que uma resposta não seja usada.
- **Consentimento informado:** explicar tema, duração, finalidade, registro, anonimização, uso e descarte dos dados antes de começar.
- **Áudio:** gravação opcional com aceite próprio. Participar sem gravação e apenas com anotações deve ser permitido.
- **Vídeo:** não está previsto nem é necessário para os objetivos definidos.
- **Confidencialidade:** não solicitar projetos confidenciais, nomes de clientes, códigos proprietários ou informações de organizações que identifiquem pessoas.
- **Anonimização:** códigos de participantes `UE01`, `UE02` etc.; `E01`–`E20` permanecem reservados às perguntas do roteiro.
- **Proteção de registros:** acesso restrito à equipe, publicação apenas de achados anonimizados e descarte após a finalidade acadêmica, salvo orientação institucional em contrário.

---

# Parte B — Ferramentas de coleta

Conforme **Identificação de Necessidades — Parte B**, cada integrante escolhe um método, produz um instrumento e define o protocolo de aplicação. As técnicas da equipe são distintas e incluem o questionário requerido.

| ID | Integrante | Técnica | Papel na investigação | Situação |
|---|---|---|---|---|
| I01 | Gabriel | Questionário exploratório | Respostas padronizadas sobre perfil, tarefas, experiência e necessidades. | Elaborado, não aplicado. |
| I02 | João Pedro | Entrevista semiestruturada | Aprofundamento de processos, razões, erros, interpretação e vocabulário. | Elaborado, não aplicado. |

## I01 — Questionário exploratório sobre atividades de simulação e análise

**Autor:** Gabriel Koiama de Rocha Lira — 22.125.067-3  
**Hipóteses:** H01, H02 e H03  
**Situação:** instrumento completo, ainda não aplicado.

### Público, meio e tempo previstos

Público preferencial: pessoas com experiência em simulação, mobilidade, engenharia, experimentação computacional ou análise técnica. Aplicação preferencial em formulário digital sem identificação obrigatória; proxies possíveis com ressalva. **Duração estimada: 5–8 minutos**, a confirmar em piloto.

### Protocolo de aplicação de I01

1. Montar formulário on-line, mantendo o enunciado e as opções documentadas a seguir.
2. Desabilitar coleta automática de e-mail e exigência de login, se o serviço permitir.
3. Revisar termos e testar em dispositivos usuais; fazer piloto de clareza antes de recrutar o público final.
4. Apresentar objetivo, tempo, caráter voluntário, direitos e consentimento.
5. Encerrar imediatamente se o participante não concordar.
6. Permitir preenchimento autônomo sem orientar a resposta.
7. Agradecer e armazenar as respostas em local privado, separando dados brutos da futura síntese anônima.

### Texto de abertura e consentimento

**Questionário sobre atividades de simulação e análise de resultados**

Esta pesquisa integra a disciplina de Interação Humano-Computador da FEI. Queremos compreender como pessoas de áreas técnicas preparam, executam e analisam simulações ou experimentos. Não é uma avaliação do conhecimento do participante. A participação é voluntária, dura aproximadamente 5 a 8 minutos, pode ser interrompida e não exige dados pessoais identificáveis. Respostas eventualmente coletadas serão usadas apenas para fins acadêmicos e divulgadas sem identificação individual.

**Q00 — Consentimento:** concorda voluntariamente em participar segundo as informações acima? **( ) Sim  ( ) Não**. Se “Não”, encerrar o questionário.

### Questionário completo

*Indicação:* questões de escolha múltipla permitem marcar mais de uma opção; “outro” exige campo de texto; as questões abertas são opcionais. As opções de desconhecimento evitam presumir especialização no domínio.

#### Seção 1 — Perfil e experiência

##### Q01. Qual opção melhor descreve sua área de formação, estudo ou atuação?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H01.

- [ ] Mobilidade urbana / transportes
- [ ] Engenharia de tráfego
- [ ] Engenharia em outra área
- [ ] Ciência da Computação / Sistemas de Informação / software
- [ ] Ciência de dados / análise de dados
- [ ] Pesquisa acadêmica
- [ ] Gestão ou coordenação técnica
- [ ] Outra área técnica
- [ ] Nenhuma das anteriores
- [ ] Outro: ____

##### Q02. Qual opção melhor descreve sua experiência com softwares técnicos, simulações ou análise computacional?

**Tipo:** escolha única.  
**Hipótese(s):** H01.

- ( ) Nunca utilizei
- ( ) Já tive contato pontual
- ( ) Utilizo eventualmente
- ( ) Utilizo com frequência
- ( ) Trabalho ou pesquiso diretamente com esse tipo de ferramenta

##### Q03. Quais tipos de ferramentas você já utilizou em atividades técnicas ou acadêmicas?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H01/H02.

- [ ] Planilhas
- [ ] Ferramentas de análise de dados
- [ ] Scripts ou programas próprios
- [ ] Simuladores
- [ ] Dashboards ou ferramentas de BI
- [ ] Softwares de engenharia
- [ ] Ferramentas de mobilidade/tráfego
- [ ] Nunca utilizei ferramentas desse tipo
- [ ] Outro: ____

##### Q04. Caso já tenha utilizado simuladores ou ferramentas especializadas, quais?

**Tipo:** aberta opcional.  
**Hipótese(s):** H01.

**Resposta:** ________________________________________

#### Seção 2 — Preparação e configuração

##### Q05. Em uma atividade que envolve executar uma simulação, análise ou experimento, quais informações você considera importante revisar antes de iniciar?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H02.

- [ ] Cenário ou conjunto de dados
- [ ] Parâmetros configurados
- [ ] Método, algoritmo ou estratégia
- [ ] Condição de entrada ou demanda
- [ ] Seed ou outra condição de reprodutibilidade
- [ ] Duração/horizonte da execução
- [ ] Local de armazenamento dos resultados
- [ ] Versão/configuração do método
- [ ] Normalmente não faço essa verificação
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ____

##### Q06. Qual situação seria mais problemática em uma execução técnica?

**Tipo:** escolha única.  
**Hipótese(s):** H02.

- ( ) Usar parâmetros incorretos
- ( ) Usar cenário ou entrada incorretos
- ( ) Executar método diferente do planejado
- ( ) Não saber quais condições produziram o resultado
- ( ) Descobrir erro somente após processamento
- ( ) Não identificar se execução falhou
- ( ) Não tenho experiência suficiente para responder
- ( ) Outro: ____

##### Q07. Quando existem muitos parâmetros técnicos, qual abordagem costuma ser mais útil para você?

**Tipo:** escolha única.  
**Hipótese(s):** H02.

- ( ) Ver todos ao mesmo tempo
- ( ) Ver primeiro os principais e abrir avançados quando necessário
- ( ) Usar configurações pré-definidas e alterar algumas
- ( ) Depende da atividade
- ( ) Não tenho experiência suficiente para responder
- ( ) Outro: ____

#### Seção 3 — Execução e acompanhamento

##### Q08. Durante uma execução que demora algum tempo, quais informações você considera mais importantes?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H02.

- [ ] Indicação clara de execução ativa
- [ ] Percentual/progresso
- [ ] Tempo decorrido
- [ ] Estimativa restante
- [ ] Cenário/entrada em execução
- [ ] Método/algoritmo ativo
- [ ] Parâmetros principais
- [ ] Mensagens de erro
- [ ] Logs técnicos
- [ ] Opção de cancelar
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ____

##### Q09. Quando uma execução apresenta erro, qual informação é mais importante para você?

**Tipo:** escolha única.  
**Hipótese(s):** H02.

- ( ) Saber apenas que houve erro
- ( ) Saber em qual etapa
- ( ) Entender provável causa
- ( ) Receber orientação de correção
- ( ) Acessar detalhes técnicos
- ( ) Combinação das alternativas
- ( ) Não tenho experiência suficiente para responder
- ( ) Outro: ____

#### Seção 4 — Resultados e comparação

##### Q10. Quando uma execução termina, quais informações você normalmente procura primeiro?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H03.

- [ ] Resultado principal
- [ ] Métricas de desempenho
- [ ] Condições e parâmetros
- [ ] Erros ou alertas
- [ ] Gráficos
- [ ] Dados detalhados
- [ ] Comparação com outra execução
- [ ] Local dos arquivos completos
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ____

##### Q11. Em uma análise de tráfego ou simulação semelhante, quais indicadores você consideraria relevantes?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H03.

- [ ] Tempo médio de espera
- [ ] Tempo médio de viagem
- [ ] Tamanho das filas
- [ ] Throughput / quantidade de veículos processados
- [ ] Veículos que não concluíram
- [ ] Trocas de fase
- [ ] Duração das fases verdes
- [ ] Erros, colisões ou teleports
- [ ] Não conheço suficientemente essas métricas
- [ ] Outro: ____

##### Q12. Quando você precisa comparar diferentes execuções ou alternativas, como costuma realizar essa comparação?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H03.

- [ ] Comparação manual de valores
- [ ] Planilha
- [ ] Gráficos
- [ ] Relatório
- [ ] Script ou análise automatizada
- [ ] Dashboard
- [ ] Ferramenta específica do domínio
- [ ] Não costumo comparar
- [ ] Outro: ____

##### Q13. Quais condições você considera que precisam permanecer identificáveis ao comparar duas execuções?

**Tipo:** múltipla escolha.  
**Hipótese(s):** H02/H03.

- [ ] Cenário
- [ ] Entrada/demanda
- [ ] Parâmetros principais
- [ ] Seed
- [ ] Duração/horizonte
- [ ] Método/algoritmo
- [ ] Versão da configuração
- [ ] Data da execução
- [ ] Não tenho experiência suficiente para responder
- [ ] Outro: ____

##### Q14. Quando precisa consultar uma execução antiga, como normalmente a localiza?

**Tipo:** escolha única.  
**Hipótese(s):** H03.

- ( ) Pasta/estrutura de arquivos
- ( ) Nome do experimento
- ( ) Data
- ( ) Planilha ou registro separado
- ( ) Histórico dentro da ferramenta
- ( ) Busca ou filtros
- ( ) Não costumo consultar execuções antigas
- ( ) Outro: ____

#### Seção 5 — Linguagem e necessidades

##### Q15. Que termos você utilizaria para diferenciar uma execução que mostra visualmente a simulação de outra executada apenas em processamento, sem interface gráfica?

**Tipo:** aberta opcional.  
**Hipótese(s):** H01/H02.

**Resposta:** ________________________________________

##### Q16. Pensando em ferramentas técnicas ou de análise que você já utilizou, qual dificuldade mais atrapalha sua experiência?

**Tipo:** aberta opcional.  
**Hipótese(s):** H01/H02/H03.

**Resposta:** ________________________________________

##### Q17. Existe alguma informação ou recurso que você considera importante em uma ferramenta de configuração, execução e análise e que não apareceu nas perguntas anteriores?

**Tipo:** aberta opcional.  
**Hipótese(s):** H01/H02/H03.

**Resposta:** ________________________________________

### Mensagem de encerramento

Obrigado pela participação. As respostas, caso coletadas, serão utilizadas exclusivamente na atividade acadêmica indicada, com apresentação anonimizada dos resultados.

### Plano de análise — I01

As questões fechadas serão examinadas por frequências absolutas e proporções de alternativas, considerando o número de respostas válidas por questão. Para itens de múltipla marcação, a soma dos percentuais pode ultrapassar 100%, e respostas “não sei” ou “não tenho experiência” não serão interpretadas como rejeição do recurso. Perguntas abertas Q04/Q15/Q16/Q17 serão categorizadas tematicamente após leitura, agrupamento e revisão das respostas.

Não existem percentuais, falas ou categorias observadas a apresentar nesta entrega; eventuais exemplos de tabulação seriam apenas ilustrativos e não foram inseridos como resultado.

| Perguntas | Hipótese | O que podem informar | Artefatos passíveis de revisão |
|---|---|---|---|
| Q01–Q04 | H01 | Formação, experiência e familiaridade. | P01/P02 e contexto de uso. |
| Q05–Q07 | H02 | Preparação e configuração. | PF01, PP02/PP03, T02/T03. |
| Q08–Q09 | H02 | Feedback e recuperação de falhas. | PF02, PP03/PP04, T04/T05. |
| Q10–Q14 | H02/H03 | Resultados, condições comparáveis e histórico. | PF03, PP06/PP07, T06–T08. |
| Q15–Q17 | H01–H03 | Vocabulário e necessidades não antecipadas. | Signos, textos e propostas de V1. |

---

## I02 — Entrevista semiestruturada sobre processos técnicos e interpretação de resultados

**Autor:** João Pedro Lopes Santana Villas Bôas — RA 22.125.065-7  
**Hipóteses:** H01, H02 e H03  
**Situação:** roteiro e protocolo completos, não aplicados.

### Objetivo, público, modalidade e duração

Aprofundar a descrição de atividades e os motivos das escolhas, sem pedir aprovação das telas existentes. Público ideal: profissionais, pesquisadores e estudantes com experiências pertinentes às tarefas. A entrevista pode ser presencial ou por videoconferência; duração planejada **20–30 minutos**, a ajustar em piloto. Será **semiestruturada**, permitindo questões de seguimento neutras como “Pode dar um exemplo?”, “O que aconteceu depois?” e “Por que isso foi importante?”.

### Protocolo de aplicação de I02

1. Revisar o roteiro, preparar anotações e, se necessário, testar microfone e conexão.
2. Informar objetivos, duração, caráter voluntário, anonimização e possibilidade de recusa.
3. Solicitar consentimento para participar e, separadamente, para eventual gravação de áudio; sem aceite de gravação, usar somente anotações.
4. Conduzir aquecimento, blocos principais e encerramento sem sugerir a resposta preferida pela equipe.
5. Obter exemplos concretos e registrar o contexto em que ocorreram; não projetar comportamento de especialistas a partir de um proxy.
6. Após a sessão, revisar anotações, identificar o participante como `UE##`, retirar dados identificáveis e guardar registros brutos em local privado.
7. Consolidar apenas os temas evidenciados e suas limitações, sem confundir fala isolada com consenso.

### Texto de abertura sugerido

Esta entrevista integra uma atividade acadêmica de Interação Humano-Computador da FEI. Procuramos compreender processos de configuração, execução, análise e comparação de resultados em atividades técnicas. Não há respostas certas ou erradas, a participação é voluntária, e você poderá interromper a qualquer momento. As informações serão registradas e analisadas de maneira anonimizada; áudio só será gravado com autorização específica.

### Roteiro completo da entrevista

#### Bloco — Perfil e contexto

##### E01. Você pode descrever brevemente sua área de estudo ou atuação e as principais atividades que realiza?

**Hipótese(s):** H01.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Há quanto tempo realiza essas atividades?
- São acadêmicas, profissionais ou ambas?
- Atua na configuração, execução, análise ou decisão?

##### E02. Você utiliza ou já utilizou softwares técnicos, ferramentas de análise, simuladores ou sistemas que executam algum tipo de processamento?

**Hipótese(s):** H01/H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Quais ferramentas?
- Para quais tarefas?
- O que funciona e o que incomoda?

#### Bloco — Preparação

##### E03. Pense em uma atividade técnica, análise ou experimento que você já realizou. Como normalmente começa esse processo?

**Hipótese(s):** H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- O que define primeiro?
- Utiliza roteiro, arquivo ou checklist?

##### E04. Antes de iniciar uma execução ou processamento, o que você costuma conferir?

**Hipótese(s):** H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Quais erros são mais graves?
- O que sempre verifica?
- Já houve validação automática útil?

##### E05. Quando existem muitos parâmetros ou opções técnicas, como você prefere lidar com eles?

**Hipótese(s):** H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Usa valores padrão?
- Quais raramente altera?
- Quando precisa acessar opções avançadas?

#### Bloco — Execução e feedback

##### E06. Durante um processamento que leva algum tempo, como você costuma saber se tudo está acontecendo corretamente?

**Hipótese(s):** H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- O que observa: estado, progresso, tempo ou logs?
- Qual informação é indispensável?

##### E07. Conte sobre alguma situação em que uma ferramenta apresentou erro ou um processamento não terminou como esperado.

**Hipótese(s):** H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Como percebeu a falha?
- A mensagem ajudou?
- Como se recuperou?

##### E08. Em uma execução longa, em que situação você consideraria importante ter a possibilidade de cancelar?

**Hipótese(s):** H02.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- O cancelamento seria por configuração, erro ou tempo?
- Quais consequências precisa conhecer?

#### Bloco — Resultados

##### E09. Quando uma execução termina, qual costuma ser sua primeira pergunta sobre o resultado?

**Hipótese(s):** H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Que informação procura primeiro?
- Quando busca detalhes?

##### E10. Como você decide se um resultado é confiável o suficiente para ser interpretado?

**Hipótese(s):** H02/H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Precisa consultar parâmetros, erros, reprodutibilidade ou referência?

#### Bloco — Comparação

##### E11. Conte como você normalmente compara duas alternativas, execuções ou resultados.

**Hipótese(s):** H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Usa planilha, gráfico, relatório, script ou comparação manual?

##### E12. Como você decide se duas execuções podem ser comparadas de forma justa?

**Hipótese(s):** H02/H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- O que deve ser igual?
- O que pode variar?
- Como confere isso?

##### E13. Quando existem muitas métricas, como você decide quais realmente importam?

**Hipótese(s):** H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Há métrica principal?
- Prefere síntese antes de detalhes?
- Depende do objetivo?

#### Bloco — Histórico e rastreabilidade

##### E14. Se você precisasse recuperar hoje o resultado de uma análise realizada semanas ou meses atrás, como faria?

**Hipótese(s):** H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Buscaria por nome, data, pasta, planilha ou histórico?
- O que dificulta?

##### E15. Quais informações deveriam permanecer associadas a uma execução para que você consiga entendê-la no futuro?

**Hipótese(s):** H02/H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Que contexto precisaria recuperar para interpretar corretamente?

#### Bloco — Comunicação e linguagem

##### E16. Quando você precisa explicar o resultado de uma análise para outra pessoa, como costuma fazer?

**Hipótese(s):** H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- O público é técnico?
- Usa tabelas, gráficos e síntese?

##### E17. Existem termos utilizados por ferramentas técnicas que você considera difíceis, ambíguos ou excessivamente voltados à implementação?

**Hipótese(s):** H01.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Pode citar exemplos?
- Como os nomearia?

#### Bloco — Necessidades abertas

##### E18. Pensando em todo esse processo, qual é a etapa mais trabalhosa ou sujeita a erro?

**Hipótese(s):** H02/H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Por quê?
- Qual foi o efeito em uma situação real?

##### E19. Se você pudesse melhorar uma única coisa em uma ferramenta usada para configurar, executar e analisar atividades técnicas, o que melhoraria?

**Hipótese(s):** H01/H02/H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Que problema concreto seria resolvido?

##### E20. Existe algo importante sobre esse tipo de atividade que eu não perguntei e que você considera relevante?

**Hipótese(s):** H01/H02/H03.  
**Aprofundamentos possíveis (somente quando pertinentes, sem induzir):**
- Há algo que gostaria de acrescentar?

### Encerramento sugerido

Obrigado pela participação. A equipe utilizará apenas informações pertinentes à atividade acadêmica e publicará sínteses sem identificação pessoal. Se houver áudio autorizado, ele não será publicado automaticamente.

### Plano de análise — I02

1. **Organização:** identificar registros por participante (`UE##`), tarefa e contexto; transcrever somente os trechos necessários quando houver gravação autorizada.
2. **Leitura e codificação:** marcar evidências relacionadas a preparação, parâmetros, erros, feedback, métricas, comparação, histórico, linguagem e comunicação. Permitir novos códigos emergentes, em vez de obrigar todas as falas a categorias previstas.
3. **Agrupamento temático:** relacionar códigos semelhantes, preservando diferenças entre perfis e exemplos contraditórios.
4. **Relação com hipóteses:** comparar indícios com H01–H03 e classificar achados como sustentação limitada, revisão possível, contradição ou insuficiência de evidência, sempre com o contexto da amostra.
5. **Implicações:** propor alterações nos artefatos apenas quando existirem evidências correspondentes e rastreáveis.

Os termos “feedback”, “comparação” e “histórico” designam **categorias previstas para codificação**, não resultados encontrados.

| Perguntas | Hipótese | Tema investigado | Artefatos que poderão ser revisados |
|---|---|---|---|
| E01–E02 | H01 | Perfil e ferramentas. | P01/P02, contexto, linguagem. |
| E03–E05 | H02 | Preparação, configuração, verificações. | PF01, PP01–PP03, T01–T03. |
| E06–E08 | H02 | Execução, feedback, erro, controle. | PF02, PP03–PP05, T04/T05. |
| E09–E10 | H02/H03 | Resultados e confiança na execução. | PF03, PP07, T06. |
| E11–E13 | H02/H03 | Critérios e métodos de comparação. | T07/T08, PP06/PP07 e proposta futura. |
| E14–E15 | H02/H03 | Recuperação e contexto experimental. | PP06 e vínculo execução–resultados. |
| E16–E17 | H01/H03 | Comunicação e termos usados. | Signos e hierarquia dos resultados. |
| E18–E20 | H01–H03 | Dificuldades e necessidades abertas. | Qualquer artefato afetado. |

---

# Consolidação da equipe

## Complementaridade de I01 e I02

| Critério | I01 — Questionário | I02 — Entrevista |
|---|---|---|
| Estrutura | Padronizada | Roteiro adaptável |
| Evidência típica | Distribuição de opções e respostas curtas | Exemplos, motivos e sequência de ações |
| Abrangência | Potencialmente mais respostas em menos tempo | Menos participantes, maior profundidade |
| Principal utilidade | Identificar padrões exploratórios | Explicar razões e contextos |
| Limitação | Pouco aprofundamento | Não permite generalização estatística |
| Situação | Planejado, sem aplicação | Planejado, sem aplicação |

A escolha evita depender de uma única técnica para compreender necessidades. Sua combinação futura não será tratada como validação automática, especialmente se forem usados participantes proxy.

## Critérios para tratar H01–H03 após eventual coleta

- **Sustentada no contexto estudado:** evidências coerentes e adequadas à pergunta de investigação, explicitando o perfil e a amostra.
- **Refinada:** o princípio geral permanece plausível, mas dados exigem ajuste de público, tarefa ou representação.
- **Contrariada/refutada no contexto estudado:** evidência consistente contrária, devidamente descrita; não implica verdade universal.
- **Inconclusiva:** amostra, recrutamento, clareza ou quantidade não permitem decisão responsável.

O estado **atual** continua sendo **aberta** para as três hipóteses, porque não houve aplicação.

## Relação com E1–E6

| Entrega | Contribuição aproveitada na E7 |
|---|---|
| E1 | Hipóteses H01–H03, usuários e lacunas. |
| E2 | Ferramentas profissionais comparáveis e padrões de interface para investigar, não copiar. |
| E3 | Proto-personas P01/P02, contexto e jornada. |
| E4 | C01/C02: preparação/execução e interpretação/comparação. |
| E5 | T01–T08 e modelos HTA/GOMS/CTT. |
| E6 | V0, PF01–PF03, PP01–PP07, observações O01–O10 e decisões propostas V0→V1. |

## Utilização futura dos dados

Caso os instrumentos sejam aplicados, registrar perfil real e consentimento, analisar limitações, revisar a rastreabilidade e justificar eventuais mudanças nas personas, cenários, tarefas, signos, MoLIC, protótipo e planejamento da avaliação. Não transformar uma sugestão de interface em requisito confirmado sem evidência.

## Síntese

A equipe elaborou o **I01** (questionário, Gabriel) e o **I02** (entrevista semiestruturada, João), ambos com procedimentos, conteúdo integral, públicos previstos, cuidados éticos e plano de análise. As perguntas investigam usuário prioritário, preparação/execução, feedback, métricas, comparabilidade, histórico e vocabulário, sem presumir funções inexistentes na V0. A comparação automática permanece apenas como possibilidade de evolução. Como os instrumentos não foram aplicados, **não há dados empíricos, participantes nem validação de H01–H03 a relatar**.

## Checklist

- [x] Hipóteses e dúvidas herdadas de E1–E6 explicitadas.
- [x] Dados e perfis especificados individualmente.
- [x] Uma técnica por integrante; técnicas diferentes; questionário incluído.
- [x] I01 e I02 documentados integralmente e com instruções de aplicação.
- [x] Perguntas associadas a hipóteses e futuras decisões de design.
- [x] Procedimentos éticos, privacidade, consentimento e possibilidade de desistência previstos.
- [x] Proxies e suas limitações considerados.
- [x] Plano de análise quantitativa simples e qualitativa previsto.
- [x] Nenhuma aplicação, resposta, observação ou validação fictícia declarada.
- [x] Comparação automática não foi atribuída à V0.

## Referências

- BARBOSA, Simone D. J.; SILVA, Bruno S. *Interação Humano-Computador*. Elsevier/Campus, 2010.
- CENTRO UNIVERSITÁRIO FEI. *CC8122 — Identificação de Necessidades dos Usuários e Requisitos de IHC — Parte A e Parte B*. Materiais de aula, 2026/2.
- Entregas 1–6 e [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md) deste projeto.
