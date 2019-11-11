COMPOSER

permission denied for composer in /usr/local/bin/
cd ~/.cache/composer
chmod 755 composer-temp.phar
sudo mv composer-temp.phar /usr/local/bin/composer

Warning: “continue” targeting switch is equivalent to “break”. Did you mean to use “continue 2”?
composer self-update
