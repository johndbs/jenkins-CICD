# Use the official Jenkins image as the base image
FROM jenkins/jenkins:lts

# Switch to the root user, to install Docker CLI
USER root

# Install the Docker CLI
RUN curl -fsSL https://get.docker.com -o get-docker.sh && sh get-docker.sh

# Add the jenkins user to the docker group
RUN usermod -aG docker jenkins

# Switch back to the jenkins user
USER jenkins
