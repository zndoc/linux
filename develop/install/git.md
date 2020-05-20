# GIT

## Установка

## Настрока

Генерация ключа

    ssh-keygen -t rsa -b 2048 -C "theyamshikov@yandex.ru"

Вводим путь к ключу:

    /home/vitaliy/.ssh/my-gitlab

Открыть публичный ключ

    nano ~/.ssh/my-gitlab.pub

Добавить назначение ключа хосту.
Открываем файл `/home/vitaliy/.ssh/config` и добавляем код:

    Host github.com
     IdentityFile /home/vitaliy/.ssh/my-github
    Host gitlab.com
     IdentityFile /home/vitaliy/.ssh/my-gitlab

## Разное

Список ключей

    ssh-add -l
