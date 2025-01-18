FROM openjdk:17
WORKDIR /App

# Copy the Maven project files (pom.xml and source code) to the Docker image
COPY pom.xml /app
COPY src /app/src

# Install Maven
RUN apt-get update && apt-get install -y maven

# Run the Maven build
RUN mvn clean install

COPY /target/Point-of-sale-0.0.1-SNAPSHOT.jar .


ENTRYPOINT ["java", "-jar" , "Point-of-sale-0.0.1-SNAPSHOT.jar"]









