

## Permissions

https://www.smashingmagazine.com/2014/05/proper-wordpress-filesystem-permissions-ownerships/

```
sudo find . -type f -exec chmod 664 {} \;
sudo find . -type d -exec chmod 775 {} \;
sudo chmod 660 wp-config.php
```

https://www.digitalocean.com/community/questions/can-t-install-or-update-wordpress-plugins

add this line to wp-config.php
```
define('FS_METHOD', 'direct');
```
