# docker
This repository uses to storage some files for docker containers.

## run DNMP(docker nginx mariadb php)
/path/nginx/www is the path in host to storage web files
/path/mariadb/data is the path in host to storage database

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name mariadb -p 3306:3306 -v /path/mariadb/data:/var/lib/mysql -d liumiaocn/maria`(note: build by mariadb-second)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name php-fpm -v /path/nginx/www:/var/www --link mariadb:mariadb -d php-fpm:7.2`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name nginx -p 80:80 -v /path/nginx/www:/var/www --link php-fpm:php-fpm -d nginx:1.14.0`
