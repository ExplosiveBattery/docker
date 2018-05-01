## Build
download files in the directory and execute this command:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker build -t php-fpm:7.2 ./`

the size of container is 80.5MB.

## Run
### Simply run
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name php-fpm -p 9000:9000 -d php-fpm:7.2`

### Run with nginx container
/path/nginx/www is the path in host to storage web files

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name php-fpm -d php-fpm:7.2`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name nginx -p 80:80 -v /path/nginx/www:/var/www  -d --link php-fpm:php-fpm nginx:1.14.0`
