# PHP with Apache
FROM php:8.2-apache

# System dependencies + PHP extensions
RUN apt-get update && apt-get install -y \
    git unzip libpq-dev libzip-dev zip \
 && docker-php-ext-install pdo pdo_mysql zip

# Enable Apache mod_rewrite
RUN a2enmod rewrite

# Set working directory
WORKDIR /var/www/html

# Copy application code
COPY . .

# Install Composer
COPY --from=composer:2 /usr/bin/composer /usr/bin/composer
RUN composer install --no-dev --optimize-autoloader

# Copy Apache config (create this file next)
COPY ./docker/apache.conf /etc/apache2/sites-available/000-default.conf

EXPOSE 80
CMD ["apache2-foreground"]
