FROM nginx:latest

RUN apt-get update && \
    apt-get -y install git vim libicu-dev libonig-dev libzip-dev locales && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

COPY ./conf.d/default.conf /etc/nginx/conf.d/default.conf
