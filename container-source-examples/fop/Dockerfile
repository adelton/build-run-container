FROM registry.fedoraproject.org/fedora:latest
RUN dnf install -y fop /usr/share/fonts/dejavu/DejaVuSans-Bold.ttf /usr/share/fonts/dejavu/DejaVuSansMono.ttf && dnf clean all
WORKDIR /data
ENTRYPOINT [ "/usr/bin/fop" ]
LABEL RUN_OPTS "--tmpfs /tmp"
