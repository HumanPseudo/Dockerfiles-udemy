FROM centos

RUN yum install httpd -y

WORKDIR /var/www/html

COPY startbootstrap-freelancer-master .

ENV contenido what does the fox say

RUN echo "$contenido" > /var/www/html/prueba.html

CMD apachectl -DFOREGROUND
