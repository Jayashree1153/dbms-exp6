# dbms-exp6
Enter password: *********
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 22
Server version: 8.0.30 MySQL Community Server - GPL

Copyright (c) 2000, 2022, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> Enter password: *********
    -> Welcome to the MySQL monitor.  Commands end with ; or \g.
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Enter password: *********
Welcome to the MySQL monitor.  Commands end with' at line 1
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'or' at line 1
    -> Your MySQL connection id is 21
    -> Server version: 8.0.30 MySQL Community Server - GPL
    ->
    -> Copyright (c) 2000, 2022, Oracle and/or its affiliates.
    ->
    -> Oracle is a registered trademark of Oracle Corporation and/or its
    -> affiliates. Other names may be trademarks of their respective
    -> owners.
    ->
    -> Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.
    ->
    -> mysql> create database flipkart;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '.
Your MySQL connection id is 21
Server version: 8.0.30 MySQL Community Server -' at line 1
mysql> Query OK, 1 row affected (0.01 sec)
    ->
    -> mysql> use flipkart;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Query OK, 1 row affected (0.01 sec)

mysql> use flipkart' at line 1
mysql> Database changed
    -> mysql> create table emp(emp_no int(3), ename varchar(20), sal int);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Database changed
mysql> create table emp(emp_no int(3), ename varchar(20), sal i' at line 1
mysql> Query OK, 0 rows affected, 1 warning (0.03 sec)
    ->
    -> mysql> insert into emp(1,"dora",20000),(2,"light",30000),(3,"heidi",50000),(4,"julie",25000),(5,"jak",80000);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Query OK, 0 rows affected, 1 warning (0.03 sec)

mysql> insert into emp(1,"dora"' at line 1
mysql> ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '1,"dora",20000),(2,"light",30000),(3,"heidi",50000),(4,"julie",25000),(5,"jak",8' at line 1
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ERROR 1064 (42000): You have an error in your SQL syntax' at line 1
    -> mysql> insert into emp values(1,"dora",20000),(2,"light",30000),(3,"heidi",50000),(4,"julie",25000),(5,"jak",80000);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'the manual that corresponds to your MySQL server version for the right syntax to' at line 1
mysql> Query OK, 5 rows affected (0.01 sec)
    -> Records: 5  Duplicates: 0  Warnings: 0
    ->
    -> mysql> select * from emp;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Query OK, 5 rows affected (0.01 sec)
Records: 5  Duplicates: 0  Warnings: 0

mys' at line 1
mysql> +--------+-------+-------+
    -> | emp_no | ename | sal   |
    -> +--------+-------+-------+
    -> |      1 | dora  | 20000 |
    -> |      2 | light | 30000 |
    -> |      3 | heidi | 50000 |
    -> |      4 | julie | 25000 |
    -> |      5 | jak   | 80000 |
    -> +--------+-------+-------+
    -> 5 rows in set (0.00 sec)
    ->
    -> mysql> select * from emp order by emp.sal desc;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '+--------+-------+-------+
| emp_no | ename | sal   |
+--------+-------+-------+' at line 1
mysql> +--------+-------+-------+
    -> | emp_no | ename | sal   |
    -> +--------+-------+-------+
    -> |      5 | jak   | 80000 |
    -> |      3 | heidi | 50000 |
    -> |      2 | light | 30000 |
    -> |      4 | julie | 25000 |
    -> |      1 | dora  | 20000 |
    -> +--------+-------+-------+
    -> 5 rows in set (0.00 sec)
    ->
    -> mysql> create table customer(customer_id int(5),customer_name varchar(20), contact_no int(10),address varchar(50),city varchar(50),postel_code varchar(5),country char(20);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '+--------+-------+-------+
| emp_no | ename | sal   |
+--------+-------+-------+' at line 1
mysql> ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '' at line 1
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ERROR 1064 (42000): You have an error in your SQL syntax' at line 1
    -> mysql> create table customer(customer_id int(5),customer_name varchar(20), contact_no int(10),address varchar(50),city varchar(50),postel_code varchar(5),country char(20));
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'the manual that corresponds to your MySQL server version for the right syntax to' at line 1
mysql> Query OK, 0 rows affected, 2 warnings (0.02 sec)
    ->
    -> mysql> desc customer;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Query OK, 0 rows affected, 2 warnings (0.02 sec)

mysql> desc customer' at line 1
mysql> +---------------+-------------+------+-----+---------+-------+
    -> | Field         | Type        | Null | Key | Default | Extra |
    -> +---------------+-------------+------+-----+---------+-------+
    -> | customer_id   | int         | YES  |     | NULL    |       |
    -> | customer_name | varchar(20) | YES  |     | NULL    |       |
    -> | contact_no    | int         | YES  |     | NULL    |       |
    -> | address       | varchar(50) | YES  |     | NULL    |       |
    -> | city          | varchar(50) | YES  |     | NULL    |       |
    -> | postel_code   | varchar(5)  | YES  |     | NULL    |       |
    -> | country       | char(20)    | YES  |     | NULL    |       |
    -> +---------------+-------------+------+-----+---------+-------+
    -> 7 rows in set (0.00 sec)
    ->
    -> mysql> select
    ->     -> s;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '+---------------+-------------+------+-----+---------+-------+
| Field         |' at line 1
mysql> ERROR 1054 (42S22): Unknown column 's' in 'field list'
    -> mysql> insert into customer values(1,"nayan",9887654386,
    ->     ->
    ->     -> :
    ->     -> ;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ERROR 1054 (42S22): Unknown column 's' in 'field list'
mysql> insert into custom' at line 1
mysql> ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near ':' at line 3
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ERROR 1064 (42000): You have an error in your SQL syntax' at line 1
    -> mysql> insert into customer values(1,"nayan",9887654386,"aadhinagar","chennai",60067,"India"),(2,"sri",987656765,"idlinagar","trichy",89068,"india"),(3,"kayal",8976898765,"ammanagar","madurai",60056,"India");
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'the manual that corresponds to your MySQL server version for the right syntax to' at line 1
mysql> ERROR 1264 (22003): Out of range value for column 'contact_no' at row 1
    -> mysql> insert into customer values(1,"nayan",9887646,"aadhinagar","chennai",60067,"India"),(2,"sri",97656765,"idlinagar","trichy",89068,"india"),(3,"kayal",897689765,"ammanagar","madurai",60056,"India");
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ERROR 1264 (22003): Out of range value for column 'contact_no' at row 1
mysql> i' at line 1
mysql> Query OK, 3 rows affected (0.01 sec)
    -> Records: 3  Duplicates: 0  Warnings: 0
    ->
    -> mysql> select * from customer;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Query OK, 3 rows affected (0.01 sec)
Records: 3  Duplicates: 0  Warnings: 0

mys' at line 1
mysql> +-------------+---------------+------------+------------+---------+-------------+---------+
    -> | customer_id | customer_name | contact_no | address    | city    | postel_code | country |
    -> +-------------+---------------+------------+------------+---------+-------------+---------+
    -> |           1 | nayan         |    9887646 | aadhinagar | chennai | 60067       | India   |
    -> |           2 | sri           |   97656765 | idlinagar  | trichy  | 89068       | india   |
    -> |           3 | kayal         |  897689765 | ammanagar  | madurai | 60056       | India   |
    -> +-------------+---------------+------------+------------+---------+-------------+---------+
    -> 3 rows in set (0.00 sec)
    ->
    -> mysql> insert into customer values(6,"kitty",9887646,"aadhinagar","chennai",60067,"India"),(5,"kavi",97656765,"idlinagar","trichy",89068,"india"),(4,"abi",897689765,"ammanagar","madurai",60056,"India");
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '+-------------+---------------+------------+------------+---------+-------------' at line 1
mysql> Query OK, 3 rows affected (0.00 sec)
    -> Records: 3  Duplicates: 0  Warnings: 0
    ->
    -> mysql> select * from customer;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'Query OK, 3 rows affected (0.00 sec)
Records: 3  Duplicates: 0  Warnings: 0

mys' at line 1
mysql> +-------------+---------------+------------+------------+---------+-------------+---------+
    -> | customer_id | customer_name | contact_no | address    | city    | postel_code | country |
    -> +-------------+---------------+------------+------------+---------+-------------+---------+
    -> |           1 | nayan         |    9887646 | aadhinagar | chennai | 60067       | India   |
    -> |           2 | sri           |   97656765 | idlinagar  | trichy  | 89068       | india   |
    -> |           3 | kayal         |  897689765 | ammanagar  | madurai | 60056       | India   |
    -> |           6 | kitty         |    9887646 | aadhinagar | chennai | 60067       | India   |
    -> |           5 | kavi          |   97656765 | idlinagar  | trichy  | 89068       | india   |
    -> |           4 | abi           |  897689765 | ammanagar  | madurai | 60056       | India   |
    -> +-------------+---------------+------------+------------+---------+-------------+---------+
    -> 6 rows in set (0.00 sec)
    ->
    -> mysql> select country,count(*)from customer group by country order by country asc;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '+-------------+---------------+------------+------------+---------+-------------' at line 1
mysql> +---------+----------+
    -> | country | count(*) |
    -> +---------+----------+
    -> | India   |        6 |
    -> +---------+----------+
    -> 1 row in set (0.01 sec)
    ->
    -> ;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '+---------+----------+
| country | count(*) |
+---------+----------+
| India   |' at line 1
mysql> select count(city),city from customer group by city having count(city)>1;
ERROR 1046 (3D000): No database selected
mysql> use flipkart;
Database changed
mysql> select count(city),city from customer group by city having count(city)>1;
+-------------+---------+
| count(city) | city    |
+-------------+---------+
|           2 | chennai |
|           2 | trichy  |
|           2 | madurai |
+-------------+---------+
3 rows in set (0.00 sec)
