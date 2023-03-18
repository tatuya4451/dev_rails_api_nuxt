FROM ruby:3.2.1

ENV APP_ROOT=/var/www/dev_rails_api_nuxt/api

ENV LANG=C.UTF-8 \
    TZ=Asia/Tokyo

RUN apt-get update && \
    apt-get install -y \
    build-essential \
    default-mysql-client

RUN gem install bundler

WORKDIR $APP_ROOT
