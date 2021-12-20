FROM httpd:alpine

COPY index.html /usr/local/apache2/htdocs/

COPY httpd.conf /usr/local/apache2/conf

EXPOSE 9999

ENV CONTAINER docker

#vCMD echo $CONTAINER

ENTRYPOINT ["/bin/sh", "-c" , "echo $CONTAINER && httpd-foreground"]