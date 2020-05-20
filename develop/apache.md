# Apache

## Установка

    sudo apt-get install apache2

## Запуск

    sudo systemctl start apache2

## Включение htaccess

    sudo a2enmod rewrite

открыть файл:
/etc/apache2/apache2.conf

Добавить код:

    <Directory /var/www>
        Options Indexes FollowSymLinks MultiViews
        AllowOverride All
        Order allow,deny
        allow from all
    </Directory>

## Автозагрузка

    sudo systemctl enable apache2

## Проверка статуса сервиса

    sudo systemctl status apache2

## Включение SSL

    sudo a2enmod ssl
