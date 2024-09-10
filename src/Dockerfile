# Use a base image with Java 11 installed
FROM openjdk:11-jre-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the JMusicBot JAR file and example config file to the container
# Make sure to replace "JMusicBot-X.Y.Z.jar" with the actual filename
COPY JMusicBot-X.Y.Z.jar /app/JMusicBot.jar
COPY config.txt /app/config.txt

# Expose the port that JMusicBot will use (replace with the actual port if necessary)
EXPOSE 9000

# Set the entrypoint to run the JMusicBot JAR file
ENTRYPOINT ["java", "-Dnogui=true", "-jar", "/app/JMusicBot.jar"]
