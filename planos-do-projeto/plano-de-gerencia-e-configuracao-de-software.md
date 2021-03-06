# Plano de Gerência e Configuração de Software

**Histórico de Revisão**

| **Data** | **Versão** | **Descrição** | **Autor** |
| --- | --- |
| 11/06/18 | 1.0 | Adicionando Introdução, Ferramentas e Políticas. | Igor Gabriel |

## 1. Introdução

 Neste documento, será descrito o planejamento dos principais itens relevantes em relação a Gerência de Configuração de _Software_, com o objetivo de apresentar as ferramentas utilizadas na configuração do projeto além dos padrões de organização e nomenclatura a serem utilizados.

## 2. Item de Configuração

 Um item de configuração é um artefato produzido no projeto que necessite de gerenciamento \(itSMF, 2002\). Portanto, para determinar quais ferramentas serão utilizadas e métodos de versionamento, determina-se quais serão os artefatos que se tornarão itens de configuração. Para o contexto deste projeto, serão considerados dois principais itens de configuração a serem mantidos:

* **Documentos:** Arquivos em texto contendo planejamentos, descrição do produto e projeto e outros semelhantes.
* **Código:** É um dos artefatos resultantes da execução do projeto, sendo composto por um conjunto de arquivos texto, que conterá o código de uma ou mais linguagens de programação, por exemplo Python.

## 3. Ferramentas

| **Ferramenta** | **Descrição** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Git/Github |  Sistema de versionamento em nuvem. |
| Python | Linguagem de programação utilizada para o desenvolvimento do projeto. |
| Gitbook | O _gitbook_ é um gerador de sites com base em arquivos _markdown._ |
| Zenhub |  Ferramenta para controle e distribuição de _issues_/histórias. |
| Atom |  Editor de Texto. |
| Pip | _Pip_ é um sistema de gerenciamento de pacotes usado para instalar e gerenciar pacotes de software escritos na linguagem de programação _Python_. |
| SQLite3/Python | Biblioteca para gerenciamento de banco de dados SQLite. |
| SQLAlchemy Migrate | fornece uma maneira de lidar com mudanças no esquema do banco de dados em projetos SQLAlchemy. |

## 4. Políticas

### 4.1 Política de Contribuição na Documentação\(GitBook\)

 Com o intuito de manter a rastreabilidade e controle das alterações feitas no _gitbook_ \( gerador de sites com base em arquivos _markdown_\) do projeto, o _gitbook_ já fornece essa funcionalidade de rastreabilidade através de uma integração com o _github_, onde para cada modificação realizada em certo documento é gerado um _commit_ em nosso repositório, dedicado a armazenar esses documentos gerados no _gitbook._ 

### 4.2 Política de Commits

Os _commits_ devem ser atômicos, representando uma funcionalidade ou parte dela. A mensagem deve descrever o que foi produzido, de forma sucinta. Além disso, o _commit_ deverá ser em inglês.

### 4.3 Política de _Branches_

Haverá apenas um repositório com uma branch principal \(master\) e uma branch auxiliar de desenvolvimento \(devel\). Será necessária a criação de branches auxiliares para o desenvolvimento de cada história de usuário ou história técnica, essas serão ramificações da devel. Após o término da funcionalidade, os desenvolvedores responsáveis deverão mesclar o conteúdo da _branch_ auxiliar na qual a funcionalidade foi desenvolvida com a branch auxiliar de desenvolvimento \(devel\). Essa tarefa deve ser realizada com o comando merge. A funcionalidade deverá ser integrada a master através do pull request, onde o qualidade do código será analisada.

### 4.4 Política de Aprovação do Código

 O código será aprovado caso seja funcional e siga todas as especificações da folha de estilo com a aplicação das técnicas de programação, tais como: identação, presença de loggings, comentários, ou seja, o uso de programação defensiva. Além disso o código deverá conter uma cobertura de testes mínima determinada pelo time, assim como, satisfazer todos os requisitos das ferramentas de análise de código. O Scrum Master da sprint em questão deverá revisar o código presente em cada pull request. Caso não obedeça às regras e não seja explicado o não uso de uma das especificações estabelecidas acima o **Scrum Master deverá recusar o pull request** a branch mastere voltar a branch devel para a última versão estável.

