FROM php:fpm

RUN docker-php-ext-install pdo pdo_mysql && \
	docker-php-ext-enable pdo pdo_mysql

COPY --from=composer:2 /usr/bin/composer /usr/bin/composer
