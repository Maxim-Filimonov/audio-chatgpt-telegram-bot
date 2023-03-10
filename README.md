# Telegram bot transcriber

Telegram bot to use transcribe chat messages using whisper ai from openAI.

The bot has been deployed on [Railway](https://railway.app), and it works amazingly! 🚀
You can deploy your own bot, or try out mine! [@AudioGPT_bot](https://t.me/whisper_to_me_bot)

## Features

* Use voice or file attachments to interact with the bost
* Type or speak in many different languages 
* Fast answers (2-3 seconds)


## Bot commands

* `/reset` – start new dialog
* `/help` – show help
* `/start` – register to the service


## Setup for deployment

1. Register the new bot with [@BotFather](https://core.telegram.org/bots/tutorial) and retrieve the bot key
2. Register to [OpenAI](https://openai.com)  and retrieve the key
3. Register to [Railway](https://railway.app) and use the template I created to set up your own configuration:

   [![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/rxWKuE?referralCode=c9RZUJ)
   
If you want to run locally, you will still need to set up a PostgreSQL database and configure the following env variable in `app/.env` file:
```YAML
    API_TELEGRAM = ""
    OPENAI_TOKEN = ""

    MODE = 'polling'
    PORT = '8443'
    CHATGPT_MODEL = "gpt-3.5-turbo"

    PGDATABASE = ""
    PGHOST = ""
    PGPASSWORD = ""
    PGPORT = ""
    PGUSER = ""

```




