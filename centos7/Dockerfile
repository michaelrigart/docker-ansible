FROM centos:centos7

MAINTAINER Michaël Rigart <michael@netronix.be>

RUN echo "====> Installing EPEL... <====" && \
    yum -y install epel-release && \
    \
    \
    echo "====> Installing sudo... <====" && \
    yum -y install sudo && \
    \
    \
    echo "====> To avoid error: sudo: sorry, you must have a tty to run sudo... <====" && \
    sed -i -e "s/Defaults    requiretty.*/ #Defaults    requiretty/g" /etc/sudoers && \
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
