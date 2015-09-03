FROM centos:centos6

MAINTAINER Michaël Rigart <michael@netronix.be>

RUN echo "====> Installing EPEL... <====" && \
    yum -y install epel-release && \
    \
    \
    echo "====> Installing sudo... <====" && \
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
    yum -y remove epel-release && \
    yum clean all

CMD [ "ansible-playbook", "--version" ]
