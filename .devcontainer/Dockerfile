FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash - \
    && apt-get install -y nodejs

RUN apt-get update && apt-get install -y openjdk-17-jdk

RUN apt-get install -y docker.io

RUN node --version && java -version
