FROM centos

LABEL version=1.0
LABEL description="esta es una imagen de apache"
LABEL vendor=yo

RUN yum install httpd -y

COPY startbootstrap-freelancer-master /var/www/html

RUN echo "$(whoami)" > /var/www/html/user1.html

RUN useradd human

RUN chown human /var/www/html -R

USER human

RUN echo "$(whoami)" > /tmp/user2.html

USER root

RUN cp /tmp/user2.html /var/www/html/user2.html

CMD apachectl -DFOREGROUND
