# Dockerfile

# Author       : Munawar
# Github       : https://github.com/Munawar9488
# Messenger    : https://m.me/Munawar9488
# Email        : munawarmujahid3749@gmail.com
# Date         : 08-07-2023
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/Munawar9488/SCAMER"

# Working directory
WORKDIR /SCAMER/
# Add files 
ADD . /SCAMER

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "maxphisher.py", "--noupdate"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t Munawar9488/SCAMER:latest", "sudo docker run --rm -it Munawar9488/SCAMER:latest"

## "sudo docker pull Munawar9488/SCAMER", "sudo docker run --rm -it Munawar9488/SCAMER"