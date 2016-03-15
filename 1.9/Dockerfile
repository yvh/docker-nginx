FROM nginx:1.9
MAINTAINER Yannick Vanhaeren

RUN sed -i -e "s|keepalive_timeout\s*65|keepalive_timeout 2|" /etc/nginx/nginx.conf \
    && sed -i -e "s|#gzip\s*on;|gzip on;\n\tgzip_disable \"msie6\";|" /etc/nginx/nginx.conf
