#
# Base image to all jboss related "non X11" docker images. 
#
FROM jorgemoralespou/java
MAINTAINER Jorge Morales <jorgemoralespou@gmail.com>

RUN groupadd -r jboss -g 1000 && useradd -u 1000 -r -g jboss -d /opt/jboss -s /sbin/nologin -c "JBoss user in Docker" jboss \
    && mkdir /opt/jboss \
    && chown -R jboss:jboss 

WORKDIR /opt/jboss

ENV HOME /opt/jboss

USER jboss
