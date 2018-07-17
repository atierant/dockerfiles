FROM debian:unstable
ENV DEBIAN_FRONTEND="noninteractive"
RUN apt-get update -yqq && apt-get install -yqq unzip findutils make git php7.2-cli composer php7.2-mbstring php7.2-dom php7.2-curl php7.2-xml php7.2-mysql php-pear librdkafka-dev php7.2-dev
RUN pecl install rdkafka
# Attention... En PHP 7.2, on enlève le .so et on laisse juste rdkafka
RUN echo 'extension=rdkafka' >> /etc/php/7.2/cli/php.ini
