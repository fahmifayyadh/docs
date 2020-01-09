# APACHE

### setting FTP
https://www.cloudjojo.com/how-to-connect-ec2-machine-with-ftp/<br>
<p>->allow port ufw firewall ubuntu <br>
- $ sudo ufw allow *port* <br>
Port : 20, 21, 80, 443, and open 1200-12100 <br></p>
- $ sudo ufw allow 1200:12100/tcp <br>
- ->last, open your VM port <br>

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
