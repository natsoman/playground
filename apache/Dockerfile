FROM httpd:2.4.41-alpine

COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
COPY ./httpd-vhosts.conf /usr/local/apache2/conf/extra/httpd-vhosts.conf
COPY ./example.com.conf /usr/local/apache2/conf/extra/example.com.conf
COPY ./index.html /usr/local/apache2/htdocs/example/public/index.html

# COPY ./ssl/server.cert /usr/local/apache2/conf/server.cert
# COPY ./ssl/server.key /usr/local/apache2/conf/server.key

WORKDIR /usr/local/apache2/htdocs/

EXPOSE 80