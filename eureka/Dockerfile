FROM tomcat:7.0.85-jre8

EXPOSE 80

ADD eureka-server-1.8.8-SNAPSHOT.war /opt/tomcat/webapps/

ADD server.xml /opt/tomcat/conf/

CMD ["catalina.sh", "run"]
