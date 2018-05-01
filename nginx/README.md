### Build
download files in the directory and execute this command:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker build -t nginx:1.14.0 ./`

the size of container is 18MB.

### Simply run
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sudo docker run --name nginx -p 80:80 -v /path/nginx/www:/var/www  -d nginx:1.14.0`
