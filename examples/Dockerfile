# Use a base image with Java
FROM openjdk:17-slim

# Set working directory inside container
WORKDIR /app

# Copy source file into container
COPY Main.java .

# Compile Java code
RUN javac Main.java

# Command to run the app
CMD ["java", "Main"]
