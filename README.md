# development playground on docker
## containers
### apache

---
Apache 2.4 webserver

Ports *:80 *:443

Add ```127.0.0.1 example.com``` to your host file

#### Enable SSL
Add ```server.key``` and ```server.cert``` under **apache/ssl** and 
then uncomment lines 8 and 9 at apache/Dockerfile

<br/>

### php-fpm

---

PHP-FPM with PHP 7.4

<br/>

### mysql

---

Standalone MySQL 8.0 server

Port *:3306

<br/>

### redis

---

Standalone Redis 6.0 instance

Port *:6379
