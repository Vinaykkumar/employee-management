# Use an official OpenJDK runtime as a parent image
FROM openjdk:17

# Set the working directory to /app
WORKDIR /

# Copy the Spring Boot JAR file from the target directory to the root of the container
ADD target/employeemanagmentbackend-0.0.1-SNAPSHOT.jar employeemanagmentbackend-0.0.1-SNAPSHOT.jar

# Expose port 8080 for the Spring Boot application
EXPOSE 8080

# Specify the command to run your Spring Boot application
CMD ["java", "-jar", "employeemanagmentbackend-0.0.1-SNAPSHOT.jar"]
