#
# Base image to all java related containers
#
FROM centos
MAINTAINER Jorge Morales <jmorales@redhat.com>

# Update the system
RUN yum -y update; yum -y install java-1.7.0-openjdk-devel unzip wget tar; yum clean all
ENV JAVA_HOME /usr/lib/jvm/java

CMD ["/bin/bash","-l"]

