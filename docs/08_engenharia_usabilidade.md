# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** 21/10/2026  
**Status:** 🟨 em andamento  
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Transformar o conhecimento acumulado nas Entregas 1–7 sobre usuários, tarefas, contexto de uso, plataforma e protótipo em **princípios de projeto e requisitos de usabilidade verificáveis**, mantendo o caráter iterativo do processo de IHC.

A Engenharia de Usabilidade considera que o projeto da interface deve partir do conhecimento sobre:

- usuários;
- tarefas;
- contexto de uso;
- capacidades e restrições da plataforma;
- requisitos qualitativos de interação;
- níveis de usabilidade esperados.

No projeto desta equipe, a Entrega 8 utiliza diretamente os artefatos já construídos:

- H01, H02 e H03 — hipóteses prioritárias;
- P01 e P02 — proto-personas;
- C01 e C02 — cenários de problema;
- T01–T08 — tarefas;
- PF01–PF03 — fluxos do protótipo;
- PP01–PP07 — estados documentados da V0;
- W01–W04 — tarefas do walkthrough;
- O01–O10 — observações da Entrega 6;
- I01 e I02 — instrumentos de investigação da Entrega 7.

A interface funcional existente continua sendo tratada como **protótipo digital V0**. As decisões apresentadas nesta entrega não significam que todas as alterações propostas já tenham sido implementadas.

---

# Delimitação do sistema interativo

É necessário diferenciar a contribuição técnica do TCC da camada de interação analisada na disciplina de IHC.

| Camada | O que pertence ao projeto | O que será avaliado em IHC |
|---|---|---|
| Contribuição técnica do TCC | Algoritmo híbrido de controle semafórico baseado em Max Pressure e lógica actuated, implementado em Python e integrado ao ambiente de simulação SUMO por meio do TraCI. O TCC também utiliza estratégias de referência, como controle de tempo fixo e Max Pressure convencional, e métricas de tráfego para avaliação experimental. | O desempenho técnico dos controladores não será utilizado como medida de usabilidade. Métricas como fila, tempo de espera, tempo de viagem ou throughput avaliam o experimento de tráfego, e não a qualidade da interação. |
| Camada de interação | Interface desktop utilizada para selecionar cenários, configurar experimentos, escolher controlador e modo de execução, validar condições, iniciar e acompanhar simulações, recuperar execuções anteriores e consultar seus resultados. | Compreensão da interface, conclusão das tarefas, prevenção e recuperação de erros, eficiência de interação, feedback, facilidade de aprendizado, satisfação e demais aspectos relacionados ao uso. |
| Integrações e dados experimentais | SUMO, TraCI, arquivos dos cenários, configurações dos experimentos, logs e resultados produzidos pelas simulações. | A interface deve comunicar adequadamente o estado dessas integrações e manter clara a relação entre cenário, configuração, execução e resultado. |

A V0 utilizada nas Entregas 6–8 está integrada ao ambiente experimental real do TCC. Portanto, os estados documentados representam o funcionamento da aplicação e sua relação com o SUMO, e não apenas telas fictícias desconectadas do processamento.

A avaliação de IHC deverá permanecer concentrada na **forma como uma pessoa interage com esse ambiente**, e não substituir a avaliação experimental do algoritmo realizada no TCC.

---

# 1. Características da plataforma

A análise das capacidades e restrições da plataforma considera os recursos técnicos disponíveis e suas consequências para a interação.

Segundo o ciclo de Engenharia de Usabilidade trabalhado na disciplina, devem ser consideradas possibilidades e limitações relacionadas a equipamentos, sistemas operacionais, ambiente de janelas, recursos de processamento e demais elementos que possam afetar o uso da interface.

## 1.1 Características gerais

| Característica | Descrição | Consequência para IHC |
|---|---|---|
| Software | Aplicação desktop desenvolvida em Python e integrada ao SUMO por meio do TraCI. A interface fornece acesso aos principais fluxos de configuração, execução e análise do ambiente experimental. | A interação deve considerar convenções de aplicações desktop e manter clara a transição entre a interface principal e componentes externos, como o SUMO-GUI. |
| Ambiente de simulação | O SUMO executa as simulações de tráfego utilizadas pelo TCC. No modo Visual, o usuário também acompanha a simulação pelo SUMO-GUI. | A abertura de uma janela externa não deve fazer o usuário perder a compreensão de qual experimento está ativo ou de qual aplicação controla a execução. |
| Hardware/dispositivos | Computador desktop ou notebook capaz de executar Python, a interface e o SUMO. A interação é realizada principalmente por monitor, teclado e mouse. | Os controles devem ser adequados à interação convencional de desktop e não devem depender de dispositivos especiais. |
| Processamento | As simulações podem possuir duração variável conforme cenário, parâmetros, seed, controlador e modo de execução. | A interface deve deixar evidente quando uma execução está sendo inicializada, executada, concluída ou interrompida por erro. |
| Armazenamento de resultados | Execuções geram informações que podem ser recuperadas posteriormente pela área de resultados/histórico. | Cada resultado deve permanecer associado ao contexto experimental que o produziu, reduzindo risco de interpretação ou comparação incorreta. |
| Execução Visual | O modo Visual utiliza o SUMO-GUI para permitir inspeção direta do comportamento da rede. | A interface deve comunicar claramente que a janela do SUMO faz parte da execução ativa e preservar a identificação do experimento. |
| Execução Headless | O experimento pode ser executado sem a visualização gráfica da rede. | Como não existe evidência visual direta do SUMO-GUI, o feedback textual e o estado da execução tornam-se ainda mais importantes. |
| Configuração avançada | Determinados experimentos disponibilizam parâmetros técnicos adicionais além das configurações principais. | Os parâmetros avançados não devem dominar o fluxo principal e precisam permanecer diferenciados das configurações utilizadas com maior frequência. |

---

## 1.2 Capacidades da plataforma

| Capacidade | Justificativa | Consequência para o projeto da interface |
|---|---|---|
| Selecionar diferentes cenários/infraestruturas | O ambiente experimental do TCC utiliza diferentes redes e condições de simulação. | O cenário ativo deve permanecer claramente identificado durante a preparação do experimento. |
| Exibir informações do cenário | O usuário precisa compreender em qual infraestrutura realizará o experimento. | Informações visuais e textuais devem complementar identificadores técnicos sempre que possível. |
| Configurar parâmetros experimentais | As condições do experimento influenciam diretamente sua execução e posterior interpretação. | Parâmetros devem possuir organização clara e distinção entre configurações principais e avançadas. |
| Selecionar diferentes estratégias de controle | O TCC compara Fixed-Time, Max-Pressure e Hybrid Max-Pressure + Actuated. | O controlador selecionado precisa permanecer explícito antes, durante e depois da execução. |
| Configurar seed | A seed faz parte das condições experimentais e contribui para rastreabilidade e reprodutibilidade. | A seed deve permanecer vinculada à execução e ao resultado produzido. |
| Escolher modo Visual ou Headless | O sistema suporta diferentes formas de execução. | O usuário deve compreender a diferença entre os modos e receber feedback suficiente em ambos. |
| Validar a configuração antes da execução | Uma configuração inadequada pode inutilizar um experimento ou comprometer sua interpretação posterior. | A interface deve prevenir erros conhecidos antes de iniciar o processamento. |
| Confirmar condições antes do início | A execução pode consumir tempo e gerar resultados que só são úteis quando correspondem às condições planejadas. | O sistema deve oferecer oportunidade de revisão antes do início definitivo. |
| Fornecer feedback durante a execução | O processamento não é necessariamente instantâneo. | O estado principal deve ser perceptível sem exigir interpretação de logs técnicos. |
| Executar simulação visualmente | O SUMO-GUI permite observar diretamente o comportamento da rede. | Essa capacidade deve permanecer disponível sem substituir informações de estado fornecidas pela aplicação principal. |
| Manter histórico de execuções | O projeto realiza múltiplos experimentos com cenários, controladores, seeds e configurações diferentes. | O usuário precisa conseguir recuperar uma execução e identificar seu contexto. |
| Apresentar resultados individuais | Cada execução produz métricas e informações utilizadas na análise experimental. | Resultado, configuração e identificação da execução devem permanecer associados. |
| Apresentar gráficos da execução | Representações gráficas auxiliam a interpretação das métricas produzidas. | O gráfico deve complementar os valores e não eliminar o acesso às informações que explicam o contexto do resultado. |

---

## 1.3 Restrições da plataforma

| Restrição | Justificativa | Consequência para IHC |
|---|---|---|
| Dependência do SUMO e do ambiente experimental | A execução depende da infraestrutura técnica utilizada pelo TCC. | Falhas de inicialização ou integração precisam produzir mensagens compreensíveis e permitir recuperação. |
| Vocabulário especializado | Termos como seed, Max-Pressure, Hybrid, Headless e parâmetros do controlador fazem parte do domínio técnico. | A precisão técnica deve ser preservada, mas termos potencialmente desconhecidos devem receber contexto quando necessário. |
| Configuração com muitos parâmetros | Certos controladores e cenários exigem valores adicionais. | A elevada densidade de informação pode aumentar carga cognitiva. A separação entre configuração principal e avançada deve ser preservada. |
| Processamento com duração variável | Diferentes cenários e configurações podem produzir tempos distintos de execução. | O usuário não pode interpretar ausência temporária de resultado como travamento da aplicação. |
| SUMO-GUI em janela externa | A execução Visual ocorre fora da janela principal da interface. | A separação entre as duas janelas pode produzir perda de contexto e deve ser compensada por identificação e feedback adequados. |
| Histórico pode crescer com novas execuções | O uso contínuo do ambiente pode gerar grande quantidade de resultados. | A necessidade de mecanismos adicionais de busca, filtros ou organização deverá ser confirmada antes de sua implementação definitiva. |
| Comparação não automatizada na V0 | A aplicação permite consultar execuções individualmente, mas não mantém duas execuções em uma visualização comparativa automática. | T07 exige atualmente alternância entre resultados e comparação manual externa. Uma visualização comparativa permanece como possibilidade de evolução, não como funcionalidade existente. |
| Dependência de conhecimento do domínio | A interpretação das configurações e métricas pode exigir experiência em simulação, tráfego ou experimentação. | A interface não deve eliminar precisão técnica, mas precisa evitar exigir conhecimento da implementação interna quando isso não for necessário para a tarefa. |
| Ausência de papéis administrativos no recorte atual | Não foram identificadas tarefas de gerenciamento de usuários, perfis ou permissões nas Entregas 1–7. | Não há justificativa atual para introduzir telas administrativas ou mecanismos de autorização apenas para tornar o sistema mais complexo. |

---

## 1.4 Conectividade e execução local

O fluxo principal da V0 é baseado na execução do ambiente experimental no computador utilizado pelo pesquisador.

A conexão contínua com serviços externos não constitui uma necessidade central dos fluxos PF01–PF03 atualmente documentados.

Consequentemente, problemas de latência de rede não são tratados como uma das principais restrições de interação nesta etapa.

O tempo percebido pelo usuário está principalmente associado a:

- inicialização do ambiente experimental;
- complexidade do cenário;
- duração configurada;
- estratégia utilizada;
- modo de execução;
- capacidade de processamento da máquina.

Esses fatores reforçam a importância do feedback de estado identificado na Entrega 6.

---

## 1.5 Segurança e privacidade

A V0 não possui, no recorte atual, cadastro de usuários, autenticação, perfis administrativos ou tratamento operacional de dados pessoais como parte do fluxo principal de simulação.

Os principais dados manipulados são relacionados aos experimentos:

- cenário;
- parâmetros;
- controlador;
- seed;
- informações de execução;
- logs;
- métricas;
- resultados.

Por esse motivo, segurança e privacidade na interface operacional estão relacionadas principalmente a:

- evitar alteração acidental de condições experimentais;
- preservar a relação entre execução e configuração;
- impedir interpretações incorretas causadas por perda de contexto;
- evitar exposição desnecessária de informações locais em evidências públicas.

Questões de privacidade relacionadas a participantes de pesquisa pertencem principalmente ao plano ético documentado na Entrega 7.

---

## 1.6 Volume de dados e histórico

A metodologia do TCC prevê múltiplos cenários, estratégias, seeds e execuções.

A existência de histórico já é justificada pela necessidade de recuperar resultados anteriores.

Entretanto, as Entregas 1–7 **não validaram a necessidade de um mecanismo avançado específico de busca, filtros, paginação ou agrupamento**.

A decisão atual é:

- preservar o histórico existente;
- manter contexto suficiente para identificar cada execução;
- observar o comportamento do sistema quando o volume crescer;
- investigar posteriormente quais mecanismos adicionais realmente são necessários.

Essa decisão evita transformar uma possibilidade de interface em requisito sem evidência.

---

## 1.7 Tempo de processamento e feedback

O tempo de uma simulação não é constante.

O usuário precisa reconhecer pelo menos os seguintes estados:

```text
configuração preparada
        ↓
validação
        ↓
confirmação
        ↓
inicialização
        ↓
execução
        ↓
conclusão
