## Linux Apache Mysql Php for Laravel © 2021

### Navigate

- Application:
    - [http://localhost](http://localhost)
    - [http://localhost:8101](http://localhost:8101)
    - [http://lamp.lv.localhost:8101](http://lamp.lv.localhost:8101)
    - [http://lamp.lv.localhost:80](http://lamp.lv.localhost:80)
    - [https://lamp.lv.localhost](https://lamp.lv.localhost)
- PhpMyAdmin:
    - [http://localhost:8102](http://localhost:8102)
    - [http://db.lamp.lv.localhost:8102](http://db.lamp.lv.localhost:8102)

### Initialize LV project

```
cd ./lamp-lv
rm -rf ./codebase
composer create-project symfony/website-skeleton codebase
sudo chmod -R og+rw lamp-lv/
sudo chown -R jarek:jarek lamp-lv/
```

### DB connection string

- Run on docker container: ```docker exec -it --user www-data lamp_lv-server bash```
```
echo $DATABASE_URL
```
- Output like
```
mysql://app_user:t3rceS@db_server:3306/lamp_lv?serverVersion=10.5
```

### Credits to

[LAMP Docker setup with PHP 8 and MariaDB for Symfony projects](https://www.bornfight.com/blog/blog-lamp-docker-setup-with-php-8-and-mariadb-for-symfony-projects/)