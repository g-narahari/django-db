FROM mcr.microsoft.com/devcontainers/python:3.11

# Install system packages for MySQL and Django support
RUN apt-get update && \
    apt-get install -y mysql-server libmysqlclient-dev && \
    apt-get clean

# Start MySQL service by default in container
CMD ["bash", "-c", "sudo service mysql start && bash"]
