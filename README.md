# development playground on docker
## containers
### apache - 2.4
Ports *:80 *:443

Add ```127.0.0.1 example.com``` to your host file
#### Enable SSL
Add ```server.key``` and ```server.cert``` under **apache/ssl** and 
then uncomment lines 8 and 9 at apache/Dockerfile
### php-fpm - 7.4 
### mysql - 8.0
Port *:3306
### redis - 6.0
Port *:6379