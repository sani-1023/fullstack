FROM maven:3.8-openjdk-17 AS build
EXPOSE 8080
LABEL authors="sani"
ADD target/sqlproject.jar sqlproject.jar

ENV TZ=Asia/Dhaka
RUN ln -fs /usr/share/zoneinfo/$TZ /etc/localtime
ENTRYPOINT ["java", "-jar", "/sqlproject.jar"]