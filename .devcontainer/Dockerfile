FROM mcr.microsoft.com/devcontainers/php:3-8.4-bookworm

USER root

RUN apt-get update \
    && apt-get install -y \
        mariadb-client \
        git \
        unzip \
        curl \
    && docker-php-ext-install mysqli pdo pdo_mysql \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*