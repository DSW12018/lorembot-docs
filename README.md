---
description: ué
---

# Bem-Vindo

## 1. Introdução

### 1.1. Objetivos

### 1.2. Escopo

Este documento descreve os estilos e decisões arquiteturais do framework LoremBot.

### 1.3. Acrônimos

| Acrônimo | Definição |
| --- | --- | --- |
| API | Application Programming Interface |
| ORM | Object-Relational Mapping |

## 2. Representação Arquitetural

### 2.1. Implementação

O framework foi desenvolvido utilizando o padrão MVC \(Model-View-Controller\) e escrito em Python. As vantagens na utilização dessa arquitetura são:

* Separação de responsabilidades
* Reutilização de código

**Models** - Representam entidades responsáveis pela manipulação de dados persistentes em banco de dados da aplicação. No LoremBot, as models serão utilizadas para definir uma interface de comunicação com o banco de dados, através da ORM SQLAlchemy. Dessa maneira, é possível descrever na classe que representa uma modelo quais são os atributos.

**Controller** - 

View - 

