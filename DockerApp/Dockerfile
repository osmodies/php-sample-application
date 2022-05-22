FROM php:7.4-apache
COPY 000-default.conf /etc/apache2/sites-available/000-default.conf
COPY . /var/www/html
WORKDIR /var/www/html
RUN chmod 777 /var/www/html/logs/
RUN chmod 777 /var/www/html/
RUN a2enmod rewrite && service apache2 restart



#WORKDIR /usr/src/myapp
#CMD [ "php", "./your-script.php" ]

#docker build -t php-odiaz -f .\DockerApp\Dockerfile .