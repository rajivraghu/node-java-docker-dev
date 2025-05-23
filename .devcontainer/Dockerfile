# Base image from Microsoft's Dev Container collection
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Update and install OpenJDK 17
RUN apt-get update && \
    apt-get install -y openjdk-17-jdk && \
    apt-get clean

# Verify Java installation
RUN java -version

# Install JBang
RUN curl -Ls https://sh.jbang.dev | bash -s - app setup

# Install Node.js and npm (necessary for npm packages)
# Using NodeSource for a more recent and stable Node.js version
RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash - && \
    apt-get install -y nodejs && \
    apt-get clean

# Install the @anthropic-ai/claude-code npm package globally
RUN npm install -g @anthropic-ai/claude-code
