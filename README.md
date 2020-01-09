# APACHE

### setting FTP

> open FTP remote
https://www.cloudjojo.com/how-to-connect-ec2-machine-with-ftp/<br>
1. ***allow port ufw firewall ubuntu***
   - $ sudo ufw allow *port*
     - Port : 20, 21, 80, 443, and open 1200-12100
   - $ sudo ufw allow 1200:12100/tcp
2. ***open your VM port***

# COMPOSER

> permission denied for composer in /usr/local/bin/

'''
cd ~/.cache/composer
chmod 755 composer-temp.phar
sudo mv composer-temp.phar /usr/local/bin/composer
'''

Warning: “continue” targeting switch is equivalent to “break”. Did you mean to use “continue 2”?
composer self-update



LUMEN

chmod -R o+w projectname/storage
