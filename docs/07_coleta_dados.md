# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 20/10/2026  
**Status:** 🟨 em andamento  
**Responsabilidade:** soluções individuais + técnicas distintas; questionário entre as técnicas

## Objetivo da atividade

Planejar os dados necessários para compreender melhor os usuários, suas atividades, necessidades e requisitos de IHC, selecionar técnicas de coleta coerentes com as dúvidas existentes no projeto e produzir instrumentos que possam ser aplicados de forma reproduzível.

Nesta entrega, os instrumentos são **planejados e documentados para eventual aplicação**. Não são apresentados resultados empíricos fictícios e nenhuma hipótese é considerada validada apenas pela elaboração do questionário ou da entrevista.

O projeto já possui hipóteses sobre o usuário prioritário, a organização do fluxo de trabalho e a forma de apresentar os resultados. A Entrega 7 procura transformar essas hipóteses em perguntas de investigação que possam futuramente ser respondidas com evidências.

---

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

| ID | Hipótese/lacuna | Evidência atual | Decisão que depende da resposta | Prioridade |
|---|---|---|---|---|
| H01 | Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface. | Entregas 2 e 3 reforçaram a plausibilidade do perfil por meio da análise de ferramentas profissionais e da construção das proto-personas P01 e P02. A Entrega 6 relacionou o protótipo V0 a tarefas coerentes com esse perfil, mas ainda não existe validação direta com usuários reais. | Definição do público prioritário, vocabulário utilizado, grau de detalhamento técnico e características das personas. | alta |
| H02 | Organizar a interação em definição do cenário, configuração, execução/acompanhamento e análise facilita a realização dos experimentos. | Entregas 3–5 detalharam a jornada, cenários e tarefas. A Entrega 6 materializou essa hipótese nos fluxos PF01 — Preparar experimento, PF02 — Executar e acompanhar e PF03 — Analisar e comparar. | Organização do fluxo principal, agrupamento das configurações, feedback durante a execução e quantidade de informações apresentadas em cada etapa. | alta |
| H03 | Uma apresentação consolidada e comparativa das métricas facilita a interpretação do desempenho das estratégias. | Entregas 2–5 indicaram a necessidade de relacionar métricas ao contexto experimental e verificar comparabilidade. Na Entrega 6, PP06 e PP07 representam resultados e comparação, mas a adequação dessa forma de apresentação ainda não foi investigada com usuários. | Seleção e hierarquia das métricas, forma de comparação, necessidade de histórico, gráficos, síntese ou detalhamento adicional. | alta |

---

# Parte A — necessidades e requisitos de IHC

> **Responsabilidade:** solução individual por integrante.

---

## A01 — Gabriel Koiama de Rocha Lira

**Autor(a):** Gabriel Koiama de Rocha Lira — 22.125.067-3

### Objetivo da investigação individual

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

### Que dados coletar?

A coleta foi estruturada a partir das cinco categorias trabalhadas na disciplina: informações sobre o próprio usuário, relação com tecnologia, conhecimento do domínio, tarefas e motivações/valores.

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
| Tarefas | Informações consultadas primeiro após uma execução. | H03 | Permite identificar quais resultados merecem maior destaque. | Hierarquia de PP06 e futuras telas de resultados. |
| Tarefas | Forma atual de comparar diferentes execuções ou alternativas. | H03 | Permite compreender se a comparação acontece por planilhas, gráficos, scripts, relatórios ou outro processo. | Estrutura de PP07 e fluxo PF03. |
| Tarefas | Condições consideradas necessárias para que duas execuções sejam comparáveis. | H02, H03 | Comparações sem equivalência podem produzir conclusões inadequadas. | Validação de compatibilidade e contexto exibido. |
| Tarefas | Forma utilizada para localizar resultados ou execuções anteriores. | H03 | Permite investigar se existe necessidade real de histórico, busca ou filtros. | Decisão sobre histórico e mecanismos de recuperação de execuções. |
| Motivações/valores | Prioridade entre rapidez, rastreabilidade, controle detalhado e facilidade de interpretação. | H02, H03 | Usuários diferentes podem valorizar controle técnico ou síntese de maneira distinta. | Equilíbrio entre detalhamento e simplicidade. |
| Motivações/valores | Principal dificuldade percebida ao trabalhar com experimentos ou análises semelhantes. | H01, H02, H03 | Pergunta exploratória pode revelar necessidades não antecipadas pela equipe. | Possível revisão de tarefas, fluxos, signos e protótipo. |

### Minimização dos dados

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

### De quem coletar?

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Pesquisador ou profissional relacionado à mobilidade, tráfego ou simulação | Possuir experiência acadêmica ou profissional com estudos, simulações, análise de mobilidade ou experimentos semelhantes. | Perfil mais próximo de P01 — Marina Ribeiro. |
| Analista, engenheiro ou pesquisador que trabalhe com ferramentas técnicas ou análise experimental | Realizar configuração, execução ou interpretação de processos computacionais com parâmetros e resultados. | Pode fornecer evidências sobre H01 e H02 mesmo quando não utiliza exatamente o mesmo simulador do TCC. |
| Gestor/coordenador que consulte resultados técnicos | Utilizar resultados consolidados de análises ou estudos para apoiar decisões. | Aproxima-se de P02 — Carlos Mendes e pode contribuir principalmente para H03. |
| Participante proxy com experiência acadêmica em computação, engenharia, simulação ou análise de dados | Possuir familiaridade com experimentação ou ferramentas técnicas, mesmo sem atuação profissional em mobilidade. | Alternativa metodológica quando o acesso ao público especializado for inviável. Deve ser identificada explicitamente como proxy e não tratada como equivalente ao usuário final. |

### Limitação de recrutamento

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

# Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**.

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

# Como os dados do I01 seriam analisados

A análise deverá combinar resultados quantitativos simples das perguntas fechadas com categorização qualitativa das respostas abertas.

Não há necessidade de inferência estatística complexa, especialmente se a amostra for pequena ou composta por participantes proxy.

## Perguntas fechadas

Serão calculadas:

- frequências absolutas;
- proporção de participantes por alternativa;
- alternativas predominantes;
- padrões de coocorrência quando forem relevantes.

Exemplo:

```text
Q08 — informações durante execução

6 participantes marcaram progresso
5 marcaram método ativo
5 marcaram mensagens de erro
2 marcaram logs completos
```

Esse tipo de resultado poderá orientar a hierarquia das informações apresentadas.

---

## Perguntas abertas

As respostas de Q04, Q15, Q16 e Q17 serão analisadas por **codificação temática simples**.

Procedimento:

1. ler todas as respostas;
2. identificar ideias recorrentes;
3. criar categorias;
4. agrupar respostas semelhantes;
5. registrar exemplos anonimizados;
6. relacionar as categorias às hipóteses H01, H02 ou H03.

Exemplo hipotético de categorias:

```text
dificuldade com excesso de parâmetros
falta de feedback durante processamento
problemas para localizar resultados antigos
terminologia excessivamente técnica
necessidade de comparação
```

Essas categorias somente deverão ser registradas como achados se aparecerem efetivamente nos dados coletados.

---

## Relação pergunta → hipótese → decisão

| Perguntas | Hipótese principal | Possível interpretação futura | Artefatos que podem ser revisados |
|---|---|---|---|
| Q01–Q04 | H01 | Perfil e experiência dos participantes são ou não compatíveis com P01/P02. | Personas, contexto de uso, terminologia. |
| Q05–Q07 | H02 | Forma como participantes preparam e verificam configurações. | PF01, PP02, PP03, T02/T03. |
| Q08–Q09 | H02 | Informações necessárias durante processamento e recuperação de erro. | PF02, PP03, PP04, T04/T05. |
| Q10–Q14 | H03 | Como resultados são consultados, comparados e recuperados. | PF03, PP06, PP07, T06–T08. |
| Q15 | H01/H02 | Vocabulário utilizado para modos de execução. | Signos da Entrega 9 e rótulos futuros. |
| Q16–Q17 | H01/H02/H03 | Necessidades e dificuldades não antecipadas pela equipe. | Qualquer artefato afetado pela evidência. |

---

## Critérios para atualização das hipóteses

Após eventual aplicação, as hipóteses não deverão ser classificadas apenas como “verdadeiras” ou “falsas”.

Poderão assumir:

### Sustentada

Quando as respostas obtidas forem coerentes com a hipótese e não apresentarem evidência relevante em sentido contrário dentro da amostra analisada.

### Refinada

Quando a hipótese geral permanecer plausível, mas os dados indicarem mudanças importantes.

Exemplo:

> P01 continua plausível, mas os participantes valorizam configurações pré-definidas mais do que exposição direta de todos os parâmetros.

### Refutada

Quando as evidências obtidas forem incompatíveis com a hipótese dentro da amostra investigada.

### Inconclusiva

Quando a quantidade ou perfil dos participantes não permitir uma conclusão responsável.

> Participantes proxy não devem ser utilizados para afirmar que necessidades específicas de profissionais especializados foram definitivamente validadas.

---

# A02 — João Pedro Lopes Santana Villas Bôas

**Autor(a):** João Pedro Lopes Santana Villas Bôas — 22.125.065-7

> **PENDENTE — contribuição individual do integrante.**

A Parte A de João deverá identificar seus próprios dados prioritários, público e aspectos éticos, mantendo coerência com H01, H02 e H03 sem simplesmente duplicar a análise de Gabriel.

---

# Instrumento I02 — Entrevista semiestruturada

**Autor(a):** João Pedro Lopes Santana Villas Bôas — 22.125.065-7  
**Técnica prevista:** entrevista semiestruturada

> **PENDENTE — instrumento de responsabilidade de João.**

A entrevista deverá complementar o questionário de Gabriel buscando maior profundidade sobre atividades, decisões, dificuldades, vocabulário e comparação de resultados.

As duas técnicas não devem ser cópias uma da outra: o questionário busca maior estrutura e amplitude, enquanto a entrevista deverá explorar exemplos concretos, justificativas e experiências em maior profundidade.

---

# Síntese parcial

A contribuição de Gabriel estrutura uma investigação voltada às três hipóteses prioritárias do projeto.

O questionário foi elaborado para investigar:

- **H01:** quem são os potenciais usuários, qual sua experiência e quais ferramentas e termos utilizam;
- **H02:** como atividades de configuração e execução são realizadas e quais informações, validações e feedbacks são considerados importantes;
- **H03:** como resultados são consultados, comparados e recuperados.

O instrumento evita pressupor que recursos como dashboard, histórico ou filtros sejam obrigatórios. Em vez disso, procura investigar processos e necessidades existentes para que futuras decisões de design possam ser justificadas.

A elaboração do instrumento **não valida as hipóteses**. Caso seja realizada uma aplicação futura, somente os dados efetivamente obtidos poderão sustentar, refinar ou refutar H01, H02 e H03.

A síntese definitiva da Entrega 7 deverá ser consolidada após a inclusão da Parte A e do Instrumento I02 de João.

---

# Checklist

## Situação da contribuição de Gabriel

- [x] Hipóteses/lacunas prioritárias da Entrega 1 foram revisitadas.
- [x] A coleta investiga a plausibilidade do usuário, das tarefas e do contexto adotado.
- [x] Perguntas não pressupõem que dashboard, CRUD, filtros ou relatórios sejam necessários.
- [x] Cada dado a coletar responde uma dúvida concreta do projeto ou possui consequência de design identificável.
- [x] A Parte A de Gabriel identifica dados e perfis de coleta de forma específica.
- [x] Aspectos éticos foram contextualizados para o projeto.
- [x] O questionário possui objetivo, público, procedimento e conteúdo integral.
- [x] Perguntas evitam indução e coletam apenas dados necessários.
- [x] Está definido como os dados seriam analisados e utilizados no design.
- [x] O instrumento distingue público especializado e participantes proxy.
- [x] Nenhum resultado de pesquisa foi inventado.
- [x] A elaboração do instrumento não foi tratada como validação de H01, H02 ou H03.

## Situação da entrega da equipe

- [ ] Há uma técnica completa por integrante e técnicas distintas.
- [x] Questionário está incluído entre as técnicas.
- [ ] Parte A de João foi concluída.
- [ ] Instrumento I02 de João foi concluído.
- [ ] Síntese final da equipe foi consolidada.

---

# Referências

- BARBOSA, Simone D. J.; SILVA, Bruno S. **Interação Humano-Computador**. Elsevier/Campus, 2010.
- CENTRO UNIVERSITÁRIO FEI. **CC8122 — Identificação de Necessidades dos Usuários e Requisitos de IHC — Parte A**. Material de aula, 2026/2.
- CENTRO UNIVERSITÁRIO FEI. **CC8122 — Identificação de Necessidades dos Usuários e Requisitos de IHC — Parte B**. Material de aula, 2026/2.
- Entrega 1 — Conhecendo o projeto, o usuário e o problema.
- Entrega 3 — Personas, empatia, contexto e jornada.
- Entrega 4 — Cenários de análise/problema.
- Entrega 5 — Análise de tarefas: HTA, GOMS e CTT.
- Entrega 6 — Prototipação em papel / protótipo digital V0.
- Matriz de rastreabilidade de IHC do projeto.
