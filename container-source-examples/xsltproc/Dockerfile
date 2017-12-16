FROM registry.fedoraproject.org/fedora:latest
RUN dnf install -y libxslt docbook-slides && dnf clean all
WORKDIR /data
ENTRYPOINT [ "/usr/bin/xsltproc" ]
LABEL RUN_OPTS ""
