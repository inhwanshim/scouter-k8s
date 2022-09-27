#FROM --platform=amd64 openjdk:8-jdk-slim
#RUN mkdir /scouter
#ADD ./scouter/agent.host /scouter
#WORKDIR /scouter
#CMD ["java", "-classpath", "/scouter/scouter.host.jar", "scouter.boot.Boot", "/scouter/lib"]
FROM tomcat:10.0

ENV TOMCAT_HOME /usr/local/tomcat
COPY agent.java /opt/scouter/agent.java
COPY catalina.sh $TOMCAT_HOME/bin/catalina.sh

EXPOSE 6180/tcp
EXPOSE 6188/tcp
EXPOSE 8080/tcp
EXPOSE 6100/tcp
EXPOSE 6100/udp

#RUN chown -R test:test /usr/local/tomcat

WORKDIR ${TOMCAT_HOME}/bin
CMD ["catalina.sh", "run"]
