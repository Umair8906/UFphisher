# Dockerfile

# Author       : UMAIR
# Github       : https://github.com/Umair8906
# Messenger    : 
# Email        : 
# Date         : 25-08-2021
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/Umair8906/UFPhisher"

# Working directory
WORKDIR /UFPhisher/
# Add files 
ADD . /UFPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "UFphisher.py", "--noupdate"]

## 