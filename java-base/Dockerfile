#
# Base image to all java related containers
#
FROM fedora:20
MAINTAINER Jorge Morales <jorgemoralespou@gmail.com>

# Update the system
RUN yum -y update && yum clean all
RUN yum -y install bsdtar unzip augeas java-1.7.0-openjdk-devel \
    && yum clean all
ENV JAVA_HOME /usr/lib/jvm/java

CMD ["/bin/bash","-l"]

