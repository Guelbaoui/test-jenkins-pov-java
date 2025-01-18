FROM openjdk:17
WORKDIR /app

# Copy the Maven project files (pom.xml and source code) to the Docker image
COPY pom.xml .
COPY src ./src



# Copy the built JAR file
COPY target/Point-of-sale-0.0.1-SNAPSHOT.jar .

ENTRYPOINT ["java", "-jar" , "Point-of-sale-0.0.1-SNAPSHOT.jar"]

