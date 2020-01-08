FROM java:8-jre
WORKDIR usr/src
ENV MYSQL_HOST=localhost:3306
ENV MYSQL_USER=root
ENV MYSQL_PASSWORD=root
ENV MYSQL_DATABASE=keepNote
ENV MYSQL_CI_URL=jdbc:mysql://${MYSQL_HOST}/${MYSQL_DATABASE}
ADD ./target/ReminderService-0.0.1-SNAPSHOT.jar /usr/src/ReminderService-0.0.1-SNAPSHOT.jar
EXPOSE 9001
ENTRYPOINT ["java","-jar","ReminderService-0.0.1-SNAPSHOT.jar"]
