FROM openjdk:11-slim

WORKDIR /app

COPY . /app/

RUN javac SimpleHttpServer.java

EXPOSE 4000

CMD ["java", "SimpleHttpServer"]
