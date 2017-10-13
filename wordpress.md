

## Permissions

https://www.smashingmagazine.com/2014/05/proper-wordpress-filesystem-permissions-ownerships/

Run the following commands from inside the root of the Wordpress installation in no particular order:

```
sudo chown -R www-data:www-data * 
```
```
sudo find . -type f -exec chmod 644 {} \;
```
```
sudo find . -type d -exec chmod 775 {} \;
```
```
sudo chmod 660 wp-config.php
```

https://www.digitalocean.com/community/questions/can-t-install-or-update-wordpress-plugins

add this line to wp-config.php
```
define('FS_METHOD', 'direct');
```
