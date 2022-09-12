FROM --platform=amd64 openjdk:8-jdk-slim
RUN mkdir /scouter
ADD ./scouter/agent.host /scouter
WORKDIR /scouter
CMD ["java", "-classpath", "/scouter/scouter.host.jar", "scouter.boot.Boot", "/scouter/lib"]
