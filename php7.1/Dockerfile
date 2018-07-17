FROM debian:unstable
ENV DEBIAN_FRONTEND="noninteractive"
RUN apt-get update -yqq && apt-get -yqq install findutils make git php7.1-cli composer php7.1-mbstring php7.1-dom php7.1-curl php7.1-xml php7.1-mysql php-pear librdkafka-dev php7.1-dev
RUN pecl install rdkafka
RUN apt-get install -yqq unzip
