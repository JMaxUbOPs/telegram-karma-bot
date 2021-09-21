# Telegram Karma Bot
Telegram Bot that watches and manages karma for everything

Inspired by leprosorium.ru users.

## Installation

Tested on CentOS 7 (for **Ubuntu/Debian** replace `yum` with `apt-get` below):

``` 
python3 -m pip install redis
yum install redis python3-virtualenv
git clone https://github.com/br0ziliy/telegram-karma-bot.git
cd ./telegram-karma-bot
virtualenv python3
source python3/bin/activate
pip3 install telepot
```

Now go and talk to `@BotFather` bot in your Telegram client to create your own
bot. `@BotFather` will guide you through the process. Hint: use `/newbot`
command. If everything goes well, you'll get a bot token which looks like this:
`12345678:xxxxxxxxxxxxxxxxxxxxxxxxx`. Open `bot.py` and put your token near the
top of the file (look for `BOT_TOKEN` variable).

## Usage

Make sure redis is started:

```
systemctl start redis
```

Run the bot:

```
python3 bot.py
```

That's it!
