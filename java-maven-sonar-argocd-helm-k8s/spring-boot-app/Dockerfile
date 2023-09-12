FROM abhishekf5/maven-abhishek-docker-agent:v1

# Simply the artifact path
#ARG artifact=target/spring-boot-web.jar

# Set the working directory inside the container
WORKDIR /opt/app

# Copy all files from the current directory into the container
COPY . .

# Run Maven to install dependencies and build the application
RUN mvn install

# Copy the built JAR file into the container
#COPY ${artifact} app.jar

# Define the entry point for the container
ENTRYPOINT ["java", "-jar", "target/spring-boot-web.jar"]






