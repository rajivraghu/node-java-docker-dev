# Base image from Microsoft's Dev Container collection
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Update and install OpenJDK 17
RUN apt-get update && \
    apt-get install -y openjdk-17-jdk && \
    apt-get clean

# Verify Java installation
RUN java -version
