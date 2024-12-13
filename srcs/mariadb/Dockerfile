# Use the official MariaDB image as the base
FROM mariadb:10.5

# Set the maintainer label
LABEL maintainer="your_email@example.com"

# Set environment variables for MariaDB
ENV MYSQL_ROOT_PASSWORD=your_root_password
ENV MYSQL_DATABASE=your_database
ENV MYSQL_USER=your_user
ENV MYSQL_PASSWORD=your_password

# Expose port 3306 for MySQL
EXPOSE 3306

# Start MariaDB
CMD ["mysqld"]
