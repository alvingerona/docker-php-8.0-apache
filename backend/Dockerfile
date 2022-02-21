FROM oberd/php-8.0-apache

ENV APACHE_RUN_DIR /var/run/apache2
ENV APACHE_PID_FILE /var/run/apache2/apache2.pid
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2

WORKDIR /var/www

CMD bash -c "composer install &&

#USER www-data

COPY . /var/www


EXPOSE 80

CMD ["/usr/sbin/apache2", "-DFOREGROUND"]