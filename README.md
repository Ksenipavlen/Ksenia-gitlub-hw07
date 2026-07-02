Задание 1
<img width="1280" height="691" alt="IMG_7504" src="https://github.com/user-attachments/assets/81afc7bb-3d37-423a-964e-18203ade972b" />
<img width="1280" height="937" alt="IMG_7505" src="https://github.com/user-attachments/assets/3b36a007-025c-4248-b2e4-64461dcadb58" />
<img width="1280" height="943" alt="IMG_7506" src="https://github.com/user-attachments/assets/5bd90358-455f-4a5b-8638-b6444b586f41" />

CREATE USER 'sys_temp'@'%' IDENTIFIED BY 'password';

SELECT User, Host
FROM mysql.user;

GRANT ALL PRIVILEGES
ON *.*
TO 'sys_temp'@'%'
WITH GRANT OPTION;

FLUSH PRIVILEGES;

SHOW GRANTS FOR 'sys_temp'@'%';

ALTER USER 'sys_temp'@'%'
IDENTIFIED WITH mysql_native_password
BY 'password';

FLUSH PRIVILEGES;

CREATE DATABASE sakila;

USE sakila;

SHOW TABLES;


Задание 2
<img width="971" height="975" alt="IMG_7507" src="https://github.com/user-attachments/assets/b1534b9f-7fc0-49d9-bb76-12ccdd2f8249" />
