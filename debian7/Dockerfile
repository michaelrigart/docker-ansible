FROM debian:wheezy

MAINTAINER Michaël Rigart <michael@netronix.be>

ENV DEBIAN_FRONTEND noninteractive

RUN echo "===> Installing python, sudo, and supporting tools..."  && \
    apt-get update  && \
    \
    \
    echo "====> Installing sudo... <====" && \
    apt-get install -y sudo && \
    \
    \
    echo "====> Installing python dependencies... <====" && \
    apt-get install -y python-dev python-pip && \
    \
    \
    echo "====> Installing Git... <====" && \
    apt-get install -y git && \
    \
    \
    echo "====> Installing Ansible... <====" && \
    pip install ansible

CMD [ "ansible-playbook", "--version" ]
