# ubuntu-command


phpmyadmin-on-ubuntu-22-04
---
https://tecadmin.net/how-to-install-phpmyadmin-on-ubuntu-22-04/
https://computingforgeeks.com/install-and-use-firewalld-on-ubuntu/


Mysql
---
- sudo chown mysql:mysql /etc/mysql/my.cnf
- sudo chmod 600 /etc/mysql/my.cnf
- sudo chmod -Rf 0777 /var/lib/mysql
- cd /var/lib/mysql
- service mysql restart
- mysql -u root -p ecd < /home/dev/Downloads/DB/ecd_2306.sql

Services
---
- sudo service apache2 restart
- sudo systemctl restart apache2
- sudo systemctl reload apache2
- sudo systemctl status apache2

Virtual host
---
- sudo cp /etc/apache2/sites-available/test.local.conf /etc/apache2/sites-available/test.local.conf
- sudo a2ensite test.com.conf

PHP
---
sudo apt show php -a
php8.1 -m

- sudo apt update && sudo apt upgrade 
- sudo apt install software-properties-common ca-certificates lsb-release apt-transport-https 
- LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php 
- sudo apt update 
- sudo apt install php8.1 
- sudo apt install php7.4 
- sudo apt install php7.2 
- sudo apt install php5.6 
- sudo apt install php7.4-[extension]
- sudo apt install php7.4-mysql php7.4-mbstring php7.4-xml php7.4-curl php7.4-gd php7.4-intl php7.4-xsl php-zip php7.4-zip php-dom
- php -v

- sudo update-alternatives --set php /usr/bin/php7.4
- sudo update-alternatives --config php

- sudo a2dismod php8.1
- sudo a2enmod php8.1

Remove PHP
---
- sudo apt remove php5.6 
- sudo apt remove php5.6-* 


Workbench Ubuntu
---
- https://linuxhint.com/installing_mysql_workbench_ubuntu/

- sudo apt-get autoremove 
- sudo apt-get autoclean

Laravel setup
---
- sudo chmod -Rf 0777 storage bootstrap/cache
