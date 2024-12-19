FROM openjdk:8u151-jdk-alpine3.7

EXPOSE 8070

# ENV APP_HOME /usr/src/app

# COPY target/*.jar $APP_HOME/app.jar

# WORKDIR $APP_HOME

# ENTRYPOINT exec java -jar app.jar
# Dockerfile improvements
ENV APP_HOME=/usr/src/app

# Ensure the JAR file is copied correctly
COPY target/shopping-cart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

# Use JSON format for ENTRYPOINT
ENTRYPOINT ["java", "-jar", "/usr/src/app/app.jar"]
