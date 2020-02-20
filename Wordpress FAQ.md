## Установка wordpress на свой VPS ubuntu

### Чтобы можно было делать установку плагинов через админку wordpress

1. https://invs.ru/support/chastie-voprosy/kak-ustanovit-wordpress-na-vps-s-ubuntu-16-04-16-10-17-04/
2. http://bologer.ru/oshibka-pri-dobavleniiobnovlenii-plaginov-v-wordpress/

1. Выдаем права папке: chmod -R 777 /var/www/html/flowers.ru/wp-content
2. Добавить в файл wp-config.php строчку define('FS_METHOD', 'direct'); после define('DB_COLLATE', ''); — это позволит устанавливать плагины напрямую с WordPress сайта.
