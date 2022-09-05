FROM php:7.1.9-apache

RUN apt update && \
    apt install -y wget git libmcrypt-dev && \
    wget -O /tmp/composer-setup.php https://getcomposer.org/installer && \
    php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer && \
    docker-php-ext-install mcrypt


