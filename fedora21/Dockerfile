FROM fedora:21

MAINTAINER Michaël Rigart <michael@netronix.be>

RUN echo "====> Installing sudo... <====" && \
    yum -y install sudo && \
    \
    \
    echo "====> Installing Ansible... <====" && \
    yum -y install ansible && \
    \
    \
    echo "====> Installing Git... <====" && \
    yum -y install git && \
    \
    \
    echo "====> Removing unused YUM resources... <====" && \
    yum clean all

CMD [ "ansible-playbook", "--version" ]
