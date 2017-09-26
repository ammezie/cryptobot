# cryptobot

A bot to compare cryptocurrencies

## Getting Started

Clone the project repository by running the command below if you use SSH

```bash
git clone git@github.com:ammezie/cryptobot.git
```

If you use https, use this instead

```bash
git clone https://github.com/ammezie/cryptobot.git
```

## Install Dependencies

`cd` into the project directory and run:

```bash
composer install
```

Duplicate `.env.example` and rename it `.env`

Run:

```bash
php artisan key:generate
```

## Create a Slack app

Visit the [Slack API](https://api.slack.com/apps?new_app=1) website in order to create a new Slack app. Then visit [https://botman.io/2.0/driver-slack](https://botman.io/2.0/driver-slack) to see how to configure your app. Once you've installed your app, paste the `Bot User OAuth Access Token` in `.env`:

```txt
SLACK_TOKEN=YOUR_SLACK_BOT_USER_TOKEN
```

## Create a Telegram bot

Visit [https://core.telegram.org/bots](https://core.telegram.org/bots) to create a Telegram bot. Then visit [https://botman.io/2.0/driver-telegram](https://botman.io/2.0/driver-telegram) to see how to configure your bot. Then paste your `API Token` in `.env`:

```txt
TELEGRAM_TOKEN=YOUR-TELEGRAM-TOKEN
```

Finally, run:

```bash
php artisan serve
```

and visit [http://localhost:8000/](http://localhost:8000/) to see the application in action.