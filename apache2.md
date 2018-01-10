# Apache 2


restart `sudo /etc/init.d/apache2 restart`

each site has a file in
`/etc/apache2/sites-available/`

after the file has been created
`sudo a2ensite website-name.conf`

`service apache2 reload`
