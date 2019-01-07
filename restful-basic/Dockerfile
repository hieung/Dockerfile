# Get Image from https://github.com/hieung/Dockerfile/tree/master/ubuntu16.04-java8
#FROM ubuntu16.04-java8
FROM anapsix/alpine-java

MAINTAINER HieuNG

# Build spring cloud project from https://github.com/hieung/springboot-cloud-microservice/tree/master/restful-basic
# Goto <springboot-cloud-microservice>/restful-basic/target/customer-0.0.1-SNAPSHOT.jar
COPY customer-0.0.1-SNAPSHOT.jar /customer-0.0.1-SNAPSHOT.jar

Expose 8080

# Execute Jar File
CMD ["java","-jar", "customer-0.0.1-SNAPSHOT.jar"]  