#
# Base image to all java related containers
#
FROM fedora:20
MAINTAINER Jorge Morales <jorgemoralespou@gmail.com>

# Update the system
RUN yum -y update \
    && yum -y install java-1.7.0-openjdk-devel bsdtar unzip augeas
    && yum clean all
ENV JAVA_HOME /usr/lib/jvm/java

CMD ["/bin/bash","-l"]

