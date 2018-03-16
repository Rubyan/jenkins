FROM jenkins/jenkins:lts

USER root

RUN apt update && apt-get install zip

# Setup Maven
ENV MAVEN_VERSION 3.5.3

RUN curl -fsSL http://archive.apache.org/dist/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz | tar xzf - -C /usr/share \
  && mv /usr/share/apache-maven-$MAVEN_VERSION /usr/share/maven \
  && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn

ENV MAVEN_HOME /usr/share/maven
#COPY settings.xml /root/.m2/settings.xml
USER jenkins

