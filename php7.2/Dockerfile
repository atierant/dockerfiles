FROM debian:unstable
ENV DEBIAN_FRONTEND="noninteractive"
RUN apt-get update -yqq && apt-get install -yqq unzip findutils make git php7.2-pdo php7.2-cli composer php7.2-mbstring php7.2-dom php7.2-curl php7.2-xml php7.2-mysql php-pear librdkafka-dev php7.2-dev php-xdebug
RUN pecl install rdkafka
# Attention... En PHP 7.2, on enlève le .so et on laisse juste rdkafka
RUN echo 'extension=rdkafka' >> /etc/php/7.2/cli/php.ini
RUN wget -O /usr/local/bin/phpmetrics https://github.com/phpmetrics/PhpMetrics/releases/download/v2.4.1/phpmetrics.phar && chmod +x /usr/local/bin/phpmetrics
RUN wget -O /usr/local/bin/phpunit https://phar.phpunit.de/phpunit-7.phar && chmod +x /usr/local/bin/phpunit
RUN wget -O /usr/local/bin/phpcov https://phar.phpunit.de/phpcov.phar && chmod +x /usr/local/bin/phpcov
