# GPG

Генерация

  gpg --full-generate-key

Список ключей

  gpg --list-secret-keys --keyid-format LONG

Посмотреть публичный ключ

  gpg --armor --export 545166771694DE62

Расшифровать файл

  gpg --output ~/xxx/xxx.txt --decrypt ~/xxx/xxx.gpg
