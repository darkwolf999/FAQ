<H2> MySQL Shell </H2>

**����������� � ��������� ��**  

1. $ **\sql**  
2. $ **\connect root@51.15.118.65**  

**������ ������ ������� ��**  

1. $ **CREATE USER 'non-root'@'localhost' IDENTIFIED BY '123';**  
2. $ **GRANT ALL PRIVILEGES ON * . * TO 'non-root'@'ip';**   <span style="color:green">		//������ ip ����� �������� ��� ip, % - ��������� � ������ ip, ���� localhost</span>
3. $ **FLUSH PRIVILEGES;**  

$ **mysql -u root -p**  
$ **mysql> SET PASSWORD FOR root@localhost=PASSWORD('new_password');**  