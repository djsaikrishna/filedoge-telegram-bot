# Project Title

Telegram files to FileDoge upload - bot, returning download links after upload.

![Logo](./static/filedoge.png)

## Tech Stack

- Backend: Node
- Framwork: Express
- Bot SDK: Telegraf

## Installation

Clone and Install the required packages for filedoge-telegram-bot with npm

```bash
git clone https://github.com/kurdi-dev/filedoge-telegram-bot.git
cd filedoge-telegram-bot
npm i
```

## Run Locally

Clone the project

```bash
git clone https://github.com/kurdi-dev/filedoge-telegram-bot.git
```

Go to the project directory

```bash
cd filedoge-telegram-bot
```

Install dependencies

```bash
npm install
```

Update `.env` file, see Environment Variables section

Start the server

```bash
  npm run start
```

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file, check `.env.example`.

`TELEGRAM_TOKEN`: Api token given by Telegram BotFather.

`BOT_SERVER_URL`: your production server URL, leave it blank while developing localy, check setWebhook method inside `index.js:228`

## Deployment

# Deploy to Heroku

To deploy this project on Heroku, after loging in run

```bash
heroku create
```

Update/Set Environmental Varibales:

```bash
heroku config:set TELEGRAM_TOKEN=<your botfather bot token>  BOT_SERVER_URL=<your newly created Dyno URL>  PORT=8443
```

Then, push the code to Heroku

```bash
git push heroku main
```

## License

[MIT](https://choosealicense.com/licenses/mit/)