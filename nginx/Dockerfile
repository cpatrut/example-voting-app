FROM nginx
MAINTAINER catalin.patrut@systematic.com

RUN rm /etc/nginx/nginx.conf
RUN rm /usr/share/nginx/html/index.html
ADD index.html /usr/share/nginx/html/index.html
ADD nginx.conf /etc/nginx/nginx.conf
