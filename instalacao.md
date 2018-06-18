---
description: Descrição de como se instala o LoremBot
---

# Instalação

## Dependencias

Para rodar o lorem-bot voce precisa instalar a versão 3 da linguagem python.

Obtenha mais ajuda em: [https://docs.python.org/3/using/index.html](https://docs.python.org/3/using/index.html)

## Processo de Instalação

### 1. Obtenha o pacote

Na pasta do seu projeto, instale o pacote através do pip.

```text
pip3 install lorem-bot
```

Todas as dependencias tamém serão instaladas.

### 2. Gere o Projeto

Utilize o comando:

```text
setup.py build
```

Será criada a seguinte estrutra de arquivos:

```text
./requirements.txt
./models.py
./tasks.py
./settings.py
./boot.py
./commands.py
./settings.py
```

### 3. Token

No arquivo settings.py, insira seu token de comunicação com o chatbot.

```text
TOKEN = "YOUR TOKEN"
```

Voce também pode definir outras configurações para o intervalo de busca de updates e o timeout das mensagens.

```python
settings = Settings(token=TOKEN, commands=COMMANDS, interval=0.5, timeout=100)
```

Inicialize o serviço para obtenção de updates, conforme:

```python
def main():
    updater = TelegramService() messaging = Messaging()
    
    # Attaching obsersers to chatbot
    updater.attach(messaging)
    updater.attach(payments)
    updater.attach(responsing)
    updater.fetch_updates()
    

if __name__ == '__main__': main()

```



