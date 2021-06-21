FROM node:lts-alpine

RUN apk add --no-cache \
    autoconf \
    automake \
    bash \
    gcc \
    g++ \
    libc6-compat \
    libjpeg-turbo-dev \
    libc-dev \
    libpng-dev \
    make \
    nasm \
    git \
    curl \
    openssl \
    openssh

## Install PHP mods for Laravel
#RUN apt-get update && apt-get install -y \
#      libicu-dev \
#      libpq-dev \
#      libmcrypt-dev \
#      zlib1g-dev \
#    && rm -r /var/lib/apt/lists/* \
#    && docker-php-ext-configure pdo_mysql --with-pdo-mysql=mysqlnd \
#    && docker-php-ext-install \
#      intl \
#      mbstring \
#      mcrypt \
#      pcntl \
#      pdo_mysql \
#      pdo_pgsql \
#      pgsql \
#      zip \d
#      opcache
#
## Install composer
#RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer
#
## Configure Apache for Laravel
#COPY laravel.conf /etc/apache2/sites-available/laravel.conf
#RUN a2dissite 000-default.conf && a2ensite laravel.conf && a2enmod rewrite
