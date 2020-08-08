# APACHE

## 404 apache2
> the requested url was not found
1. *** masuk apache conf
   - $ sudoedit /etc/apache2/apache2.conf
2. *** Setelah itu akan muncul isi file konfigurasi apache2.conf pada terminal. Lalu carilah tulisan seperti dibawah ini : (rubah AllowOverride dari None ke All)
   - $ <Directory /var/www/>
   - Options Indexes FollowSymLinks
   - AllowOverride *none* All
   - Require all granted
   - </Directory>
3. *** Restart dulu apache nya
   - $ sudo service apache2 restart
4. *** aktifkan modul rewrite
   - $ sudo a2enmod rewrite
5. *** restart apache kembali

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
