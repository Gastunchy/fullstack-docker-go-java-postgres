FROM amazoncorretto:21-alpine-jdk

WORKDIR /app

COPY . .

EXPOSE 8080

RUN apk add --no-cache maven=3.9.5-r0 \
&& mvn clean install

CMD [ "java", "-jar", "./target/words.jar" ]