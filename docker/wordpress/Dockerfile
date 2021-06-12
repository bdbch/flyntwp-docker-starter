FROM wordpress:5.7.2-apache as wordpress

# Copy wp content into image
COPY wp-content /var/www/html/wp-content

# Install composer
COPY --from=composer /usr/bin/composer /usr/bin/composer

# Install composer packages
WORKDIR /var/www/html/wp-content/themes/flynt
RUN composer require

WORKDIR /var/www/html