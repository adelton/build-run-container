FROM registry.fedoraproject.org/fedora:latest
RUN dnf install -y subversion && dnf clean all
WORKDIR /data
ENTRYPOINT [ "/usr/bin/svn" ]
