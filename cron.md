
###Cron @reboot
See your current crontab options:
`crontab -u root -l`  

Edit crontab:
`crontab -u root -e` - 

@reboot - runs at reboot


Crontab line for re-running a forever node app that starts via an npm script:

`@reboot cd /path/to/node/project/ && forever start -c "npm run start" ./`
