FROM alpine:3.11

COPY . /app

RUN apk update \
    && apk fetch openjdk8 \
    && apk add openjdk8 \
    && apk add maven

WORKDIR /app

ENTRYPOINT ["mvn"]
CMD ["spring-boot:run"]
EXPOSE 8080
