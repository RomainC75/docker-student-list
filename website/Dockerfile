FROM php:apache
LABEL Romain Chenard <rom.chenard@gmail.com>

RUN apt-get update -y \
    && 

COPY ./index.php /usr/src/myapp/
WORKDIR /usr/src/myapp

CMD [ "php", "./your-script.php" ]