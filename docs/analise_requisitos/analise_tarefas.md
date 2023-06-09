<div class="body">

# Análise de Tarefas

## Introdução

<div align="justify">

&emsp;&emsp;Uma análise de tarefas é utilizada para se ter um entendimento sobre qual é o trabalho dos usuários, como eles o realizam e por quê. Nesse tipo de análise, o trabalho é definido em termos dos objetivos que os usuários querem ou precisam atingir. [1]

&emsp;&emsp;Esta análise pode ser usada para identificar a situação atual (apoiada ou não por um sistema computacional), para o (re)design ou para a avaliação do resultado de uma intervenção que inclua a introdução de um (novo) sistema computacional. Um dos primeiros passos numa análise de tarefas é a coleta de um conjunto objetivos das pessoas ao utilizarem o sistema analisado. 

&emsp;&emsp;O site do Banco Central do Brasil (BCB) é um site majoritariamente informativo, disponibilizando de uma gama de informações. O usuário pode acessar informações como: história do BCB; agenda das Autoridades, Chefes de Unidade e Gabinetes; calendário de eventos relacionados ao sistema financeiro; cotação das moedas internacionais; conversor de moedas; estatísticas e identificadores econômicos; consulta às mudanças no sistema financeiro; informações quanto as cédulas e moedas (como identificar a autenticidade, moedas e notas antigas e comemorativas, formas de conservação); entre outros tipos de informação. Tendo em vista a quantidade de ramificações de um objetivo como o acesso a informações, foi decidido por não escolher essa tarefa para análise.

&emsp;&emsp;As principais tarefas para análise identificadas no site do Banco Central do Brasil, foram: consultar dados financeiros pessoais através do Registrato (cheques sem fundo estornados, empréstimos e financiamentos, contas de bancos, chaves pix cadastradas, relatório de dívidas e operações de câmbio), acessar cursos, consultar taxas de juros, consultar empresas vinculadas ao BCB e seus dados, consultar valores a receber do governo e calculadora do cidadão. Essas tarefas foram definidas de acordo com os dados coletados do [perfil de usuário](https://interacao-humano-computador.github.io/2023.1-BancoCentral/#/analise_requisitos/perfil_usuario), onde é relatado as atividades que os usuários utilizam ou possuem interesse de utilizar. 

## Metodologia

&emsp;&emsp;A metodologia de desenvolvimento das análises de tarefas foi definida visando explorar diferentes técnicas, definindo a mais compatível com cada tarefa selecionada. As técnicas de análise escolhidas foram o AHT (Análise Hierárquica de Tarefas) e o CTT (Árvore de Tarefas Concorrentes). Essa análise é essencial para identificar o fluxo de passos das tarefas, identificando o que deve ser melhorado.

## Análise Hierárquica de Tarefas


&emsp;&emsp;A Análise Hierárquica de Tarefas (HTA), criada na década de 60, é uma ferramenta utilizada para entender as competências e habilidades necessárias para realizar tarefas complexas e não repetitivas. Além disso, é útil para identificar problemas de desempenho. A HTA ajuda a relacionar as ações das pessoas, o motivo pelo qual elas as executam e quais são as consequências se essas ações não forem realizadas corretamente.

&emsp;&emsp;A Tabela 1 apresenta os elementos de uma análise hierárquica de tarefas.

</div>

| <p align="center">Elemento</p> | <p align="center">Descrição</p> | 
| --                           | ---- | 
|**Tarefa**:     | parte do trabalho que precisa ser realizada, pode ser definida em termos de objetivos e subobjetivos|
|**Objetivo**:   | é um estado específico, um estado final, definido por eventos ou por valores fisicamente observáveis de variáveis, que atuam como critério de alcance do objetivo |
|**Subobjetivo**:| decomposição de objetivos complexos, utilizados para identificar quais subobjetivos são mais difíceis de atingir, visto que limitam ou mesmo impedem o atingimento do objetivo maior|
|**Plano**:      | define os subobjetivos necessários para alcançar um outro objetivo maior, e a ordem em que esses subobjetivos devem ser alcançados|
|**Operação**:   | circunstâncias nas quais o objetivo é ativado (input ou entrada), pelas atividades ou ações (actions) que contribuem para atingi-lo e pelas condições que indicam o seu atingimento (feedback)|
<div align="center">
<p> <b>Tabela 1</b>: Elementos de uma HTA (Fonte: GOMES, Larissa. 2023). </p>
</div>


<p align="justify">A Figura 1 apresenta os elementos de um diagrama HTA.</p>

<img title="a title" alt="Elementos HTA" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/main/docs/img/analise_tarefas/elementosHTA.png" width="100%">

<div align="center">
<p> <b>Figura 1</b>: Elementos de um diagrama HTA (Fonte: GOMES, Larissa. 2023). </p>
</div>

<p align="justify">

&emsp;&emsp;Os planos podem possuir relações entre os subobjetivos, como: sequência fixa (um objetivo deve ser atingido antes do próximo); regra de seleção ou decisão (quais objetivos que deverão ser atin-gidos dependem das circunstâncias); ou em paralelo (mais de um objetivo deve ser atingido ao mesmo tempo). A Figura 1 apresenta a forma gráfica de representação dessas relações.
</p>

### Motivo da escolha

<p align="justify">

&emsp;&emsp;Este método foi escolhido para analisar as tarefas <b>Consultar dados financeiros pessoais através do Registrato</b> e <b>Calculadora do cidadão</b>, esta última foi dividida em duas partes, sendo a tarefa da calculadora de correção de valores uma tarefa maior dentro da calculadora do cidadão, portanto foi decidido fazer uma análise separada para ela, visto que são tarefas com muitas possibilidades, entretanto todas possuem uma mesma ordem de operações. Tendo isso em vista, a separação em subobjetivos hierárquicos seria a melhor forma de entender o comportamento do usuário.</p>

### Análise da Tarefa HTA 1: Consultar dados financeiros pessoais através do Registrato

<p align="justify">

&emsp;&emsp;A principal tarefa oferecida pelo BCB é "consultar dados financeiros pessoais através do Registrato". O Registrato é um sistema administrado pelo Banco Central que permite aos cidadãos terem acesso pela internet, de forma rápida e segura, a relatórios contendo informações sobre relacionamentos com as instituições financeiras, operações de crédito e de câmbio. Na Tabela 2 está a análise detalhada representada em tabela.

</p>

|<p align="center">objetivos / operações</p> | <p align="center">Relações</p> | <p align="center">problemas e recomendações</p> |
| --                                         | :----: |  ---- | 
| 0. acessar dados financeiros pessoais      |  1>2	 | **Input**: acesso ao registrato pelo gov.br, com cpf e senha, com a escolha do tipo de dado a ser acessado (em alguns casos a escolha das datas dos dados) e a concordância com os termos.</br> **Plano**: acessar registrato, **depois** escolher o tipo de dado a ser acessado, **em seguida** aceitar os termos e **por último** gerar relatório.</br> **Feedback**: Relatório de Serviços gerado.</br> **Problema**: o registrato apenas apresenta as informações para quem possui nível prata ou ouro em sua conta gov.br.</br> **Recomendação**: informar antes de acessar o registrato a necessidade de ter uma conta gov.br acima do nível prata. |
| 1. acessar o registrato |  1>2  | **Plano**: informar o cpf e **depois** a senha do gov.br. </br> **Feedback**: tela menu de Serviços Registrato. |
| 1.1.	Informar cpf  |    |  |
| 1.2.	Informar senha do gov.br |    |  |
| 2. Escolher tipo de dado a ser acessado |  1/2  | **Plano**: selecionar uma das opções, **entre** Cheques sem Fundos, Empréstimos e Financiamentos, Contas e Relacionamentos, Cadin Federal, Chaves Pix ou Câmbio. </br> **Feedback**: tela menu de solicitação de relatório. |
| 2.1. Selecionar Cheques sem Fundos	 |    |  |
| 2.2. Empréstimos e Financiamento |  1>2  | **Plano**: selecionar Empréstimos e Financiamentos, **em seguida** definir informações. |
| 2.2.1. Selecionar Empréstimos e Financiamento	 |    |  |
| 2.2.2. Definir informações |  1+2  | **Plano**: informar tipo de relatório e data-base inicial e final. |
| 2.2.2.1. Informar Data-base inicial	 |    |  |
| 2.2.2.2. Informar Data-base final |    |  |
| 2.2.2.3. Informar tipo de relatório	 |    |  |
| 2.3. Selecionar Contas e Relacionamentos |    |  |
| 2.4. Selecionar Cadin Federal (Relatório de dívidas) |    |  |
| 2.5. Câmbio |  1>2  | **Plano**: selecionar Câmbio, **em seguida** definir informações |
| 2.5.1. Selecionar Câmbio   |    |  |
| 2.5.2. Definir informações |  1+2  | **Plano**: informar data liquidação inicial e final. |
| 2.5.2.1. Informar Data de liquidação inicial	 |    |  |
| 2.5.2.2. Informar Data de liquidação inicial	 |    |  |
| 2.6. Selecionar Chaves Pix	 |    |  |
| 3. Aceitar 	termos de ciência e responsabilidade	 |    |  |
| 4. Gerar relatório	 |    |  |

<div align="center">
<p> <b>Tabela 2</b>: Tabela da representação HTA da tarefa "Consultar dados financeiros pessoais através do Registrato" (Fonte: GOMES, Larissa. 2023). </p>
</div>

<p align="justify">

&emsp;&emsp;Com o resultado da análise descrita na Tabela 2, foi criado o diagrama HTA (Figura 2). A Tabela 1 e Figura 1 são fundamentais para o entendimento do diagrama, sendo uma legenda para ele.

</p>

<img title="a title" alt="Diagrama HTA" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/main/docs/img/analise_tarefas/diagramaHTA.png" width="100%">

<div align="center">
<p> <b>Figura 2</b>: Diagrama da representação HTA da tarefa "Consultar dados financeiros pessoais através do Registrato" (Fonte: GOMES, Larissa. 2023). </p>
</div>

### Análise da Tarefa HTA 2: Calculadora do Cidadão - Aplicação com depósitos regulares, Financiamento com prestações fixas e Valor futuro de um capital

<p align="justify"> 

&emsp;&emsp;A calculadora do cidadão é uma calculadora financeira, onde o usuário pode fazer diversos tipos de cálculos, ela pode ser dividada em duas partes, sendo a de Aplicação com depósitos regulares, Financiamento com prestações fixas e Valor futuro de um capital com mesmo fluxo de passos para sua realização, como pode ser observado na Tabela 3 e Figura 3

</p>

|<p align="center">objetivos / operações</p> | <p align="center">Relações</p> | <p align="center">problemas e recomendações</p> |
| --                                         | :----: |  ---- | 
| 0. Utilizar a calculadora do cidadão | 1/2/3 | **Plano**: selecionar uma das tarefas possíveis dentro da modalidade calculadora do cidadão. |
| 1. Simular aplicações com depósitos regulares | | **Plano**: informar dados para a simulação da aplicação (meses, parcelas, valor final, taxa de juros) |
| 1.1. Informar dados para simulação | |  |
| 2. Simular financiamento com prestações fixas | | **Plano**: informar dados para a simulação da aplicação (meses, parcelas, valor final, taxa de juros) |
| 2.1. Informar dados para simulação | |  |
| 3. Simular valor futuro de capital | | **Plano**: informar dados para a simulação da aplicação (meses, parcelas, valor final, taxa de juros) |
| 3.1. Informar dados para simulação | |  |

<div align="center">
<p> <b>Tabela 3</b>: Tabela da representação HTA da tarefa "Calculadora do Cidadão, parte 1" (Fonte: RIBEIRO, Bruno. 2023). </p>
</div>

<p align="justify">

&emsp;&emsp;Com o resultado da análise descrita na Tabela 3, foi criado o diagrama HTA (Figura 3). A Tabela 1 e Figura 1 são fundamentais para o entendimento do diagrama, sendo uma legenda para ele.

</p>

<img title="a title" alt="Diagrama HTA" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-BancoCentral/main/docs/img/analise_tarefas/HTA_calculadora_cidadao.png" width="100%">

<div align="center">
<p> <b>Figura 3</b>: Diagrama da representação HTA da tarefa "Calculadora do Cidadão, exceto correção de valores" (Fonte: RIBEIRO, Bruno. 2023). </p>
</div>

### Análise da Tarefa HTA 2.1: Calculadora do Cidadão - Correção de Valores

<p align="justify"> 

&emsp;&emsp;A segunda parte da calculadora, a opção de correção de valores, possue um fluxo de passos diferente da primeira parte, sendo focada em correção de valores baseado em datas. Essa opção possue várias subopções dentro da tarefa, dentro delas está a parte de informação de dados para correção, possuindo cada uma passos que as diferem das outras opções. A análise dessa tarefa pode ser vista na Tabela 4 e Figura 4.

</p>

|<p align="center">objetivos / operações</p> | <p align="center">Relações</p> | <p align="center">problemas e recomendações</p> |
| --                                         | :----: |  ---- | 
| 0. acessar dados financeiros pessoais      |  1>2	 | **Input**: acesso ao registrato pelo gov.br, com cpf e senha, com a escolha do tipo de dado a ser acessado (em alguns casos a escolha das datas dos dados) e a concordância com os termos.</br> **Plano**: acessar registrato, **depois** escolher o tipo de dado a ser acessado, **em seguida** aceitar os termos e **por último** gerar relatório.</br> **Feedback**: Relatório de Serviços gerado.</br> **Problema**: o registrato apenas apresenta as informações para quem possui nível prata ou ouro em sua conta gov.br.</br> **Recomendação**: informar antes de acessar o registrato a necessidade de ter uma conta gov.br acima do nível prata. |
| 1. acessar o registrato |  1>2  | **Plano**: informar o cpf e **depois** a senha do gov.br. </br> **Feedback**: tela menu de Serviços Registrato. |
| 1.1.	Informar cpf  |    |  |
| 1.2.	Informar senha do gov.br |    |  |
| 2. Escolher tipo de dado a ser acessado |  1/2  | **Plano**: selecionar uma das opções, **entre** Cheques sem Fundos, Empréstimos e Financiamentos, Contas e Relacionamentos, Cadin Federal, Chaves Pix ou Câmbio. </br> **Feedback**: tela menu de solicitação de relatório. |
| 2.1. Selecionar Cheques sem Fundos	 |    |  |
| 2.2. Empréstimos e Financiamento |  1>2  | **Plano**: selecionar Empréstimos e Financiamentos, **em seguida** definir informações. |
| 2.2.1. Selecionar Empréstimos e Financiamento	 |    |  |

<div align="center">
<p> <b>Tabela 4</b>: Tabela da representação HTA da tarefa "Calculadora do Cidadão, correção de valores" (Fonte: SANTOS, Mizael. 2023). </p>
</div>

<p align="justify">

&emsp;&emsp;Com o resultado da análise descrita na Tabela 4, foi criado o diagrama HTA (Figura 4). A Tabela 1 e Figura 1 são fundamentais para o entendimento do diagrama, sendo uma legenda para ele.</p>

<img title="a title" alt="Diagrama HTA" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/main/docs/img/analise_tarefas/NOMEARQUIVO.png" width="100%">

<div align="center">
<p> <b>Figura 4</b>: Diagrama da representação HTA da tarefa "Calculadora do Cidadão, parte 2" (Fonte: SANTOS, Mizael. 2023). </p>
</div>


### Conclusão das análises HTA

<p align="justify">

&emsp;&emsp;As tabelas e os diagramas (Tabelas 2 a 4 e Figuras 2 a 4) mostram a sequência de passos realizados por um usuário para atingir seu objetivo. Para um melhor entendimento do fluxo de passos realizados pelos usuários para executar sua tarefa, o objetivo principal da atividade foi decomposto em subobjetivos e com as suas relações para determinar a sequência de operações a serem realizadas para alcançar a conclusão da tarefa.</p>

## Árvore de Tarefas Concorrentes (CTT)

<div align="justify">

&emsp;&emsp;A Árvore de Tarefas Concorrentes (CTT) é uma técnica de design de interação que permite representar as tarefas que podem ser executadas simultaneamente pelo usuário em um sistema interativo. A técnica do CTT foi desenvolvida como uma extensão da Árvore de Tarefas (AT), uma metodologia que permite representar as tarefas que o usuário precisa realizar para atingir seus objetivos em um sistema.

Nesse modelo existem 4 tipos de tarefas:

- Tarefas do usuário, realizadas fora do sistema;
- Tarefas do sistema, em que o sistema realiza um processamento sem interagir com o usuário;
- Tarefas interativas, em que ocorrem diálogos usuário-sistema;
- Tarefas abstratas, que não são tarefas em si, mas sim uma representação de uma composição de tarefas que auxilie a decomposição.

Assim como na análise de tarefas HTA, haverão diferentes níveis hierárquicos.

A técnica de Árvore de Tarefas Concorrentes (CTT) foi escolhida como método de avaliação das tarefas dos usuários, pois:

- Permite identificar quais tarefas podem ser realizadas ao mesmo tempo pelo usuário, sem que uma interfira na outra. Isso é importante para otimizar a interação e reduzir o tempo de conclusão das tarefas;
- Permite organizar as tarefas de forma hierárquica, o que ajuda a entender a relação entre as tarefas e a priorizar aquelas que são mais importantes para o usuário;
- Permite identificar os pontos em que o usuário precisa tomar uma decisão, o que ajuda a entender melhor o comportamento do usuário e a projetar uma interface mais intuitiva e fácil de usar;
- Permite visualizar de forma clara as relações entre as tarefas e as dependências entre elas. Isso ajuda a entender o fluxo de trabalho do usuário.

</div>

### Nomenclaturas utilizadas no CTT

<div align="justify">

&emsp;&emsp;Foi demonstrado como seriam as atividades com árvores de tarefas concorrentes (CTT), onde alguns símbolos foram utilizados para poder representar a ordem das tarefas. Sendo eles:

- T1 >> T2: Tarefa 2 iniciará após o término da tarefa 1;
- T1 ||| T2: Especifica que as tarefas 1 e 2 podem ser realizadas em qualquer ordem ou ao mesmo tempo;
- T1 []>> T2: Tarefa 2 iniciará após o término da tarefa 1 e a informação da tarefa 1 é passada para a tarefa 2.
- T1 [] T2: Especifica que o usuário deve escolher entre realizar a tarefa 1 ou a tarefa 2.

Essas relações entre tarefas podem ser observadas na Figura 5, logo a seguir.</div>

<img alt="Legenda da CTT" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/master/docs/img/analise_tarefas/legenda_ctt.png" width="100%">

<div align="center">
<p> <b>Figura 5</b>: Legenda da Árvore de Tarefas Concorrentes (Fonte: BOSI, Rafael. 2023). </p>
</div>

### Motivo da Escolha

<p align="justify">

&emsp;&emsp;Este método foi escolhido para analisar as tarefas <b>Acessar Cursos</b>, <b>Consultar taxas de juros</b>, <b>Consultar empresas vinculadas ao BCB e seus dados</b> e <b>Consultar valores a receber do governo</b>, visto que em todas essas atividades são necessárias interações entre o usuário e o sistema. A técnica da Árvore de Tarefas Concorrentes consegue deixar essas interações dispostas de maneira hierarquica, além de criar uma organização cronológica entre as interações, o que deixa a tarefa disposta de maneira muito mais clara.</p>


### Análise da Tarefa CTT 1: Acessar curso

<p align="justify">

&emsp;&emsp;A tarefa "acessar curso", consistem basicamente em escolher algum dos cursos ofertados pelo BCB, em seguida fazer login ou se registrar, após isso o acesso aos cursos estará disponível ao usuário. Na Figura 6 está a análise detalhada representada em diagrama e sua legenda disponível na Figura 5. 

</p>

<img title="a title" alt="CTT Acessar Curso" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/master/docs/img/analise_tarefas/ctt_acessar_curso.png" width="100%">

<div align="center">
<p> <b>Figura 6</b>: Diagrama da representação CTT da tarefa "Acessar Curso" (Fonte: BOSI, Rafael. 2023). </p>
</div>

### Análise da Tarefa CTT 2: Consultar taxas de juros

<p align="justify"> 

&emsp;&emsp;A tarefa de taxas de juros do Banco Central é voltada apenas para a visualização em tabelas. Tendo em vista que um dos objetivos é melhoras as tarefas para se tornarem mais completas, foi desenvolvido um fluxo para esta tarefa adicionando uma opção de gerar gráficos comparativos das taxas.</p>

<img title="a title" alt="CTT Consultar taxas de juros" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/master/docs/img/analise_tarefas/consultar_taxas_CTT.png" width="100%">

<div align="center">
<p> <b>Figura 7</b>: Diagrama da representação CTT da tarefa "Consultar taxas de juros" (Fonte: ALVISSUS, Giovanni. 2023). </p>
</div>

### Análise da Tarefa CTT 3: Consultar empresas vinculadas ao BCB e seus dados

<p align="justify">

&emsp;&emsp; A tarefa "consultar empresas vinculadas ao BCB e seus dados" serve para encontra a lista de instituições autorizadas , reguladas ou supervisionadas pelo Banco Central do Brasil (BC). Essas informações são importantes para conhecer o mercado e saber se a instituição que está oferecendo uma abertura de conta, algum produto ou empréstimo está cadastrada no BC e, assim, evitar golpes. Nesta tarefa pode ser informado os dados da instituição específica ou apenas pesquisar, gerando uma tabela com instituições, ao selecionar alguma os dados dela são apresentados, divididos em categorias. O fluxo dessa tarefa está representado na Figura 8.

</p>

<img title="a title" alt="CTT Consultar empresas" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/264-correção-planejamento-avaliação-analise-de-tarefas/docs/img/analise_tarefas/consultar_empresas_CTT.png" width="100%">

<div align="center">
<p> <b>Figura 8</b>: Diagrama da representação CTT da tarefa "Consultar empresas" (Fonte: GOBBI, Lucas. 2023). </p>
</div>

### Análise da Tarefa CTT 4: Consultar valores a receber do governo

<p align="justify">

&emsp;&emsp; A tarefa "consultar valores a receber do governo" consiste em informar seus dados pessoais, qual tipo de valor a receber e em seguida consultar, em seguida sendo retornado pelo sistema do Banco Central qualquer valor a receber no nome do usuário. Esta sequência de passos pode ser observada na Figura 9; 

</p>

<img title="a title" alt="Consultar valores" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/master/docs/img/analise_tarefas/Analise_de_tarefa_ValoresReceber.png" width="100%">

<div align="center">
<p> <b>Figura 9</b>: Diagrama da representação CTT da tarefa "Consultar valores" (Fonte: PENHA, Igor. 2023). </p>
</div>

### Conclusão das análises CTT

<p align="justify">

&emsp;&emsp;Os diagramas (Figuras 6 a 9) mostram a sequência de interações realizados por um usuário, tanto próprias quanto com o sistema e os passos do sistema para o usuário ser capaz de atingir seu objetivo. Para um melhor entendimento, o objetivo principal foi decomposto em subobjetivos e com as suas relações para determinar a sequência de interações a serem realizadas.

</p>

## Referência Bibliográfica

[1] SIMONE DINIZ JUNQUEIRO BARBOSA, BRUNO SANTANA DA SILVA, Interação Humano-Computador, 1a. Edição, Editora Campus, 2010. (Versão grátis disponível em: https://docplayer.com.br/63299367-Interacao-humano-computador.html). Acessado em: 06/05/2023.

## Bibliografia

[1] SALES, André Barros. Apresentação Cap6 . Disponível em: https://aprender3.unb.br/pluginfile.php/2523447/mod_resource/content/4/Apresentacao%20cap06.pdf. Acesso em: 06 de Maio de 2023;

## Histórico de Versões

| <p align="center">Data</p> | <p align="center">Versão</p> | <p align="center">Descrição</p> | <p align="center">Autor(es)</p> | <p align="center">Data de revisão</p> | <p align="center">Revisor(es)</p> |
| :--:                       | :----: | :-------: | :---: | :-------------: | :-----: |
| 06/05/2023 | `1.0`  | Criação da introdução e escolha das tarefas | [Larissa Gomes](https://github.com/larigs) | 06/05/2023 | [Rafael Bosi](https://github.com/StrangeUnit28) |
| 08/05/2023 | `1.1`  | Adição do CTT e correção de alguns pontos | [Rafael Bosi](https://github.com/StrangeUnit28) | 08/05/2023 | [Larissa Gomes](https://github.com/larigs) |
| 08/05/2023 | `1.2`  | Adição da tabela e diagrama HTA | [Larissa Gomes](https://github.com/larigs) | 08/05/2023 | [Rafael Bosi](https://github.com/StrangeUnit28) |
| 08/05/2023 | `1.3`  | Adição do CTT e da legenda | [Rafael Bosi](https://github.com/StrangeUnit28) | 08/05/2023 | [Larissa Gomes](https://github.com/larigs) |
| 08/05/2023 | `1.4`  | Correções dentro do documento | [Larissa Gomes](https://github.com/larigs) e [Rafael Bosi](https://github.com/StrangeUnit28) | 08/05/2023 |  [Lucas Gobbi](https://github.com/LucasBergholz) |
| 20/05/2023 | `2.0`  | Adição das novas tarefas, adaptação e correção dos textos | [Larissa Gomes](https://github.com/larigs) | 20/05/2023 |  [Rafael Bosi](https://github.com/StrangeUnit28) |
| 04/07/2023 | `3.0`  | Adição de motivo de escolha e texto descritivo de cada tarefa | [Larissa Gomes](https://github.com/larigs) | 04/07/2023 |  [Giovanni Alvissus](https://github.com/giovanni1106) |
</div>
