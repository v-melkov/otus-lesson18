# Running custom nginx in docker
FROM alpine
LABEL mainteiner="Valerii Melkov <v.melkov@gmail.com>"
RUN apk add --update --no-cache nginx && mkdir -p /run/nginx
#COPY index.html /var/lib/nginx/html/index.html
COPY default.conf /etc/nginx/conf.d/default.conf
EXPOSE 80 443
CMD ["nginx","-g","daemon off;"]
