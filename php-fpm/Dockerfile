#Custom php docker file
FROM alpine
LABEL mainteiner="Valerii Melkov <v.melkov@gmail.com>"
RUN apk add --update --no-cache \
  php7 \
  php7-fpm
RUN mkdir -p /var/lib/nginx/html
COPY php-fpm.conf /etc/php7/php-fpm.d/www.conf

EXPOSE 9000

CMD ["php-fpm7","-F"]
