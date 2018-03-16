FROM tomcat:8.5
WORKDIR /usr/local/tomcat/conf
COPY tomcat-users.xml .
WORKDIR /usr/local/tomcat/webapps/manager/META-INF
COPY context.xml .
WORKDIR /usr/local/tomcat/webapps/host-manager/META-INF
COPY context.xml .
WORKDIR /usr/local/tomcat
