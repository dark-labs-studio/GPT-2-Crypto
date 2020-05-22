

### Running GPT-2-Crypto
GPT-2 Runs on an hourly Cron Schedule but needs to be kept running using one of the following methods:

1. CRONTAB

Setup crontab to restart program every hour
$ sudo crontab -e

Add to crontab file
$ */36 * * * * restart /home/future/Code/DARK-labs/Projects/c-ai/C-AI_repo/M4pSK/M4pSK/build.sh

Give cronjob access
$ chmod +x /home/future/Code/DARK-labs/Projects/c-ai/C-AI_repo/M4pSK/M4pSK/build.sh

--------------------
2. FOREVER

Show current jobs running on forever
$ forever list

add  
$ forever index.js

show data
$ /home/future/.forever/[foreverOutput].log

restart bot
$ forever restart index.js

-----------------
3. PM2 Methods

start pm2
$ pm2 start index.js

Start pm2 restarting script
$ pm2 start pm2
$ pm2 monit
