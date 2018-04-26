FROM nginx:1.13
MAINTAINER jose.romero@core-developers.com

RUN mkdir 644 -p /bazel/cache
RUN chown -R nginx:nginx /bazel

COPY conf/nginx.conf /etc/nginx/nginx.conf