# Plano de Medição

## Contexto

O LoremBot é uma aplicação criada no contexto da disciplina Desenho de Software da Universidade de Brasília (UnB) - Faculdade do Gama (FGA), que visa criar um framework que facilite a criação de bots para o telegram.

## Problema

Para melhorar e garantir qualidade em um determinado projeto de software é necessário primeiramente entender e definir os processos, produtos e recursos envolvidos neste projeto, sendo assim o Plano de Medição é de grande ajuda para definir os pontos positivos que devem ser mantidos e os pontos que podem melhorar e devem ser alterados no projeto. Considerando todos estes fatores a equipe de desenho precisa gerenciar a equipe de desenvolvimento e se ater aos prazos e requisitos da matéria além de manter o nível de qualidade.


## Planejamento de Medição

A abordagem GQM (Goal Question Metric) será adotada para identificar as métricas que atinjam os objetivos propostos para o contexto do projeto LoremBot.


# 1 Plano de medição - Conceitual
## Código
|||
| --- | --- |
|**Analisar**|o código|
|**para**|entender e garantir|
|**os pontos**|manutenabilidade e eficácia|
|**pelo ponto de vista**|de desenvolvedor|
|**sob o contexto**|do projeto LoremBot|

###  Abstraction Sheet

|||
| --- | --- |
|**Foco na Qualidade**|**Fatores de Variação**|
|**Q.1** Complexidade Ciclomática <br> **Q.2** Duplicação de código|Padronização do código <br> Complexidade do Software <br> Experiência com a tecnologia|
|**Hipóteses de Baseline**|**Impacto nas hipóteses de ​Baseline**|
|**Q.1** Complexidade Ciclomática < 4 <br> **Q.2** Duplicação de código em nível regular|Fator de complexidade bom, com boa manutenibilidade <br> Necessidade de retrabalho|

# 2 Plano de medição - Operacional

#### Código
 - Quão manutenível é o código?
 - Quão fiel o código é às boas práticas de programação?

# 3 Plano de medição - Quantitativo

### Quão manutenível é o código?
 - Erros do flake8 por arquivo.
 - Métodos com alto número de argumentos.
 - Arquivos com alto número de linhas.
 - Blocos de código idênticos.
 - Blocos de código semelhantes.
 - Classes com alto número de métodos.
 - Métodos com alto número de linhas.
 - Quantidade de estruturas de decisão muito aninhadas.

### Quão fiel o código é às boas práticas de programação?
 - Erros do flake8 por arquivo.
 - Blocos de código idênticos.
 - Blocos de código semelhantes.
 - Métodos com alto número de linhas.
 - Métodos com vários 'return'.

# Métricas

| **Métrica**           | **Erros do flake8 por arquivo** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a simplicidade na leitura do código|
| **Obtenção**             | A ferramenta de integração contínua executa o flake8 nos arquivos do projeto sempre que código é mandado ao reprositório|
| **Escala**              | Absoluta  |
| **Análise**             | Caso ocorra ao menos um erro deverá haver uma refatoração do código |

<br>

| **Métrica**           | **Métodos com alto número de argumentos** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a modularidade|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Arquivos com alto número de linhas** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a modularidade do código|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Blocos de código idênticos** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a simplicidade de leitura do código|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Blocos de código semelhantes** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a simplicidade de leitura do código|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Classes com alto número de métodos** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a visibilidade das classes|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Métodos com alto número de linhas** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a visibilidade dos métodos|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Quantidade de estruturas de decisão muito aninhadas** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a simplicidade de leitura do código|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|

<br>

| **Métrica**           | **Métodos com vários 'return'** |
|---------------------|----------|
| **Objetivo de Medição** | Garantir a simplicidade de leitura do código|
| **Obtenção**             | O code climate gera alertas para cada ocorrência|
| **Escala**              | Absoluta  |
| **Análise**             |  Caso ocorra ao menos uma issue deverá haver uma refatoração do código|
