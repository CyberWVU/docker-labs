# Builds a machine out with modified users and passwords.
FROM ubuntu:14.04
MAINTAINER CyberWVU

COPY /files/passwd /etc/passwd
COPY /files/shadow /etc/shadow

RUN apt-get update && apt-get install -y openssh-server

EXPOSE 22
CMD ["/usr/bin/sshd", "-D"]
