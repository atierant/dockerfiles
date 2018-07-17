FROM debian:unstable
ENV DEBIAN_FRONTEND="noninteractive"
RUN apt-get update -yqq && apt-get -yqq install unzip findutils make git php7.1-cli composer php7.1-mbstring php7.1-dom php7.1-curl php7.1-xml php7.1-mysql php-pear librdkafka-dev php7.1-dev
RUN pecl install rdkafka
# Attention... En PHP 7.2, on enlève le .so et on laisse juste rdkafka
RUN echo 'extension=rdkafka.so' >> /etc/php/7.1/cli/php.ini
