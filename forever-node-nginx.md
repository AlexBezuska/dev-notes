
###forever
Installation
```
npm install forever -g
```
Run a node app forever (restarts on crashes, not reboots)
```
forever start /path/to/node/project/app.js
```

Run a node app (started via npm script) forever (restarts on crashes, not reboots)
from inside `/path/to/node/project/`
```
forever start -c "npm run start" ./
```

###Cron @reboot
See your current crontab options:
`crontab -u root -l`  

Edit crontab:
`crontab -u root -e` - 

@reboot - runs at reboot


Crontab line for re-running a forever node app that starts via an npm script:

`@reboot cd /path/to/node/project/ && forever start -c "npm run start" ./`

See if process is currently running based on its name (ex node):
`ps -e|grep node`

###Nginx

Installation (ubuntu):
`sudo apt-get install nginx`

Start nginx:
`sudo service nginx start`

Stop nginx:
`sudo service nginx stop`

Restart nginx:
`sudo service nginx restart`

 
Add new nginx configuration:
configurations live in: `vim /etc/nginx/conf.d/`
example: `vim /etc/nginx/conf.d/yourdomain.com.conf`

#### Example configuration for node app
```
server {
    listen 80;

    server_name yourdomain.com www.yourdomain.com;

    location / {
        proxy_pass http://localhost:3000;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }
}
```
Notice the `server_name yourdomain.com www.yourdomain.com;` You can add multiple urls to a singl configuration if you seperate them with spaces, in this example `yourdomain.com` and `www.yourdomain.com` are two urls. 
This is very useful for adding your url with and without 'www'
**For this to work you must uncomment the line in `/etc/nginx/nginx.conf`:**
```
server_names_hash_bucket_size 64;
```
