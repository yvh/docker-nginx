FROM nginx:latest
MAINTAINER Yannick Vanhaeren

RUN sed -i -e "s|keepalive_timeout\s*65|keepalive_timeout 2|" /etc/nginx/nginx.conf \
    && sed -i -e "s|#gzip\s*on;|gzip on;\n    gzip_disable \"msie6\";\n    gzip_types text/plain application/xml;|" /etc/nginx/nginx.conf
