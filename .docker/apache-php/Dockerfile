FROM php:7.2.7-apache

RUN apt-get update \
    && apt-get install -y curl libxml2-dev zlib1g-dev libcurl4-openssl-dev \
    && docker-php-ext-install ctype bcmath json mbstring pdo xml tokenizer curl pdo_mysql zip mysqli \
    && apt-get clean \
    && /usr/sbin/a2enmod rewrite
