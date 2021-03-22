docker run --name sakila-database \
-p 3306:3306 \
-e MYSQL_ROOT_PASSWORD=minha-senha \
-v sakila-database:/var/lib/mysql \
-d mysql:latest

mysql -u root -p
CREATE DATABASE sakila;
SHOW DATABASES;

docker run -e --name sakila-sqlserver 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=yourStrong(!)Password' -p 1433:1433 -d mcr.microsoft.com/mssql/server:2017-latest


docker run --name sakila-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=minha-senha -d mysql:latest
docker run --name sakila-mariadb -p 3307:3307 -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mariadb:latest

## SQL NO JUPTER NOTEBOOK

