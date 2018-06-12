# Proposta

| Data | Versão | Descrição | Autor |
| --- | --- |
| 12/06/18 | 1.0 | Ideia, Implementação | Kairon Velozo |

## 1. Ideia

Desenvolvimento de um framework escrito em Python ou Ruby para criação de chatbots, prontos para integração com as plataformas Facebook Messenger e Telegram.

**O nosso framework agiria como um intermediário \(middleware\) entre as SDKs do Messenger e o Telegram e o código escrito pelo usuário para criar os chatbots.**

## 2. Implementação

Nós iremos desenvolver um servidor web para receber as requisições dos servidores do facebook e do telegram. irá receber a requisição e irá tratar essa requisição delegando para as SDK’s a ação final de acordo com a mensagem.  


![Diagrama de Integra&#xE7;&#xE3;o de M&#xF3;dulos do Framework](https://docs.google.com/drawings/u/1/d/sjT5PXK90cT8CLK-CUN4GJw/image?w=531&h=330&rev=277&ac=1)



