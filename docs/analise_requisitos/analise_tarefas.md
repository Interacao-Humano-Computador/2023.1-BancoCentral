<div class="body">

Uma análise de tarefas é utilizada para se ter um entendimento sobre qual é o trabalho dos usuários, como eles o realizam e por quê. Nesse tipo de análise, o trabalho é definido em termos dos objetivos que os usuários querem ou precisam atingir. [1]

Esta análise pode ser usada para identificar a situação atual (apoiada ou não por um sistema computacional), para o (re)design ou para a avaliação do resultado de uma intervenção que inclua a introdução de um (novo) sistema computacional.

Um dos primeiros passos numa análise de tarefas é a coleta de um conjunto objetivos das pessoas ao utilizarem o sistema analisado. 

O site do Banco Central do Brasil (BCB) é um site majoritariamente informativo, disponibilizando de uma gama de informações. O usuário pode acessar informações como: história do BCB; agenda das Autoridades, Chefes de Unidade e Gabinetes;, calendário de eventos relacionados ao sistema financeiro; cotação das moedas internacionais; conversor de moedas; estatísticas e identificadores econômicos; consulta às mudanças no sistema financeiro; informações quanto as cédulas e moedas (como identificar a autenticidade, moedas e notas antigas e comemorativas, formas de conservação); entre outros tipos de informação. Tendo em vista a quantidade de ramificações de um objetivo como o acesso a informações, foi decidido por não escolher essa tarefa para análise.

As principais tarefas para análise identificadas no site do Banco Central do Brasil, foram: acessar dados financeiros pessoais (cheques sem fundo estornados, empréstimos e financiamentos, contas de bancos, chaves pix cadastradas, relatório de dívidas e operações de câmbio), emissão de boletos de multas e aprender sobre o financeiro. 

As técnicas de análise escolhidas foram o AHT (Análise Hierárquica de Tarefas) e o CTT (Árvore de Tarefas Concorrentes)
</p>

## Análise Hierárquica de Tarefas

<p align="justify">A Análise Hierárquica de Tarefas (HTA), criada na década de 60, é uma ferramenta utilizada para entender as competências e habilidades necessárias para realizar tarefas complexas e não repetitivas. Além disso, é útil para identificar problemas de desempenho. A HTA ajuda a relacionar as ações das pessoas, o motivo pelo qual elas as executam e quais são as consequências se essas ações não forem realizadas corretamente.
A Tabela 1 apresenta os elementos de uma análise hierárquica de tarefas.
</p>

| <p align="center">Elemento</p> | <p align="center">Descrição</p> | 
| :--:                           | :----: | 
|**Tarefa**:     | parte do trabalho que precisa ser realizada, pode ser definida em termos de objetivos e subobjetivos|
|**Objetivo**:   | é um estado específico, um estado final, definido por eventos ou por valores fisicamente observáveis de variáveis, que atuam como critério de alcance do objetivo |
|**Subobjetivo**:| decomposição de objetivos complexos, utilizados para identificar quais subobjetivos são mais difíceis de atingir, visto que limitam ou mesmo impedem o atingimento do objetivo maior|
|**Plano**:      | define os subobjetivos necessários para alcançar um outro objetivo maior, e a ordem em que esses subobjetivos devem ser alcançados|
|**Operação**:   | circunstâncias nas quais o objetivo é ativado (input ou entrada), pelas atividades ou ações (actions) que contribuem para atingi-lo e pelas condições que indicam o seu atingimento (feedback)|
<div align="center">
<p> <b>Tabela 1</b>: Elementos de uma HTA (Fonte: GOMES, Larissa. 2023). </p>
</div>


<p align="justify">
A Figura 1 apresenta os elementos de um diagrama HTA.</p>

<img title="a title" alt="Elementos HTA" src="https://raw.githubusercontent.com/Interacao-Humano-Computador/2023.1-VideoLAN/main/docs/img/analise_tarefas/elementosHTA.png" width="100%">

<div align="center">
<p> <b>Figura 1</b>: Elementos de um diagrama HTA (Fonte: GOMES, Larissa. 2023). </p>
</div>

<p align="justify">Os planos podem possuir relações entre os subobjetivos, como: sequência fixa (um objetivo deve ser atingido antes do próximo); regra de seleção ou decisão (quais objetivos que deverão ser atin-gidos dependem das circunstâncias); ou em paralelo (mais de um objetivo deve ser atingido ao mesmo tempo). A Figura 1 apresenta a forma gráfica de representação dessas relações.
</p>

### Motivo da escolha

<p align="justify">Este método foi escolhido para analisar a tarefa <b>Acessar dados financeiros pessoais</b> pois é uma tarefa com muitas possibilidades, porém todas possuem uma mesma ordem de operações. Tendo isso em vista, a separação em subobjetivos hierárquicos seria a melhor forma de entender o comportamento do usuário.

### Análise da Tarefa: Acessar dados financeiros pessoais
A tarefa "acessar dados financeiros pessoais" é a principal oferecida pelo BCB, tendo em vista que é um site voltado mais para informações financeiras. A representação em tabela e em diagrama da HTA da tarefa pode ser vista na Tabela 2 e Figura 2, respectivamente.

## Árvore de Tarefas Concorrentes (CTT)

### Introdução

<p align="justify">A Árvore de Tarefas Concorrentes (CTT) é uma técnica de design de interação que permite representar as tarefas que podem ser executadas simultaneamente pelo usuário em um sistema interativo. A técnica do CTT foi desenvolvida como uma extensão da Árvore de Tarefas (AT), uma metodologia que permite representar as tarefas que o usuário precisa realizar para atingir seus objetivos em um sistema.</p>

<p align="justify"> Nesse modelo existem 4 tipos de tarefas:

- Tarefas do usuário, realizadas fora do sistema;
- Tarefas do sistema, em que o sistema realiza um processamento sem interagir com o usuário;
- Tarefas interativas, em que ocorrem diálogos usuário-sistema;
- Tarefas abstratas, que não são tarefas em si, mas sim uma representação de uma composição de tarefas que auxilie a decomposição.

Assim como na análise de tarefas haverão diferentes níveis hierárquicos.</p>

### Motivo da Escolha

<p align="justify">A técnica de Árvore de Tarefas Concorrentes (CTT) foi escolhida como método de avaliação das tarefas dos usuários, pois:

- Permite identificar quais tarefas podem ser realizadas ao mesmo tempo pelo usuário, sem que uma interfira na outra. Isso é importante para otimizar a interação e reduzir o tempo de conclusão das tarefas;
- Permite organizar as tarefas de forma hierárquica, o que ajuda a entender a relação entre as tarefas e a priorizar aquelas que são mais importantes para o usuário;
- Permite identificar os pontos em que o usuário precisa tomar uma decisão, o que ajuda a entender melhor o comportamento do usuário e a projetar uma interface mais intuitiva e fácil de usar;
- Permite visualizar de forma clara as relações entre as tarefas e as dependências entre elas. Isso ajuda a entender o fluxo de trabalho do usuário.</p>


### Nomenclaturas utilizadas no CTT

<p align="justify">Foi demonstrado como seriam as atividades com árvores de tarefas concorrentes (CTT), onde alguns símbolos foram utilizados para poder representar a ordem das tarefas. Sendo eles:

- T1 >> T2: Tarefa 2 iniciará após o término da tarefa 1;
- T1 ||| T2: Especifica que as tarefas 1 e 2 podem ser realizadas em qualquer ordem ou ao mesmo tempo;
- T1 []>> T2: Tarefa 2 iniciará após o término da tarefa 1 e a informação da tarefa 1 é passada para a tarefa 2.</p>

Essas relações entre tarefas podem ser observadas nas Figuras 2 e 3, logo a seguir.

### CTT Emitir Boleto de Multas

### CTT Aprender Sobre o Financeiro

<p align="justify"> emitir boleto de multas,aprender sobre o financeiro(https://www.bcb.gov.br/cidadaniafinanceira/cursos)</p>

## Referência Bibliográfica

[1] SIMONE DINIZ JUNQUEIRO BARBOSA, BRUNO SANTANA DA SILVA, Interação Humano-Computador, 1a. Edição, Editora Campus, 2010. (Versão grátis disponível em: https://docplayer.com.br/63299367-Interacao-humano-computador.html). Acessado em: 06/05/2023.

## Bibliografia

[1] SALES, André Barros. Apresentação Cap6 . Disponível em: https://aprender3.unb.br/pluginfile.php/2523447/mod_resource/content/4/Apresentacao%20cap06.pdf. Acesso em: 06 de Maio de 2023;
[2] Banco Central do Brasil. Cursos Online . Disponível em: https://www.bcb.gov.br/cidadaniafinanceira/cursos. Acesso em: 06 de Maio de 2023;

## Histórico de Versões

| <p align="center">Data</p> | <p align="center">Versão</p> | <p align="center">Descrição</p> | <p align="center">Autor(es)</p> | <p align="center">Data de revisão</p> | <p align="center">Revisor(es)</p> |
| :--:                       | :----: | :-------: | :---: | :-------------: | :-----: |
| 06/05/2023 | `1.0`  | Criação da introdução e escolha das tarefas | [Larissa Gomes](https://github.com/larigs) | 06/05/2023 | [Rafael Bosi](https://github.com/StrangeUnit28) |
| 08/05/2023 | `1.1`  | Adição do CTT e correção de alguns pontos | [Rafael Bosi](https://github.com/StrangeUnit28) | 08/05/2023 | [Larissa Gomes](https://github.com/larigs) |
</div>
