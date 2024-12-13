# Use the official WordPress image with PHP-FPM
FROM wordpress:php8.1-fpm-alpine

# Set the maintainer label
LABEL maintainer="your_email@example.com"

# Copy custom WordPress configuration if any
# COPY wp-config.php /var/www/html/

# Ensure the necessary directories have the correct permissions
RUN chown -R www-data:www-data /var/www/html

# Expose port 9000 for PHP-FPM
EXPOSE 9000

# Start PHP-FPM
CMD ["php-fpm"]
