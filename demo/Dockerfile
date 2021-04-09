FROM ubuntu:18.04

MAINTAINER kayastharonak@gmail.com

RUN apt-get update

RUN apt-get install -y openjdk-11-jre 

RUN apt-get install -y maven

RUN apt-get install -y git

RUN git clone https://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@github.com/kayastharonak/Spring-Rest-Demo

RUN cd /Spring-Rest-Demo/demo && mvn clean install

ENTRYPOINT ["java","-jar","/Spring-Rest-Demo/demo/target/demo-0.0.1-SNAPSHOT.jar"]

