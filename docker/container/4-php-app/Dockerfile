FROM php:7-apache
COPY . /var/www/html/index.php
# use server port 80
EXPOSE 80  
# in apache server the following command line is used to serve a php app
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"];