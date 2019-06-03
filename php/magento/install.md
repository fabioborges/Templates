# Install

## Resource

- <https://serverguy.com/magento/install-magento-2/>
- <https://devdocs.magento.com/guides/v2.3/install-gde/install/web/install-web-sample-data-composer.html>

## Steps

Create a key pair: <https://marketplace.magento.com/customer/accessKeys/>

Public Key: f8637d2078571bac512a64615d03f638 (username)
Private Key: 5bdac65b6de921e17468dba21ed2dbb9 (password)

Store it in the directory ~/.config/composer/auth.json
/home/fabio/.config/composer/auth.json

Installing all dependencies

```bash

sudo apt install php7.0-cli php7.0-xmlwriter php7.0-mcrypt php7.0-bcmath php7.0-ctype php7.0-curl php7.0-dom php7.0-gd php7.0-iconv php7.0-intl php7.0-mbstring php7.0-simplexml php7.0-soap php7.0-xsl php7.0-zip


sudo apt install php7.0-cli php7.0-xmlwriter php7.0-mcrypt php7.0-bcmath php7.0-ctype php7.0-curl php7.0-dom php7.0-gd php7.0-hash php7.0-iconv php7.0-intl php7.0-mbstring php7.0-openssl php7.0-pdo_mysql php7.0-simplexml php7.0-soap php7.0-spl php7.0-xsl php7.0-zip php7.0-lib-libxml

apache2 apache2-bin apache2-data apache2-utils libapache2-mod-php7.2 libapr1 libaprutil1 libaprutil1-dbd-sqlite3 libaprutil1-ldap libgd3 libwebp6 libzip4 php7.2 php7.2-bcmath php7.2-curl php7.2-gd php7.2-intl php7.2-mbstring php7.2-mysql php7.2-soap php7.2-xml
  php7.2-zip ssl-cert
```

```bash

dependencies
php7.1

  Problem 1
    - Installation request for magento/product-community-edition 2.2.3 -> satisfiable by magento/product-community-edition[2.2.3].
    - magento/product-community-edition 2.2.3 requires php 7.0.2|7.0.4|~7.0.6|~7.1.0 -> your PHP version (7.2.17) does not satisfy that requirement.
  Problem 2
    - Installation request for squizlabs/php_codesniffer 3.2.2 -> satisfiable by squizlabs/php_codesniffer[3.2.2].
    - squizlabs/php_codesniffer 3.2.2 requires ext-xmlwriter * -> the requested PHP extension xmlwriter is missing from your system.
  Problem 3
    - phpunit/phpunit 6.2.4 requires ext-dom * -> the requested PHP extension dom is missing from your system.
    - phpunit/phpunit 6.2.3 requires ext-dom * -> the requested PHP extension dom is missing from your system.
    - phpunit/phpunit 6.2.2 requires ext-dom * -> the requested PHP extension dom is missing from your system.
    - phpunit/phpunit 6.2.1 requires ext-dom * -> the requested PHP extension dom is missing from your system.
    - phpunit/phpunit 6.2.0 requires ext-dom * -> the requested PHP extension dom is missing from your system.
    - Installation request for phpunit/phpunit ~6.2.0 -> satisfiable by phpunit/phpunit[6.2.0, 6.2.1, 6.2.2, 6.2.3, 6.2.4].

  To enable extensions, verify that they are enabled in your .ini files:
    - /etc/php/7.2/cli/php.ini
    - /etc/php/7.2/cli/conf.d/10-opcache.ini
    - /etc/php/7.2/cli/conf.d/10-pdo.ini
    - /etc/php/7.2/cli/conf.d/20-calendar.ini
    - /etc/php/7.2/cli/conf.d/20-ctype.ini
    - /etc/php/7.2/cli/conf.d/20-exif.ini
    - /etc/php/7.2/cli/conf.d/20-fileinfo.ini
    - /etc/php/7.2/cli/conf.d/20-ftp.ini
    - /etc/php/7.2/cli/conf.d/20-gettext.ini
    - /etc/php/7.2/cli/conf.d/20-iconv.ini
    - /etc/php/7.2/cli/conf.d/20-json.ini
    - /etc/php/7.2/cli/conf.d/20-phar.ini
    - /etc/php/7.2/cli/conf.d/20-posix.ini
    - /etc/php/7.2/cli/conf.d/20-readline.ini
    - /etc/php/7.2/cli/conf.d/20-shmop.ini
    - /etc/php/7.2/cli/conf.d/20-sockets.ini
    - /etc/php/7.2/cli/conf.d/20-sysvmsg.ini
    - /etc/php/7.2/cli/conf.d/20-sysvsem.ini
    - /etc/php/7.2/cli/conf.d/20-sysvshm.ini
    - /etc/php/7.2/cli/conf.d/20-tokenizer.ini
  You can also run `php --ini` inside terminal to see which files are used by PHP in CLI mode.
```
