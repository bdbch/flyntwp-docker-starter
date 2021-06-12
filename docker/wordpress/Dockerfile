FROM wordpress:5.7.2-apache as wordpress

# Install composer
COPY --from=composer /usr/bin/composer /usr/bin/composer

# Install composer packages
COPY wp-content /var/www/html/wp-content
WORKDIR /var/www/html/wp-content/themes/flynt
RUN composer require