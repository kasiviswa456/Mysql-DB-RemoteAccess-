# Mysql
1. Create the Normal user.
> mysql> CREATE USER 'viswa' IDENTIFIED BY `'Reddy@123'`;
2. Create the one database in mysql.
> mysql> CREATE DATABASE kasi;
3. Give the privileges on DB and User at the same time you have to mention the your local machine ip .
> mysql> GRANT ALL ON kasi.* TO viswa@'172.31.9.55' IDENTIFIED BY 'Reddy@123';
4. Once you have finalized the permissions that you want to set up for your newusers, always be sure to reload all the privileges.
mysql> FLUSH PRIVILEGES;
5. Login the anthore machine with your remote machine ip.
> mysql -u viswa -p -h 172.31.9.55
Enter password:
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 17
Server version: 5.0.45 Source distribution

Type `'help;'` or `'\h'` for help. Type `'\c'` to clear the buffer.

mysql> _

you will login the successfully with anthore machine.
