FROM bboehmke/php:7-fpm

# install doxygen
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get -y install doxygen graphviz && \
    rm -rf /var/lib/apt/lists/*

# install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
