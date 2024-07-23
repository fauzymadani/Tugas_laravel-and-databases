
# Tugas instalasi laravel dan pembuatan database

- composer : v2.7.7 
- php : v8.2
- git : v2.39.2
## requirements

 - [composer](https://getcomposer.org/)
 - [php](https://www.php.net/)
 - [Git](https://git-scm.com/)


## Laravel Installation

```bash
composer create-project laravel/laravel:^10.0  mylaravelProject
```

if you want to download laravel 11, run this:

```bash
composer create-project laravel/laravel mylaravelProject
```

then :
```bash
  cd myLaravelProject
```
```bash
php artisan serve
```

copy this link and open in tour browser
`http://localhost:8000/`
and voilah, you're ready for laravel development.

![assets3](https://github.com/user-attachments/assets/153e704d-2f5c-47e6-8843-a89ae3cc9a21)





## Creating Database and Table with MariaDB.

mariadb version: `mariadb  Ver 15.1 Distrib 10.11.6-MariaDB, for debian-linux-gnu (x86_64) using  EditLine wrapper`

login as root in your terminal
```bash
mariadb -u root -p
```
to show databases, run the following command:
```bash
SHOW DATABASES;
```

# creating databases
to create Database
```bash
CREATE DATABASE yourDbname;
```
// navigate to the databases
```bash
use yourDbName;
```
create a table inside the databases
```bash
MariaDB [jurusan]> CREATE TABLE pplsatu ( 
   -> id int primary key auto_increment, 
   -> namasiswa varchar(30) not null unique);

Query OK, 0 rows affected (0.034 sec)
MariaDB [jurusan]> show tables;
-+
| Tables_in_jurusan |
| pplsatu
1 row in set (0.001 sec)
```

![db4](https://github.com/user-attachments/assets/285df4ab-1e53-43ac-be53-8d69e3fc7823)

### to see the detail of your table
```bash
DESC yourTable;
```

![db5](https://github.com/user-attachments/assets/a3968559-26f0-4c26-8dbe-f8506c82af65)




