# alx-backend-storage
this repo is a ALX project repo for alx-backend-storage

# 0x00. MySQL advanced

## Resources
Read or watch:
- [MySQL cheatsheet](https://devhints.io/mysql)
- [MySQL Performance: How To Leverage MySQL Database Indexing](https://www.percona.com/blog/2018/04/13/visual-explanation-of-sql-joins/)
- [Stored Procedure](https://dev.mysql.com/doc/refman/5.7/en/stored-procedures.html)
- [Triggers](https://dev.mysql.com/doc/refman/5.7/en/triggers.html)
- [Views](https://dev.mysql.com/doc/refman/5.7/en/create-view.html)
- [Functions and Operators](https://dev.mysql.com/doc/refman/5.7/en/functions.html)
- [Trigger Syntax and Examples](https://dev.mysql.com/doc/refman/5.7/en/trigger-syntax.html)
- [CREATE TABLE Statement](https://dev.mysql.com/doc/refman/5.7/en/create-table.html)
- [CREATE PROCEDURE and CREATE FUNCTION Statements](https://dev.mysql.com/doc/refman/5.7/en/create-procedure.html)
- [CREATE INDEX Statement](https://dev.mysql.com/doc/refman/5.7/en/create-index.html)
- [CREATE VIEW Statement](https://dev.mysql.com/doc/refman/5.7/en/create-view.html)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

### General
- How to create tables with constraints
- How to optimize queries by adding indexes
- What is and how to implement stored procedures and functions in MySQL
- What is and how to implement views in MySQL
- What is and how to implement triggers in MySQL

## Requirements

### General
- All your files will be executed on Ubuntu 18.04 LTS using MySQL 5.7 (version 5.7.30)
- All your files should end with a new line
- All your SQL queries should have a comment just before (i.e. syntax above)
- All your files should start by a comment describing the task
- All SQL keywords should be in uppercase (`SELECT`, `WHERE`…)
- A `README.md` file, at the root of the folder of the project, is mandatory
- The length of your files will be tested using `wc`

## More Info

### Comments for your SQL file:
```sql
$ cat my_script.sql
-- 3 first students in the Batch ID=3
-- because Batch 3 is the best!
SELECT id, name FROM students WHERE batch_id = 3 ORDER BY created_at DESC LIMIT 3;
$
```
## Use “container-on-demand” to run MySQL
- Ask for container Ubuntu 18.04 - Python 3.7
- Connect via SSH
- Or via the WebTerminal
- In the container, you should start MySQL before playing with it:
```sql
$ service mysql start
 * MySQL Community Server 5.7.30 is started
$
$ cat 0-list_databases.sql | mysql -uroot -p my_database
Enter password: 
Database
information_schema
mysql
performance_schema
sys
$
```
## How to import a SQL dump
```sql
$ echo "CREATE DATABASE hbtn_0d_tvshows;" | mysql -uroot -p
Enter password: 
$ curl "https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/274/hbtn_0d_tvshows.sql" -s | mysql -uroot -p hbtn_0d_tvshows
Enter password: 
$ echo "SELECT * FROM tv_genres" | mysql -uroot -p hbtn_0d_tvshows
Enter password: 
id  name
1   Drama
2   Mystery
3   Adventure
4   Fantasy
5   Comedy
6   Crime
7   Suspense
8   Thriller
$
```

## Repository
- GitHub repository: [alx-backend-storage](https://github.com/Emakiflom/alx-storage-.git)
- Directory: `0x00-MySQL_Advanced`

## Author
- **Aman Hablu**
