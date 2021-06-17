<h1 align=center>😈EVIL BOT😈</h1>
<img src = "https://telegra.ph/file/2345311d29a66213a9d98.jpg">

## Deploy
<p align="center"><a href="https://heroku.com/deploy?template=https://github.com/shrvan42/EvilBot"> [<img align="center" alt="Heroku" width="52px" src="https://www.nicepng.com/png/full/223-2233246_heroku-logo-salesforce-heroku.png" />].

<H2 align=center>___________</h2>

## Starting the bot.

Once you've setup your database and your configuration (see below) is complete, simply run:

`python3 -m EvilBot`


### Configuration

There are two possible ways of configuring your bot: a config.py file, or ENV variables.


If you can't have a config.py file (EG on heroku), it is also possible to use environment variables.
The following env variables are supported:
 - `API ID`: Your Api Id from [here](https://my.telegram.org).
 - `API HASH`: Your Api Hash from [here](https://my.telegram.org).
 - `ENV`: Setting this to ANYTHING will enable env variables
 - `TOKEN`: Your bot token.
 - `OWNER_ID`: An integer of consisting of your owner ID
 - `OWNER_USERNAME`: Your username

 - `DATABASE_URL`: Your database URL
 - `MESSAGE_DUMP`: optional: a chat where your replied saved messages are stored, to stop people deleting their old 
 - `LOAD`: Space separated list of modules you would like to load
 - `NO_LOAD`: Space separated list of modules you would like NOT to load
 - `WEBHOOK`: Setting this to ANYTHING will enable webhooks when in env mode
 messages
 - `URL`: The URL your webhook should connect to (only needed for webhook mode)

 - `SUDO_USERS`: A space separated list of user_ids which should be considered sudo users
 - `SUPPORT_USERS`: A space separated list of user_ids which should be considered support users (can gban/ungban,
 nothing else)
 - `WHITELIST_USERS`: A space separated list of user_ids which should be considered whitelisted - they can't be banned.
 - `DONATION_LINK`: Optional: link where you would like to receive donations.
 - `CERT_PATH`: Path to your webhook certificate
 - `PORT`: Port to use for your webhooks
 - `DEL_CMDS`: Whether to delete commands from users which don't have rights to use that command
 - `STRICT_GBAN`: Enforce gbans across new groups as well as old groups. When a gbanned user talks, he will be banned.
 - `WORKERS`: Number of threads to use. 8 is the recommended (and default) amount, but your experience may vary.
 __Note__ that going crazy with more threads wont necessarily speed up your bot, given the large amount of sql data 
 accesses, and the way python asynchronous calls work.
 - `BAN_STICKER`: Which sticker to use when banning people.
 - `ALLOW_EXCL`: Whether to allow using exclamation marks ! for commands as well as /.

