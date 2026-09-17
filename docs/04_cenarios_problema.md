# Entrega 4 — Cenários de análise/problema

**Data:** {{dd/mm/aaaa}}  
**Status:** ⬜ não iniciada  
**Responsabilidade:** 1 solução completa por integrante

## Objetivo da atividade

Descrever situações atuais em que o usuário tenta alcançar um objetivo e encontra dificuldades. O cenário de análise/problema deve tornar visível **o contexto, os atores, as ações e as rupturas**, sem antecipar a interface que será projetada.

> **Regra central:** cenário de problema é a “história do problema”. Se o texto já diz “o sistema mostra”, “o aplicativo resolve” ou descreve botões/telas futuras, provavelmente está misturando problema com solução.

Sempre que possível, o cenário deve aprofundar uma **situação concreta já registrada na Entrega 1**.

### Quando o TCC não possuía interface

O cenário continua sendo uma história de **problema/atividade humana**, não uma história do futuro sistema. Descreva como o profissional realiza hoje uma atividade semelhante ou como lida atualmente com dados, resultados, configurações, logs, decisões e limitações que o tema do TCC pretende apoiar.

Exemplo: em vez de “o DBA abre o novo dashboard e executa o algoritmo”, descreva “o DBA precisa investigar uma consulta lenta, reúne informações em ferramentas distintas, compara planos manualmente e tem dificuldade para estimar o impacto de uma mudança”.

A interface da disciplina aparecerá somente depois, nos cenários de interação.

Se o integrante escolher um novo problema/situação, explique por que ele passou a ser relevante e indique a evidência que motivou sua inclusão.

## Cenário C01 — Preparação e execução de experimentos sob condições comparáveis

**Autor(a):** Gabriel Koiama de Rocha Lira — 22.125.067-3  
**Persona(s) relacionada(s):** P01 — Marina Ribeiro  
**Necessidade relacionada:** R02 — definir corretamente as condições da simulação antes da execução; relacionada também a R01, R03 e R04  
**Situação concreta da Entrega 1 relacionada:** Entrega 1 — Seção 4.5, situação em que um pesquisador precisa comparar diferentes estratégias de controle semafórico em uma interseção com demanda desbalanceada  
**Hipóteses ainda presentes:** H01, H02

### 1. Cenário inicial

Marina Ribeiro é pesquisadora e analista de mobilidade e está realizando um estudo experimental para comparar o comportamento de diferentes estratégias de controle semafórico em uma interseção com demanda desbalanceada. Seu objetivo é executar o controle de tempo fixo, o Max Pressure convencional e o método híbrido Max Pressure + actuated em condições suficientemente equivalentes para que os resultados obtidos posteriormente possam ser comparados de forma válida.

Antes de iniciar cada experimento, Marina precisa definir ou conferir o cenário de tráfego, as condições de demanda e os parâmetros relevantes da simulação. Em seguida, precisa selecionar a estratégia de controle correspondente àquela execução. Como as estratégias são avaliadas separadamente, ela repete esse processo para cada método que deseja estudar, procurando alterar apenas aquilo que faz parte da comparação e preservar as demais condições experimentais.

Atualmente, essa atividade depende da manipulação das configurações técnicas do ambiente experimental e da conferência das informações utilizadas em cada execução. Marina precisa acompanhar quais condições foram utilizadas, qual estratégia está sendo executada e se a simulação foi concluída de forma adequada.

Esse processo exige atenção porque uma alteração não percebida em uma condição que deveria permanecer equivalente pode comprometer a comparação. Também existe o risco de Marina perceber uma configuração inadequada somente depois de executar a simulação, o que pode exigir que o experimento seja realizado novamente.

Como o estudo envolve diferentes estratégias e pode envolver várias execuções, a dificuldade não está apenas em iniciar uma simulação. Marina precisa garantir que cada execução realmente corresponda à condição experimental planejada e que seja possível reconhecer posteriormente em quais condições cada resultado foi produzido. Caso isso não aconteça, a comparação entre os métodos pode deixar de representar corretamente o comportamento das estratégias avaliadas.

### 2. Questões de refinamento

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | **Exploratória — Por que?** Por que as condições comuns do experimento precisam permanecer equivalentes entre as diferentes estratégias? | Esclarecer a consequência científica de alterar mais de uma condição ao mesmo tempo e justificar por que a comparabilidade é central para o cenário. | TCC1 — estratégia de validação; Entrega 1 — Seções 4.4 e 4.5. |
| Q2 | **Exploratória — O que é?** Quais informações caracterizam uma condição experimental e precisam ser conhecidas por Marina antes de considerar duas execuções comparáveis? | Identificar os dados que fazem parte da atividade e que precisam ser considerados durante a preparação dos experimentos. | TCC1 — metodologia e protocolo experimental; Entrega 1 — Seções 4.1 e 4.3. |
| Q3 | **Exploratória — Como?** Como Marina verifica atualmente se o cenário, a demanda e os parâmetros relevantes correspondem às condições que pretendia utilizar? | O cenário inicial afirma que a configuração precisa ser conferida, mas ainda não detalha como essa verificação é realizada na prática. | Observação do processo utilizado pela própria equipe no ambiente experimental e consulta à documentação técnica do experimento. |
| Q4 | **Exploratória — Como?** Como Marina identifica qual estratégia está associada a uma determinada execução e aos resultados produzidos por ela? | Revelar como é mantida a relação entre configuração, execução e resultado, necessária para a análise posterior. | TCC1 — metodologia; Entrega 1 — Seções 4.1 e 4.3; observação do processo experimental da equipe. |
| Q5 | **Exploratória — Como?** Como Marina determina se uma execução terminou de maneira adequada ou apresentou algum problema que comprometa seu uso posterior? | O cenário inicial menciona acompanhamento da execução, mas ainda não explica quais informações são usadas para avaliar seu término. | Observação do ambiente experimental, registros produzidos pela simulação e consulta à equipe técnica. |
| Q6 | **Exploratória — Por que?** O que acontece quando uma diferença de configuração é descoberta somente depois da conclusão de uma execução? | Aprofundar as consequências da ruptura e compreender o impacto de erros tardios sobre tempo, retrabalho e validade experimental. | Entrega 1 — Seção 4.4; experiência da equipe durante a realização dos experimentos. |
| Q7 | **Exploratória — O que é?** Quais informações de uma execução precisam permanecer disponíveis para que Marina consiga posteriormente reconhecer em quais condições o resultado foi produzido? | Determinar quais informações são necessárias para preservar a rastreabilidade experimental sem ainda definir como elas serão apresentadas em uma futura interface. | TCC1 — estratégia de validação e métricas; Entrega 1 — Seções 4.3 e 5.5. |
| Q8 | **Verificação** Uma execução pode ser considerada adequada para comparação quando Marina não consegue confirmar as condições em que ela foi realizada? | Verificar se a rastreabilidade das condições é realmente parte necessária do objetivo da atividade. | Discussão com a equipe, orientador e posteriormente com usuários ou especialistas do perfil representado por P01. |

### 3. Cenário refinado

Marina Ribeiro é pesquisadora e analista de mobilidade e está realizando um estudo experimental para comparar o comportamento do controle de tempo fixo, do Max Pressure convencional e do método híbrido Max Pressure + actuated em uma interseção com demanda desbalanceada.

Seu objetivo não é apenas executar os três métodos, mas produzir experimentos que possam ser comparados de maneira válida. **[NOVO: Para que essa comparação faça sentido, Marina precisa distinguir aquilo que deve permanecer comum entre as execuções das características que são modificadas propositalmente para avaliar cada estratégia.]**

Antes de cada execução, Marina define ou confere o cenário de tráfego, as condições de demanda e os parâmetros relevantes da simulação. Depois, identifica a estratégia que será utilizada naquela execução. **[NOVO: Essas informações caracterizam a condição experimental e precisam ser conhecidas antes que Marina possa considerar a execução adequada para comparação com as demais.]**

A atividade é repetida para cada estratégia avaliada. Como o ambiente experimental depende de configurações técnicas, Marina precisa conferir as condições utilizadas ao preparar cada execução e acompanhar seu andamento. **[NOVO: Além de reconhecer qual estratégia está sendo executada, ela precisa conseguir relacionar a execução às condições que a originaram e determinar se ela foi concluída de maneira adequada antes de utilizar seus resultados.]**

Durante esse processo podem ocorrer rupturas. Um parâmetro que deveria permanecer equivalente pode ser alterado sem que Marina perceba imediatamente, uma execução pode não corresponder às condições que ela pretendia avaliar ou a relação entre a configuração utilizada e o resultado obtido pode se tornar difícil de reconstruir posteriormente.

**[NOVO: Quando uma inconsistência é identificada somente depois da execução, Marina precisa verificar se aquele resultado ainda pode ser utilizado. Caso a diferença comprometa a equivalência experimental, a execução pode precisar ser descartada e realizada novamente, produzindo retrabalho e atrasando a análise.]**

Esse risco cresce à medida que diferentes estratégias e condições precisam ser avaliadas. Marina precisa lembrar e conferir várias informações para determinar se as execuções são realmente comparáveis. **[NOVO: Por isso, informações suficientes sobre cenário, demanda, parâmetros relevantes, estratégia executada e identificação da execução precisam permanecer associadas ao experimento para que sua origem possa ser reconhecida posteriormente.]**

Caso Marina compare resultados produzidos sob condições que não eram equivalentes, poderá atribuir à estratégia de controle uma diferença que, na realidade, foi causada pela configuração experimental. Nesse caso, o problema não afeta diretamente uma interseção real, pois o trabalho ocorre em simulação, mas pode comprometer a validade do estudo e levar a conclusões inadequadas sobre o comportamento dos métodos avaliados.

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | P01 — Marina Ribeiro, pesquisadora/analista de mobilidade responsável por preparar, executar e posteriormente analisar os experimentos. A equipe técnica pode fornecer informações sobre o funcionamento do ambiente quando necessário, mas Marina é a atriz principal do cenário. |
| Objetivo(s) | Executar diferentes estratégias de controle semafórico sob condições comparáveis e produzir resultados cuja origem experimental possa ser reconhecida posteriormente. |
| Contexto | Estudo experimental de controle semafórico realizado em ambiente de simulação, utilizando uma interseção com demanda desbalanceada e comparando tempo fixo, Max Pressure e Max Pressure + actuated. |
| Recursos/informações | Cenário de tráfego, condições de demanda, parâmetros do experimento, estratégia de controle, informações sobre a execução e registros/resultados produzidos pelo ambiente experimental. |
| Ações | Definir ou conferir o cenário; verificar condições e parâmetros; identificar a estratégia; preparar e iniciar a execução; acompanhar seu andamento; verificar se a execução corresponde ao planejado; preservar a relação entre condições, execução e resultado. |
| Problemas/rupturas | Configuração diferente daquela planejada; alteração não percebida de uma condição que deveria permanecer equivalente; dificuldade de confirmar quais condições foram utilizadas; identificação tardia de erros; dificuldade de relacionar uma execução às condições que a produziram. |
| Consequências | Necessidade de repetir experimentos, aumento de retrabalho, atraso na análise, perda da comparabilidade entre execuções e possibilidade de conclusões experimentais inadequadas sobre as estratégias avaliadas. |

### 5. Implicações para as próximas entregas

O cenário indica que as atividades relacionadas à preparação e execução dos experimentos merecem ser aprofundadas na análise de tarefas. Em especial, devem ser analisadas as tarefas T01 — definir ou selecionar a malha viária, T02 — configurar os parâmetros do experimento, T03 — selecionar a estratégia de controle, T04 — iniciar uma simulação e T05 — verificar o estado da execução.

As próximas entregas deverão investigar como essas tarefas são realizadas atualmente, quais decisões o usuário precisa tomar, quais informações precisam estar disponíveis em cada etapa, quais condições precisam ser verificadas antes de uma execução e como o usuário reconhece que um experimento foi concluído corretamente.

Também permanecem questões que ainda precisam de evidência direta, principalmente: quais etapas do processo atual são mais trabalhosas para pesquisadores ou analistas externos à equipe; quais parâmetros eles consideram mais difíceis de compreender ou conferir; como identificam erros durante uma execução; e quais informações consideram indispensáveis para reproduzir ou revisar um experimento.

Essas informações deverão orientar a análise de tarefas e as futuras decisões de interação, mas o cenário atual não define ainda telas, controles, organização visual ou qualquer solução específica para os problemas identificados.

> Repita para C02, C03... com autoria individual.

## Checklist

- [ ] Há um cenário completo por integrante.
- [ ] Cada cenário tem título, ator, objetivo, contexto e problema.
- [ ] O cenário possui origem rastreável na Entrega 1 ou justifica claramente a inclusão de uma nova situação.
- [ ] O texto descreve a situação atual, sem antecipar a solução.
- [ ] Para TCC sem interface original, o cenário descreve uma prática humana plausível relacionada à contribuição técnica, e não “a falta de uma tela”.
- [ ] Questões de refinamento acrescentam informação nova.
- [ ] O refinamento mostra claramente o que foi adicionado/alterado.
- [ ] Cenários são diferentes o suficiente para cobrir objetivos/problemas relevantes.
- [ ] Cada cenário está ligado a persona/necessidade na matriz de rastreabilidade.
