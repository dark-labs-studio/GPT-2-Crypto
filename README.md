## Setup
1. Clone or Download GPT-2-Crypto

2. Clone or Download GPT-2-Crypto-Checkpoint
+ Move /GPT-2-Crypto-Checkpoint/Checkpoint -> /GPT-2-Crypto 

3. Clone or Download GPT-2-Crypto-Model
+ Move /GPT-2-Crypto-Model/Model -> /GPT-2-Crypto 


## Running GPT-2-Crypto
GPT-2 Runs on an hourly Cron Schedule but needs to be kept running using one of the following methods:

### FOREVER

Show current jobs running on forever

```$ forever list```


add  

```$ forever index.js```


show data

```$ /home/future/.forever/[foreverOutput].log```


restart bot

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
