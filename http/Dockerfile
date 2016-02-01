FROM debian:jessie

RUN export DEBIAN_FRONTEND=noninteractive && \
    apt-get update && apt-get -qy upgrade && \
    apt-get -qy install nginx-extras

COPY conf/default /etc/nginx/sites-available/default
COPY web /var/www/html
CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
