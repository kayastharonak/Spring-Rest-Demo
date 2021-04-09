FROM ubuntu:18.04

MAINTAINER kayastharonak@gmail.com

RUN apt-get update

RUN apt-get install openjdk-11-jre

RUN apt-get install maven

RUN RUN apt-get install -y git

RUN mkdir /root/.ssh/

ADD id_rsa /root/.ssh/id_rsa

RUN touch /root/.ssh/known_hosts

RUN git clone https://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@github.com/kayastharonak/Spring-Rest-Demo

RUN cd /demo

RUN mvn clean install

RUN cd /target

ENTRYPOINT ["java","-jar","/demo-0.0.1-SNAPSHOT.jar"]

