# Setup
1. Clone or Download GPT-2-Crypto


2. Clone or Download GPT-2-Crypto-Checkpoint
[Gitlab-checkpoint](https://gitlab.com/M4pSK/gpt2-server-incrament-checkpoint)

- Move /GPT-2-Crypto-Checkpoint/Checkpoint -> /GPT-2-Crypto 


3. Clone or Download GPT-2-Crypto-Model
[Gitlab-Gpt-2-Model](https://gitlab.com/M4pSK/gpt2-server-incrament-model)

- Move /GPT-2-Crypto-Model/Model -> /GPT-2-Crypto 


## Install Node Dependencies

```$ npm install```


## Install Python Modules

```$ pip install gpt-2-simple```


# Run GPT-2-Crypto
GPT-2 Runs on an hourly Cron Schedule but needs to be kept running using one of the following methods

### FOREVER

Show current jobs running on forever

```$ forever list```


Add  Task

```$ forever index.js```


Show Data

```$ /home/future/.forever/[foreverOutput].log```


Restart Bot

```$ forever restart index.js```


### CRONTAB

Stup crontab to restart program every hour

```$ sudo crontab -e```


Add to crontab file

```$ */36 * * * * restart /home/future/Code/DARK-labs/Projects/c-ai/C-AI_repo/M4pSK/M4pSK/build.sh```


Give cronjob access

```$ chmod +x /home/future/Code/DARK-labs/Projects/c-ai/C-AI_repo/M4pSK/M4pSK/build.sh```

-----------------
### PM2 Methods

start pm2

```$ pm2 start index.js```


Start pm2 restarting script

```$ pm2 start pm2```

Monitor pm2

```$ pm2 monit```
