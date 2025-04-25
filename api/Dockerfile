FROM php:8.2-fpm

# Instalar dependências do sistema necessárias para rodar o Symfony
RUN apt-get update && apt-get install -y \
    zip \
    unzip \
    git \
    curl \
    libicu-dev \
    libonig-dev \
    libxml2-dev \
    libzip-dev \
    && docker-php-ext-install pdo pdo_mysql intl opcache zip

# Instalar o Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# Definir o diretório de trabalho
WORKDIR /var/www/html

# Copiar os arquivos do projeto Symfony
COPY . .

# Instalar as dependências do Composer, mas sem as dependências de desenvolvimento
RUN composer install --no-dev --optimize-autoloader --no-scripts

# Configurações do PHP para produção
COPY ./php.ini /usr/local/etc/php/conf.d/

# Permitir que o Nginx gerencie as requisições PHP
RUN mkdir -p /var/www/html/var && chown -R www-data:www-data /var/www/html/var

# Expor a porta 9000 (aqui é onde o PHP-FPM vai escutar)
EXPOSE 9000

# Usar o PHP-FPM para rodar o Symfony
CMD ["php-fpm"]