## MySQL Shell

### Подключение к удаленной бд

1. $ **\sql**  
2. $ **\connect root@51.15.118.65**  

### Внутри самого сервера бд  

1. $ **CREATE USER 'non-root'@'localhost' IDENTIFIED BY '123';**  
2. $ **GRANT ALL PRIVILEGES ON * . * TO 'non-root'@'ip';**   		<span style="color:green">//вместо ip можно написать сам ip, % - разрешить с любого ip, либо localhost</span>
3. $ **FLUSH PRIVILEGES;**  

$ **mysql -u root -p**  
$ **mysql SET PASSWORD FOR root@localhost=PASSWORD('new_password');**  