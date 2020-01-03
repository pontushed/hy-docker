FROM openjdk:8
RUN apt-get update && apt-get install git
WORKDIR /root
RUN git clone https://github.com/docker-hy/spring-example-project
WORKDIR /root/spring-example-project
RUN ./mvnw package
EXPOSE 8080
ENTRYPOINT ["/usr/local/openjdk-8/bin/java","-jar"]
CMD ["./target/docker-example-1.1.3.jar"]
