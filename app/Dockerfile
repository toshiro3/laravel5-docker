FROM php:latest
MAINTAINER toshiro3<t.ooka.102@gmail.com>

RUN apt-get -yq update \
  && apt-get -yq install zlib1g-dev

RUN curl -sS https://getcomposer.org/installer | php \
  && mv composer.phar /usr/local/bin/composer \
  && docker-php-ext-install zip \
  && composer global require "laravel/installer"

RUN mkdir /var/www

WORKDIR /var/www/app
EXPOSE 9000
CMD ["php", "artisan", "serve", "--host", "0.0.0.0", "--port", "9000"]
