<div class="body">

# Guia de Estilo

## Introdução

<div align="justify">

&emsp;&emsp; De acordo com Simone Barbosa e Bruno Diniz [1], um <b>Guia de Estilo</b> reune os princípios e as diretrizes adotados em um projeto. Tratando-se de um registro das principais decisões de design tomadas, de forma que elas não se percam, sendo assim efetivamente incorporadas no produto final. 

&emsp;&emsp; Para a realização do guia de estilo, foi adotada uma abordagem baseada nos pontos negativos identificadas durante a [Avaliação Heurística]() do site. Para desenvolver as melhorias foi seguido os princípios definidos no [Princípios Gerais do Projeto](), priorizando a simplicidade nas estruturas das tarefas, consistência e padronização, promoção da eficiência do usuário na realização da tarefa. Entretanto, mesmo priorizando esses princípios, os demais disponíveis no documento de [Princípios Gerais do Projeto]() também serão seguidos. O objetivo é aprimorar a experiência do usuário, proporcionando uma interface intuitiva, eficiente e agradável.

### Objetivo, Conteúdo e Organização do guia de estilo 

&emsp;&emsp; O objetivo de um guia de estilo é servir de ferramenta de comunicação entre os membros da equipe de design e também com a equipe de desenvolvimento. As decisões de design devem ser facilmente consultadas e reutilizadas nas discussões sobre extensões ou versões futuras do produto. 

&emsp;&emsp; Marcus [3] apresenta os elementos que um guia de estilo. Este artefato deve incorporar decisões de design envolvendo os principais elementos e considerações de design de interface. Fazem parte de um guia de estilo os seguintes elementos:

 - <b>Layout:</b>

   Proporção e grids   
   Uso de metáforas espaciais   
   Design gráfico de exibidores e ferramentas 
   
 - <b>Tipografia e seu uso em diálogos, formulários e relatórios</b>

 - <b>Simbolismo:</b> 

   Clareza e consistência no design de ícones  

 - <b>Cores:</b> 

   Os dez mandamentos sobre o uso de cores   

 - <b>Visualização de informação:</b> 

   Design de gráficos, diagramas e mapas   

 - <b>Design de telas e elementos de interface (widgets)</b>
 
 
</dl>

&emsp;&emsp; Esses elemento serão utilizados para cumprir o objetivo deste guia de estilo, fornecendo orientações sobre os elementos de interface, interação e ação utilizados no site do <b>Banco Central do Brasil</b>. 

&emsp;&emsp; O guia de estilo seguirá a estrutura proposta por Marcus [3] e Mayhew [2], onde é dividada em tópicos e subtópicos, os tópicos a serem seguidos são: Introdução, Resultados de análise, Elementos de interface, Elementos de interação, Elementos de ação e Vocabulário e padrões. Os subtópicos seguem os elementos descritos de um guia de estilo. O objetivo final deste artefato é padronizar a aparência e a interação do site, garantindo uma experiência do usuário consistente e de alta qualidade.

### Público Alvo

&emsp;&emsp;Um guia de estilo destina-se a todos os desenvolvedores, designers e equipes envolvidas no projeto de desenvolvimento de uma aplicação. No contexto atual, este guia será utilizado pelos estudantes de Interação Humano Computador(IHC) da UnB-FGA, visando cumprir com a análise e re-design propostos pela matéria.

### Como utilizar o Guia

&emsp;&emsp;Este documento deve ser consultado sempre que houver uma decisão de design ou desenvolvimento que afete o projeto. Ele também deve ser utilizado como referência para manutenção e atualização do site. Tendo como propósito ser utilizado unicamente para o desenvolvimento do projeto de IHC.

### Como manter o Guia

Reconhecemos que a criação do guia de estilo é um processo contínuo e dinâmico. Portanto, além das melhorias iniciais, planejamos fornecer manutenção regular ao guia de estilo à medida que o projeto evolui e novos insights são obtidos. Essa abordagem nos permitirá adaptar e aprimorar constantemente a interface, mantendo-a alinhada com as necessidades e expectativas dos usuários.
&emsp;&emsp;Sempre que houver uma decisão de design ou desenvolvimento que afete o site, o Guia de Estilo deve ser atualizado para estar de acordo com essas alterações. Sendo importante ressaltar a necessidade de ser atualizado regularmente para garantir que a padronização seja mantida em todo o site.

## Resultados de análise

&emsp;&emsp;Pelo [questionário](https://interacao-humano-computador.github.io/2023.1-BancoCentral/#/questionarios/questionario_01) foi possivel identificar que o principal ambiente de trabalho do usuário é um computador desktop ou um notebook. 

## Elementos de interface, interação e ação

&emsp;&emsp;O [Figma 1](https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FqfTjVMd6eqIsLqmj7Ru9gF%2FGuia-de-estilo---BCB%3Ftype%3Ddesign%26node-id%3D0%253A1%26t%3DhnymK0IpI8aUFX9Q-1) apresenta os elementos do guia de estilo a ser seguido neste projeto. Os elementos estão divididos em 3 grupos:

- Elementos de interface:
    1. Disposição espacial e grid
    2. Janelas
    3. Tipografia
    4. Cores

- Elementos de interação: 
    1. Estilos de interação 
    2. Seleção de um estilo 
    3. Aceleradores (teclas de atalho) 

- Elementos de ação 
    1. Preenchimento de campos 
    2. Seleção
    3. Ativação

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FqfTjVMd6eqIsLqmj7Ru9gF%2FGuia-de-estilo---BCB%3Ftype%3Ddesign%26node-id%3D0%253A1%26t%3DhnymK0IpI8aUFX9Q-1" allowfullscreen></iframe>

<div align="center">
<p> <b>Figma 1</b>: Guia de Estilo (Fonte: ALVISSUS, Giovanni; GOMES, Larissa. 2023). </p>
</div>


## Vocabulário e padrões

<b>Terminologia:</b> Cabe ao designer decidir o quanto as semelhanças e diferenças na terminologia utilizada pelos usuários devem se refletir em consistência ou quebra de consistência na interação e, posteriormente, na interface com o usuário [1]. Tendo isso em vista, durante esse projeto deve ser ponderado o uso de termos técnicos, utilizando apenas em casos extremamente necessários, priorizando o uso de termos mais comuns aos usuários, visando tornar o sistema mais intuitivo.

<b>Tipos de tela (para tarefas comuns):</b> As telas devem seguir os padrões especificados, se atentando ao tipo de conteúdo da página a ser criada para a seleção da interface, havendo 4 opções de tela. Também deve ser seguido o padrão dos elementos de interface, interação e ação criados no Figma 1.

<b>Sequências de diálogos:</b> Em uma sequência de diálogos devem ser gerados feedbacks e confirmações após uma operação ser finalizada ou realizada.

</div>

## Conclusão


Além disso, estamos utilizando protótipos de [baixa]() e [alta]() fidelidade para validar as soluções propostas. Esses protótipos nos permitem testar e interar o design, considerando diferentes fluxos de interação, layouts e elementos visuais. Com base nos resultados obtidos, faremos ajustes e refinamentos no guia de estilo, garantindo que as [Metas de Usabilidade]() sejam alcançadas.


## Referência Bibliográfica

[1] SIMONE DINIZ JUNQUEIRO BARBOSA, BRUNO SANTANA DA SILVA, Interação Humano-Computador, 1a. Edição, Editora Campus, 2010. (Versão grátis disponível em: https://docplayer.com.br/63299367-Interacao-humano-computador.html). Acessado em: 06/05/2023.

[2] Marcus, A. Graphic Design for Electronic Documents and User Interfaces. New York,
NY: Th e ACM Press, 1992.

[3] Mayhew, D. Th e Usability Engineering Lifecycle: a practitioner’s handbook for user interface
design. San Francisco, CA: Morgan Kaufmann, 1999.

## Bibliografia

[1] Banco Central do Brasil.  Disponível em: https://www.bcb.gov.br. Acesso em: 15 de Maio de 2023;

[2] FIGMA. Disponível em: [FIGMA](https://figma.com). Acesso em: 12 de Maio de 2023.

## Histórico de Versões

| <p align="center">Data</p> | <p align="center">Versão</p> | <p align="center">Descrição</p> | <p align="center">Autor(es)</p> | <p align="center">Data de revisão</p> | <p align="center">Revisor(es)</p> |
| :--:                       | :----: | :-------: | :---: | :-------------: | :-----: |
| 06/05/2023 | `1.0`  | Criação da introdução e escolha das tarefas | [Larissa Gomes](https://github.com/larigs) | 06/05/2023 | [Rafael Bosi](https://github.com/StrangeUnit28) |
| 15/05/2023 | `1.1`  | Criação do figma | [Larissa Gomes](https://github.com/larigs) e [Giovanni Alvissus](https://github.com/giovanni1106) | 06/05/2023 | [Rafael Bosi](https://github.com/StrangeUnit28) |
| 03/07/2023 | `2.0`  | Correção do figma | [Giovanni Alvissus](https://github.com/giovanni1106) | 03/07/2023 | [Larissa Gomes](https://github.com/larigs) |
| 15/05/2023 | `2.1`  | Correção dos textos | [Larissa Gomes](https://github.com/larigs) e [Giovanni Alvissus](https://github.com/giovanni1106) | 06/05/2023 | [Rafael Bosi](https://github.com/StrangeUnit28) |

</div>
