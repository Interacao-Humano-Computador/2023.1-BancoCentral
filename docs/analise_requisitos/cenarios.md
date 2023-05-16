<div class="body">

# Cenários

## Introdução
<p align="justify">Os cenários são descrições extremamente detalhadas do ambiente e da interação do usuário com a aplicação. Sob essa ótica, essa técnica é utilizada para descrever situações de uso, que permitem elicitar comportamentos e cenários onde os usuários passarão. Dessa forma, é uma estratégia que elicita a parte comportamental do software.</p>

## Modelo de Cenário
Para a descrição dos cenários, existem 5 formas diferentes:

- Texto narrativo
- Texto estruturado
- Diagramas
- Imagens e animações
- Simulações

<p align="justify">Foi escolhido a utilização do texto estruturado, com ligeiras adaptações para propósitos de aprendizado. A Tabela 1 a seguir é o molde utilizado para cada cenário:</p>

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Objetivo do cenário       |
| Contexto   | Detalhes da situação   |
| Recursos   | Objetos que interagem com os atores    |
| Ator       | Pessoa participante do cenário      |
| Episódios  | Sequência de ações realizadas pelos atores envolvidos no cenário |
| Restrições | Possíveis impedimentos às ações dos usuários     |
| Exceção    | Possíveis casos e eventos que fujam do comum nos episódios   |


<p> Tabela 1: Molde dos cenários (Fonte: GOBBI, Lucas. 2023).</p>
</div>

## Cenários Identificados
Os cenários identificados, tendo como base as [Personas](analise_requisitos/personas.md) desenvolvidas no projeto, estão apresentados nas Tabelas 2 a 8:

### C01: Consultar Panorama Econômico

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Consultar taxas de inflação e selic      |
| Contexto   | Local: No Trabalho <br> Tempo: Durante o dia <br> Pré-condições: Acesso à Internet   |
| Recursos   | Internet, computador e site do Banco Central    |
| Ator       | Um contador      |
| Episódios  | - O usuário acessa o site <br> - O usuário olha para a direita da tela, na área de "Panorama Econômico" <br> - O usuário analisa as tabelas |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet ou de energia   |

<p> Tabela 2: Cenário 01 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

### C02: Consultar Taxas e Conversão de Câmbio

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Consultar taxas de câmbio e calcular sua conversão     |
| Contexto   | Local: Na Faculdade <br> Tempo: Durante o dia <br> Pré-condições: Acesso à Internet   |
| Recursos   | Internet, computador e site do Banco Central    |
| Ator       | Um estudante de turismo     |
| Episódios  | - O usuário acessa o site <br> - O usuário olha para a esquerda da tela, na área de "Conversor de Moedas" <br> - O usuário seleciona "Ver todas as moedas" <br> - O usuário escolhe o valor e a moeda desejada na conversão |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet ou de energia   |


<p> Tabela 3: Cenário 02 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

### C03: Consultar Informações Econômicas do País

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Consultar relatórios acerca da economia do país     |
| Contexto   | Local: Em Outro País <br> Tempo: Durante a noite <br> Pré-condições: Acesso à Internet   |
| Recursos   | Internet, computador e site do Banco Central    |
| Ator       | Um brasileiro no exterior     |
| Episódios  | - O usuário acessa o site <br> - O usuário acessa, na barra de navegação, o item de "Publicações e Pesquisa" <br> - O usuário seleciona, dentro de "Publicações e Pesquisa", o item "Focus - Relatório de Mercado" <br> - O usuário seleciona o ícone de download <br> - O usuário analisa as informações do relatório |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet ou de energia   |


<p> Tabela 4: Cenário 03 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

### C04: Aprender Sobre Economia

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Aprender mais sobre economia, por meio de cursos especializados     |
| Contexto   | Local: Em Casa <br> Tempo: Durante a noite <br> Pré-condições: Acesso à Internet   |
| Recursos   | Internet, computador e site do Banco Central    |
| Ator       | Um estudante     |
| Episódios  | - O usuário acessa o site <br> - O usuário acessa, na barra de navegação, o item de "Acesso à Informação" <br> - O usuário seleciona, dentro de "Acesso à Informação", o item "Cidadania Financeira" <br> - O usuário seleciona, dentro de "Cidadania Financeira", o item "Cursos Online" <br> - O usuário seleciona a opção de se inscrever no curso <br> - O usuário participa, na eventual data planejada, do curso |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet ou de energia, falta de horários para o curso   |


<p> Tabela 5: Cenário 04 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

### C05: Consultar Dados da Poupança

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Consultar dados da poupança como: depósitos, retiradas e saldo total    |
| Contexto   | Local: No Trabalho <br> Tempo: Durante o dia <br> Pré-condições: Acesso à Internet e um Editor de Planilhas   |
| Recursos   | Internet, computador, site do Banco Central e Editor de Planilhas   |
| Ator       | Um contador    |
| Episódios  | - O usuário acessa o site <br> - O usuário acessa, na barra de navegação, o item de "Estatísticas" <br> - O usuário seleciona, dentro de "Estatísticas", o item "Poupança" <br> - O usuário seleciona, dentro de "Poupança", o item "Relatório de Poupança" <br> - O usuário seleciona a opção de download <br> - O usuário analisa os dados da planilha |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet, de energia ou de editor de planilhas  |


<p> Tabela 6: Cenário 05 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

### C06: Consultar Valores a Receber

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Consultar valores a receber    |
| Contexto   | Local: Em Casa <br> Tempo: Durante o dia <br> Pré-condições: Acesso à Internet   |
| Recursos   | Internet, computador, site do Banco Central   |
| Ator       | Um aposentado    |
| Episódios  | - O usuário acessa o site <br> - O usuário olha para o meio da tela na área de "Serviços" <br> - O usuário seleciona a opção de "Consulte Valores a Receber" <br> - O usuário seleciona o botão de "Consulte valores a receber" <br> - O usuário preenche seus dados <br> - O usuário realiza a consulta |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet ou de energia  |


<p> Tabela 7: Cenário 06 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

### C07: Consulta de Moedas Comemorativas

<div style="text-align: center">

| Elemento   | Descrição      |
| ---------- | ----------- |
| Objetivo   | Consultar moedas especiais e seus significados    |
| Contexto   | Local: Em Casa <br> Tempo: Durante a noite <br> Pré-condições: Acesso à Internet   |
| Recursos   | Internet, computador, site do Banco Central   |
| Ator       | Uma pessoa numismática (colecionadora de moedas)   |
| Episódios  | - O usuário acessa o site <br> - O usuário acessa, na barra de navegação, o item de "Cédulas e Moedas" <br> - O usuário seleciona, dentro de "Cédulas e Moedas", o item "Moedas" <br> - O usuário seleciona, dentro de "Moedas", o item "Moedas Comemorativas" <br> - O usuário seleciona a série de moedas desejada |
| Restrições | Fluxo de navegação intuitivo     |
| Exceção    | Falta de internet ou de energia  |

<p> Tabela 8: Cenário 07 (Fonte: GOBBI, Lucas. 2023).</p>
</div>

## Bibliografia

[1] CENÁRIOS: Rastreamento de Cenários. [S. l.]. Disponível em: <http://www-di.inf.puc-rio.br/~julio/bnncap3.pdf>. Acesso em: 07/05/2023.

## Histórico de Versões

| <p align="center">Data</p> | <p align="center">Versão</p> | <p align="center">Descrição</p> | <p align="center">Autor(es)</p> | <p align="center">Data de revisão</p> | <p align="center">Revisor(es)</p> |
|:------:|:--------:|-----------|-------|:---------:|-----------|
| 07/05/2023 | `1.0` | Criação do artefato | [Bruno Ribeiro](https://github.com/brunoriibeiro), [Igor Penha](https://github.com/igorpenhaa) e [Lucas Gobbi](https://github.com/lucasbergholz) | 08/05/2023 | [Larissa Gomes](https://github.com/larigs) |
| 08/05/2023 | `1.1` | Correção de alguns textos | [Larissa Gomes](https://github.com/larigs) | 08/05/2023 | [Lucas Gobbi](https://github.com/lucasbergholz) |

</div>