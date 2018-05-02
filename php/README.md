## Build
download files in the directory and execute this command:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker build -t php-fpm:7.2 ./`

the size of container is 80.5MB.

## Run

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name php-fpm -p 9000:9000 -d php-fpm:7.2`

