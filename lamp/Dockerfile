FROM php:7.4-apache 
RUN docker-php-ext-install mysqli pdo_mysql
RUN apt-get update \
    && apt-get install -y libzip-dev \
    && apt-get install -y zlib1g-dev \
    && apt-get install -y libxml2-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install zip \
    && docker-php-ext-install soap 
