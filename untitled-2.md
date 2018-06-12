# Documento de Arquitetura

| **Data** | **Versão** | **Descrição** | **Autor** |
| --- | --- |
| 11/06/18 | 1.0 | Introdução, Representação Arquitetural | Indiara Duarte |

## 1. Introdução

### 1.1. Objetivos

Este documento fornece uma visão geral da arquitetura abrangente do LoremBot. Apresenta várias visualizações de arquitetura diferente para descrever os diferentes aspectos do sistema. Destina-se a transmitir aos interessados as decisões arquiteturais significativas que foram tomadas.

### 1.2. Escopo

Este documento descreve os estilos e decisões arquiteturais do framework LoremBot.

### 1.3. Acrônimos 

| **Acrônimo** | **Definição** |
| --- | --- | --- |
| API | Application Programming Interface |
| ORM | Object-Relational Mapping |

## 2. Representação Arquitetural 

### 2.1. Implementação

O framework foi desenvolvido utilizando o padrão MVC \(Model-View-Controller\) e escrito em Python. As vantagens na utilização dessa arquitetura são:

* Separação de responsabilidades
* Reutilização de código

**Models** - Representam entidades responsáveis pela manipulação de dados persistentes em banco de dados da aplicação. No LoremBot, as models serão utilizadas para definir uma interface de comunicação com o banco de dados, através da ORM SQLAlchemy. Dessa maneira, é possível descrever na classe que representa uma modelo quais são os atributos.

**Controller** - As _controllers_ promoverão a ligação entre as _models_ e o servidor do Telegram através do envio de updates. No LoremBot, as _controllers_ são responsáveis pelo processamento dos comandos enviados pelo usuário ao chatbot. Dessa forma, será possível tratar os comandos do usuário e devolver alguma resposta.

### 2.2. Integração

A integração do LoremBot com o servidor do Telegram

### 2.3. Banco de Dados

Para persistência de dados, o LoremBot faz uso do sistema gerenciador de banco de dados  SQLite, onde a base fica guardada em um arquivo local do projeto. O SQLite possui capacidade de armazenamento apenas de dados simples **\(colocar tipos suportados\).**

O desenvolvedor não necessita escrever queries em formato SQL pois o framework oferece uma API de comunicação com o banco de dados utilizando a ORM SQL Alchemy. Tal ORM também permite que o desenvolvedor possa fazer alterações na estrutura do banco de dados utilizando _migrations_ que são estruturas de descrição para alteração do banco de dados. Tais alterações podem ser criar ou remover tabelas, criar ou remover colunas  de tabelas, etc.

### 2.4. Restrições

A escolha arquitetural também levou a identificação de algumas restrições:

**Escalabilidade**: Essa restrição é justificada pelo fato de que a arquitetura montada atualmente poderia gerar impacto no desempenho dos chatbots e a comunicação com o servidor. 

**Integrações**: O framework se integra apenas com a API do Telegram para criação de chatbots. 

## 3. Artefatos Arquiteturais

### 4.1. Funcionalidades 

A descrição das funcionalidades do LoremBot são apresentadas na forma de histórias de usuário, no repositório do projeto. Elas possuirão critérios de aceitação que descrevem de forma técnica como deverá ser desenvolvida a funcionalidade, para que, dessa forma, seja cumprido os planos de gerenciamento e qualidade do projeto.

Os artefatos para esta visão são:

* [Histórias de Usuário](https://github.com/DSW12018/LoremBot#boards?repos=136768484)
* [NFR](https://lorembot.gitbook.io/docs/~/edit/primary/nfr)

### 4.2. Integrações

Os artefatos de integração descrevem a decomposição do sistema, bem como as formas de comunicação entre os módulos.

O documentos que será disponibilizado para essa visão é:

* Diagrama de Classes



