# Ubuntu with ssh keys installed on multiple users
FROM ubuntu:14.04
MAINTAINER CyberWVU

RUN apt-get update && apt-get install openssh-server

COPY /files/authorized_keys /root/.ssh/authorized_keys

EXPOSE 22
CMD ["/usr/bin/sshd", "-D"]
