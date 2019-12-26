FROM ubuntu:18.04

COPY . /app

RUN apt-get update \
    && apt-get install openjdk-8-jdk -y \
    && apt-get install maven -y

WORKDIR /app

ENTRYPOINT mvn spring-boot:run
EXPOSE 8080
