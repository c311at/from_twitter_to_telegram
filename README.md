## Twitter >> Telegram

## installing Heroku

#### The Easy Way

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)


### Auto post tweets from Twitter, to a Telegram Channel bot

This script simply takes a twitter user name, and fetches the latest tweets
from their timeline. Then reposts those tweets to a telegram channel(via a bot)

#### Requirements:
You need Twython installed. Twython is a twitter-python API

#### Notes:

Just create a Telegram Bot(takes only seconds) and add your new bot as an
administrator to your Channel.

Edit the 'SETTINGS.py' file and update it with your own information.

The script makes a "pickled" file that holds the tweet ID of the latest tweet it 
recieved. That way, we can compare the tweet ID later, and make sure that we
only get the newest tweets, since last time we ran the script.

You can schedule the script to run with something like using cron jobs, 
every 10 min for example. I run mine at every 5 min for my current bot.
