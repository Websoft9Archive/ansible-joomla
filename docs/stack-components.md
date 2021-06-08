# Parameters

The Joomla deployment package contains a sequence software (referred to as "components") required for Joomla to run. The important information such as the component name, installation directory path, configuration file path, port, version, etc. are listed below.

## Path

### Joomla

Joomla installation directory: */data/wwwroot/joomla*  
Joomla configuration file: */data/wwwroot/joomla/configuration.php*   

### PHP

PHP configuration file: */etc/php.ini*  
PHP Modules configurations directory: */etc/php.d*

### Apache

Joomla on LAMP, the Web Server is Apache  

Apache vhost configuration file: */etc/httpd/conf.d/vhost.conf*    
Apache main configuration file: */etc/httpd/conf/httpd.conf*   
Apache logs file: */var/log/httpd*  
Apache module configuration file: */etc/httpd/conf.modules.d/00-base.conf*    

### Nginx

Joomla on LEMP, the Web Server is Nginx    

Nginx vhost configuration file: */etc/nginx/sites-available/default.conf*  
Nginx main configuration file: */etc/nginx/nginx.conf*  
Nginx logs file: */var/log/nginx/*

### MYSQL

MySQL installation directory: */usr/local/mysql*  
MySQL data directory: */data/mysql*  
MySQL configuration file: */etc/my.cnf*    
MySQL Web Management URL: *http://Internet IP/phpmyadmin*, [get credential](/stack-accounts.md)

### phpMyAdmin

phpMyAdmin installation directory: */data/apps/phpmyadmin*  
phpMyAdmin configuration file: */data/apps/phpmyadmin/config.inc.php*   
phpMyAdmin vhost configuration file: */etc/httpd/conf.d/phpMyAdmin.conf* or */etc/nginx/php.conf*  

### Redis

Redis configuration file: */etc/redis.conf*  
Redis data directory: */var/lib/redis*  
Redis logs file: */var/log/redis/redis.log*

### Docker

OnlyOffice Document Server on Docker included in this stack

## Ports

You can control(open or shut down) ports by **[Security Group Setting](https://support.websoft9.com/docs/faq/zh/tech-instance.html)** of your Cloud Server whether the port can be accessed from Internet.

These ports should be opened for this application:

| Name | Number | Use |  Necessity |
| --- | --- | --- | --- |
| HTTP | 80 | HTTP requests for Joomla | Required |
| HTTPS | 443 | HTTPS requests Joomla | Optional |
| MySQL | 3306 | Remote connect MySQL | Optional |

## Version

You can see the version from product page of Marketplace. However, after being deployed to your server, the components will be automatically updated, resulting in a certain change in the version number. Therefore, the exact version number should be viewed by running the command on the server:

```shell
# Linux Version
lsb_release -a

# PHP Version
php -v

# List Installed PHP Modules
php -m

# Apache version on Centos
httpd -v

# Apache version on Ubuntu
apache2 -v

# List Installed Apache Modules
apachectl -M

# Nginx version
nginx -v

# List Installed Nginx Modules
nginx -V

# MySQL version:
mysql -V

# Redis version
redis-server -v

# Dokcer:
docker --version
```
