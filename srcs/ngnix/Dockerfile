# Use the official NGINX image as the base
FROM nginx:stable-alpine

# Set the maintainer label
LABEL maintainer="your_email@example.com"

# Create directories for SSL certificates and configuration
RUN mkdir -p /etc/nginx/ssl /etc/nginx/conf.d

# Copy your SSL certificate and key into the container
# Replace 'your_certificate.crt' and 'your_private.key' with your actual filenames
COPY ssl/your_certificate.crt /etc/nginx/ssl/
COPY ssl/your_private.key /etc/nginx/ssl/

# Copy your NGINX configuration file
COPY conf/nginx.conf /etc/nginx/nginx.conf

# Expose port 443 for HTTPS traffic
EXPOSE 443

# Start NGINX
CMD ["nginx", "-g", "daemon off;"]
