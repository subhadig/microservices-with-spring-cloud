FROM debian:9
MAINTAINER Subhadip Ghosh (subhadip.sky@gmail.com)
RUN apt-get update
RUN apt-get install -y openjdk-8-jre
COPY target/*jar /opt/forex.jar
ENTRYPOINT ["/usr/bin/java", "-jar", "/opt/forex.jar", "-Dserver.port=\"8000\""]
EXPOSE 8000
