## Build

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker pull liumiaocn/maria`

## Run

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name mariadb -p 3306:3306 -v /path/mariadb/data:/var/lib/mysql -d liumiaocn/maria`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker exec -it mariadb /bin/sh`
