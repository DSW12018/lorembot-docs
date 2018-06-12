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

## 

