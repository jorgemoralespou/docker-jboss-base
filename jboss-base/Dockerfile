#
# Base image to all jboss related "non X11" docker images. 
#
FROM jmorales/java
MAINTAINER jmorales <jmorales@redhat.com>

RUN groupadd -r jboss -g 433 && useradd -u 431 -r -g jboss -d /home/jboss -s /sbin/nologin -c "Docker image user" jboss && mkdir /home/jboss && chown -R jboss:jboss /home/jboss && echo "jboss:jboss" | chpasswd && echo "root:root" | chpasswd
#RUN groupadd -r jboss -g 433 && useradd -u 431 -r -g jboss jboss && mkdir /home/jboss && chown -R jboss:jboss /home/jboss && echo "jboss:jboss" | chpasswd && echo "root:root" | chpasswd
USER jboss
ENV HOME /home/jboss
WORKDIR /home/jboss

CMD ["/bin/bash","-l"]

