FROM bboehmke/php:5-fpm

# install doxygen
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get -y doxygen graphviz && \
    rm -rf /var/lib/apt/lists/*

# install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
