FROM debian:9
MAINTAINER Subhadip Ghosh (subhadip.sky@gmail.com)
RUN apt-get update
RUN apt-get install -y openjdk-8-jre
COPY target/*jar /opt/currencyconversion.jar
ENTRYPOINT ["/usr/bin/java", "-jar", "/opt/currencyconversion.jar", "-Dserver.port=\"8100\""]
EXPOSE 8100
