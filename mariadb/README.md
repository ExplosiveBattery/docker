### Build
download files in the directory and execute this command:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker build -t mariadb ./`

the size of container is 202MB.

### Simply run
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name mariadb -p 3306:3306 -v /path/mariadb/data:/var/lib/mysql  -d mariadb`
