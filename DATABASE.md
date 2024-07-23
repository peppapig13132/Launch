# DATABASE

## MySQL

🧩**Connect MySQL:**
```
mysql -u root -p
```

🧩**Create a database:**
```
SHOW DATABASES;
CREATE DATABASE <dbname>;
```

🧩**Crease a user for your database:**
```
SELECT user, host FROM mysql.user;
CREATE USER '<username>@<hostname>' IDENTIFIED BY '<password>';
```
For example, `CREATE USER 'peppapig13132'@'localhost' IDENTIFIED BY 's6lqyzDKfNwpCadgDoBE';`

🧩**Grant privileges:**
```
GRANT ALL PRIVILEGES ON <dbname>.* TO '<username>'@'<hostname>';
FLUSH PRIVILEGES;
```

🧩**Drop a user:**
```
DROP USER '<username>'@'%';
```
