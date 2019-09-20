## 镜像说明

### Nginx
1. 版本为`1.17`；
2. 修改默认配置文件，将默认项目目录改为`/var/www/html`；
3. 修改`php-fpm`链接，将`127.0.0.1`改为容器名字`php`

### MySQL
1. 版本为`8.0`；
2. 修改默认验证插件为`mysql_native_password`；

### PHP
1. 版本为`7.2`；
2. 添加`redis`、`pdo_mysql`插件；
3. 添加`composer`；