FROM debian:9
MAINTAINER Subhadip Ghosh (subhadip.sky@gmail.com)
RUN apt-get update
RUN apt-get install -y openjdk-8-jre
COPY target/*jar /opt/naming-server.jar
ENTRYPOINT ["/usr/bin/java", "-jar", "/opt/naming-server.jar"]
EXPOSE 8761
