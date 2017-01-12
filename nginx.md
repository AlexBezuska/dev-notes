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

#### Example configuration for node app (or any app that runs on a port)
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

#### Example configuration for a statically-served site
```

server {
        listen 80;
        listen [::]:80;

        root /var/www/yourdomain.com/;
        index index.html index.htm index.nginx-debian.html;

        server_name yourdomain.com www.yourdomain.com;

        location / {
                try_files $uri $uri/ =404;
        }
}
```
Notice the `server_name yourdomain.com www.yourdomain.com;` You can add multiple urls to a single configuration if you seperate them with spaces, in this example `yourdomain.com` and `www.yourdomain.com` are two urls.
This is very useful for adding your url with and without 'www'
**For this to work you must uncomment the line in `/etc/nginx/nginx.conf`:**
```
server_names_hash_bucket_size 64;
```

Check all configurations for errors.
This is really helpful and even returns info on where the error is and in which file.
```
nginx -t -c /etc/nginx/nginx.conf
```