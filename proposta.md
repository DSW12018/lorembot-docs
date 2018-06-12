# Proposta

| Data | Versão | Descrição | Autor |
| --- | --- |
| 20/05/18 | 1.0 | Ideia, | Equipe |

## 1. Ideia

Desenvolvimento de um framework escrito em Python ou Ruby para criação de chatbots, prontos para integração com as plataformas Facebook Messenger e Telegram.

O nosso framework agiria como um intermediário \(middleware\) entre as SDKs do Messenger e o Telegram e o código escrito pelo usuário para criar os chatbots.

## 2. Implementação

Nós iremos desenvolver um servidor web para receber as requisições dos servidores do facebook e do telegram. irá receber a requisição e irá tratar essa requisição delegando para as SDK’s a ação final de acordo com a mensagem.  


![Diagrama de Integra&#xE7;&#xE3;o de M&#xF3;dulos do Framework](https://docs.google.com/drawings/u/1/d/sjT5PXK90cT8CLK-CUN4GJw/image?w=531&h=330&rev=277&ac=1)

## 2. Spots

### 2.1 Frozen

* Integração com Telegram
* Integração com Messenger
* SQLite para armazenamento de dados

### 2.2 Hot

* Models para armazenamento de dados
* Comandos de ação do chatbot

## 3. **Tipo do Framework**

Após a análise das funcionalidades que pretendem ser oferecidas pelo framework, identificou-se o tipo caixa cinza. O framework permitirá reúso por herança, associação dinâmica, sendo um intermediário entre os dois outros tipos de frameworks, caixa branca e caixa preta.

## 4. **Documentação**

Pretende-se elaborar uma documentação a nível de código, explicando o que cada método das classes fazem, além de criar alguns exemplos de projetos usando o framework.

## 5. **Bibliotecas**

A depender da linguagem escolhida pela equipe, poderá se utilizar as seguintes bibliotecas para a criação do framework.  


| Linguagem | Título | Descrição | URL |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Ruby | telegram-bot-ruby | Biblioteca de integração com Telegram | [https://github.com/atipugin/telegram-bot-ruby](https://github.com/atipugin/telegram-bot-ruby) |
| Ruby | Ruby Messenger | Biblioteca de integração com Facebook Messenger. | [https://github.com/netguru/messenger-ruby](https://github.com/netguru/messenger-ruby) |
| Ruby | Rack | Biblioteca para criação de servidores web. | [https://rack.github.io/](https://rack.github.io/) |
| Ruby | SQLite3/Ruby | Biblioteca para gerenciamento de banco de dados SQLite. | [https://github.com/sparklemotion/sqlite3-ruby](https://github.com/sparklemotion/sqlite3-ruby) |
| Python | Python Telegram Bot | Biblioteca de integração com Telegram. | [https://github.com/python-telegram-bot/python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) |
| Python | Python Messenger Bot | Biblioteca de integração com Facebook Messenger. | [https://github.com/hartleybrody/fb-messenger-botPython](https://github.com/hartleybrody/fb-messenger-botPython) |
| Python | SQLite3/Python | Biblioteca para gerenciamento de banco de dados SQLite. | [https://docs.python.org/2/library/sqlite3.html](https://docs.python.org/2/library/sqlite3.html) |
| Python | SQLAlchemy  | Biblioteca de mapeamento objeto-relacional SQL para Python | [http://sqlalchemy-migrate.readthedocs.io/en/latest/](http://sqlalchemy-migrate.readthedocs.io/en/latest/) |

