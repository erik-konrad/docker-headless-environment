FROM php:7.4-apache

RUN a2enmod rewrite

RUN apt update && apt install unzip -y && \
 apt install git -y && apt install zlib1g -y && \
apt install libpng-dev -y && apt install libzip-dev -y && \
apt install libsodium-dev -y && apt install libcurl4-openssl-dev -y &&  \
apt install libxml2-dev -y && apt install libonig-dev -y

RUN docker-php-ext-install gd pdo pdo_mysql mysqli zip sodium curl soap json mbstring

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer