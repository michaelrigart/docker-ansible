FROM fedora:22

MAINTAINER Michaël Rigart <michael@netronix.be>

RUN echo "====> Installing sudo... <====" && \
    dnf -y install sudo && \
    \
    \ 
    echo "====> Installing Ansible... <====" && \
    dnf -y install ansible && \
    \
    \
    echo "====> Installing Git... <====" && \
    dnf -y install git && \
    \
    \
    echo "===> Removing unused DNF resources... <====" && \
    dnf clean all

CMD [ "ansible-playbook", "--version" ]
