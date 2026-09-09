# Entrega 3 — Personas, mapa de empatia, contexto de uso e jornada

**Data:** {{09/09/2026}}  
**Status:** 🟨 em andamento 
**Responsabilidade:** 1 persona por integrante; 1 mapa de empatia, 1 contexto de uso consolidado e 1 jornada por equipe (salvo orientação diferente do docente).

## Objetivo da atividade

Representar grupos de usuários de forma útil para decisões de design. Persona não é personagem decorativo: suas características devem alterar requisitos, prioridades, linguagem, fluxos ou critérios de avaliação.

## Atenção a projetos técnicos

Em TCCs sem interface original, a persona pode representar um **profissional que se apropria da contribuição técnica**: DBA, analista, cientista de dados, administrador, pesquisador, técnico, operador, gestor ou especialista de domínio.

Não escolha um perfil apenas porque “parece combinar” com a tecnologia. Explique **qual objetivo esse perfil teria e qual parte da contribuição do TCC produziria valor para ele**. Se ainda for hipótese, mantenha como hipótese/proto-persona a validar.

Também considere papéis diferentes quando houver tarefas distintas, por exemplo:

- operador que executa análises;
- administrador que configura e gerencia permissões;
- especialista que interpreta resultados;
- gestor que consulta relatórios e decide;
- auditor que revisa histórico.

## Entradas da Entrega 1

Antes de criar personas, retome os tipos de usuários, características relevantes, objetivos e hipóteses registradas na Entrega 1. A persona **não deve transformar uma hipótese inicial em fato por meio de uma história fictícia**.

| Item da Entrega 1 | Status inicial | Evidência disponível agora | Como será tratado nesta entrega |
|---|---|---|---|
| H01 — Pesquisadores ou analistas de mobilidade representam adequadamente o usuário prioritário da interface | H | A Entrega 2 identificou Aimsun Next e PTV Vissim como ferramentas profissionais que materializam atividades semelhantes de configuração, execução e análise de simulações, mas isso ainda não constitui validação direta com usuários. | incorporar P01 como proto-persona primária e manter H01 como hipótese a validar |
| H02 — A organização da interação em definição da malha, configuração/execução e análise pode facilitar a realização dos experimentos | H | A Entrega 2 encontrou padrões de configuração, execução, feedback e análise em ferramentas profissionais, mas não houve avaliação com usuários. | utilizar como base das necessidades de P01 sem considerar H02 validada |
| H03 — Uma apresentação comparativa das métricas pode facilitar a interpretação dos métodos | H | Aimsun Next e PTV Vissim utilizam resumos, listas, gráficos e formas de comparação de resultados. | incorporar como hipótese nas necessidades de P01 e P02 e manter aberta para validação |
| Pesquisador ou analista de mobilidade urbana | H | Permanece como usuário prioritário do projeto e possui relação com T01–T08. | representar por P01 |
| Gestor de mobilidade | H | Foi identificado na Entrega 1 como stakeholder que poderia consultar resultados consolidados para apoiar avaliações e decisões. | representar por P02 como persona secundária, sem alterar o usuário prioritário |
| Uso principalmente em computadores desktop/notebooks | H | O escopo envolve mapas, parâmetros, execução e resultados; não houve validação direta com usuários. | manter como hipótese no contexto de uso |

## 1. Personas

### Persona P01 — Marina Ribeiro

**Autor(a):** Gabriel Koiama de Rocha Lira — 22.125.067-3  
**Tipo:** primária  
**Base de evidências:** proto-persona a validar / combinação entre TCC1, Entrega 1 e análise documental da Entrega 2  
**Hipóteses da Entrega 1 relacionadas:** H01, H02, H03

![Persona P01](../assets/03_personas/persona_p01.svg)

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | [H] Profissional adulto atuando em ambiente acadêmico, laboratorial ou técnico. A idade específica não é considerada determinante para a interação. |
| Ocupação/papel | [H] Pesquisadora ou analista de mobilidade responsável por preparar, executar e analisar estudos de controle de tráfego. |
| Conhecimento do domínio | [H] Possui conhecimento de tráfego, métricas de desempenho e experimentação, mas não necessariamente conhece a implementação interna do algoritmo híbrido. |
| Experiência tecnológica | [H] Está habituada ao uso de computadores e ferramentas técnicas de análise ou simulação, mas seu nível de experiência com SUMO e outras ferramentas específicas ainda precisa ser validado. |
| Objetivos | [H] Configurar experimentos corretamente, executar diferentes estratégias de controle e comparar seus resultados sob condições equivalentes. |
| Necessidades | [H] Identificar claramente cenário, parâmetros e estratégia utilizados; acompanhar o estado da execução; acessar métricas relevantes; relacionar cada resultado à configuração que o produziu. |
| Dores/frustrações | [H] Risco de configurar experimentos de forma inconsistente, perder a relação entre configuração e resultado, lidar com excesso de parâmetros técnicos e ter dificuldade para comparar múltiplas execuções. |
| Motivadores | [H] Obter resultados reproduzíveis e comparáveis e compreender de forma confiável o comportamento das diferentes estratégias de controle. |
| Restrições/acessibilidade | [?] Ainda não existem evidências sobre necessidades específicas de acessibilidade. A quantidade de informações e o espaço disponível em tela podem influenciar o uso. |
| Ambiente típico de uso | [H] Computador desktop ou notebook em ambiente acadêmico, laboratorial ou profissional. |
| Comportamentos relevantes | [H] Realiza múltiplos experimentos, altera condições de cenário ou demanda, verifica resultados e compara estratégias antes de concluir uma análise. |

**Decisões de design influenciadas por P01:**

- manter cenário, estratégia e principais parâmetros claramente identificados durante o experimento;
- agrupar configurações relacionadas para evitar excesso de informações simultâneas;
- validar parâmetros importantes antes da execução;
- apresentar feedback claro sobre o estado da simulação;
- manter os resultados vinculados à configuração e estratégia que os originaram;
- permitir comparação direta entre tempo fixo, Max Pressure e Max Pressure + actuated;
- preservar acesso às métricas detalhadas sem exigir contato com detalhes internos do código.
> Repita para P02, P03... Cada integrante deve produzir ao menos uma persona.


### Persona P02 — Carlos Mendes

**Autor(a):** João Pedro Lopes Santana Villas Bôas — 22.125.065-7  
**Tipo:** secundária  
**Base de evidências:** proto-persona a validar, construída a partir do TCC1, da Entrega 1 e da análise documental realizada na Entrega 2  
**Hipóteses da Entrega 1 relacionadas:** H03

![Persona P02](../assets/03_personas/persona_p02.svg)

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | [H] Profissional adulto atuando em contexto organizacional relacionado à mobilidade urbana. A idade específica não é considerada determinante para a interação. |
| Ocupação/papel | [H] Gestor ou coordenador de mobilidade que consulta resultados de estudos e simulações para apoiar avaliações técnicas e decisões. |
| Conhecimento do domínio | [H] Possui conhecimento sobre mobilidade urbana, indicadores de tráfego e interpretação de resultados, mas não necessariamente conhece os detalhes internos de implementação dos algoritmos avaliados. |
| Experiência tecnológica | [H] Utiliza computadores, relatórios, planilhas, dashboards ou ferramentas de análise no contexto profissional, mas sua familiaridade com simuladores específicos ainda precisa ser investigada. |
| Objetivos | [H] Compreender o desempenho das diferentes estratégias de controle, identificar diferenças relevantes entre os resultados e utilizar essas informações para apoiar avaliações ou decisões. |
| Necessidades | [H] Visualizar as principais métricas de forma consolidada; compreender quais condições produziram cada resultado; comparar estratégias ou cenários; e acessar detalhes adicionais quando necessário. |
| Dores/frustrações | [H] Excesso de parâmetros técnicos ou detalhes internos pode dificultar a identificação das informações relevantes; resultados sem contexto podem dificultar a comparação; e grande quantidade de métricas simultâneas pode tornar a análise confusa. |
| Motivadores | [H] Obter informações confiáveis, comparáveis e compreensíveis que apoiem a avaliação do comportamento das estratégias de controle semafórico. |
| Restrições/acessibilidade | [?] Ainda não existem evidências sobre necessidades específicas de acessibilidade desse perfil. A clareza das informações e a redução de complexidade técnica desnecessária podem influenciar a utilização da interface. |
| Ambiente típico de uso | [H] Computador desktop ou notebook em ambiente profissional ou institucional, principalmente durante a consulta e análise de resultados de estudos de mobilidade. |
| Comportamentos relevantes | [H] Prioriza informações consolidadas e comparações entre resultados, consultando detalhes técnicos somente quando eles são necessários para compreender ou justificar uma análise. |

**Decisões de design influenciadas por P02:**

- apresentar inicialmente as métricas mais relevantes de forma consolidada;
- permitir acesso a informações detalhadas sem obrigar o usuário a visualizar todos os parâmetros técnicos;
- deixar explícitos o cenário, a estratégia e as condições experimentais associados a cada resultado;
- utilizar terminologia do domínio de mobilidade sem depender de nomes internos do código;
- favorecer comparação visual entre estratégias e cenários;
- apresentar resultados de forma que diferenças relevantes possam ser identificadas rapidamente;
- permitir consultar uma síntese dos resultados sem eliminar a possibilidade de aprofundamento.
- 
### Síntese das personas

Explique diferenças entre os perfis e qual persona é prioritária. Evite personas duplicadas que só mudam nome/foto.

## 2. Mapa de empatia — equipe

**Persona escolhida:** {{P01}}  
**Justificativa:** {{por que esse perfil é relevante}}

![Mapa de empatia](../assets/03_personas/mapa_empatia.svg)

Documente também em texto: o que vê; ouve; diz/faz; pensa/sente; dores; ganhos. Diferencie **evidência** de **hipótese**.

## 3. Contexto de uso — consolidação

| Dimensão | Descrição | Implicação de design |
|---|---|---|
| Usuários | {{...}} | {{...}} |
| Tarefas | {{...}} | {{...}} |
| Equipamentos | {{...}} | {{...}} |
| Ambiente físico | {{...}} | {{...}} |
| Ambiente social/organizacional | {{...}} | {{...}} |
| Papéis/permissões/governança | {{...}} | {{...}} |
| Volume de dados/histórico | {{...}} | {{...}} |

## 4. Jornada do usuário — equipe

**Persona:** {{P01}}  
**Objetivo da jornada:** {{...}}  
**Início e fim da jornada:** {{...}}

| Etapa | Situação/ação | Objetivo | Pensamento/emoção | Dor | Oportunidade de design | Evidência |
|---|---|---|---|---|---|---|
| 1 | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

> A jornada pode incluir etapas **antes, durante e depois** do uso do produto. Não transforme a jornada em lista de telas.

## Síntese

Quais necessidades e objetivos devem obrigatoriamente aparecer nos cenários e nas tarefas seguintes?

## Checklist

- [ ] Existe pelo menos uma persona por integrante.
- [ ] As personas não são apenas diferenças demográficas superficiais.
- [ ] Está claro o que é dado real e o que é hipótese/proto-persona.
- [ ] A persona não “validou por ficção” uma hipótese da Entrega 1; afirmações continuam marcadas como hipótese quando não há evidência.
- [ ] Objetivos e dores têm consequência para o design.
- [ ] Contexto de uso está coerente com a Entrega 1.
- [ ] Em TCC sem interface original, a persona possui relação explícita com a contribuição técnica.
- [ ] Papéis administrativos, técnicos e decisórios só foram criados quando possuem objetivos/tarefas diferentes.
- [ ] Jornada possui etapas, dores e oportunidades e não é apenas wireflow.
- [ ] IDs das personas foram adicionados à rastreabilidade.
