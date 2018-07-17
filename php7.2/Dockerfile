FROM debian:unstable
ENV DEBIAN_FRONTEND="noninteractive"
RUN apt-get update -yqq && apt-get install findutils make git php7.2-cli composer php7.2-mbstring php7.2-dom php7.2-curl php7.2-xml php7.2-mysql php-pear librdkafka-dev php7.2-dev
RUN pecl install rdkafka
