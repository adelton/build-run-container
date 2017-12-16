FROM registry.fedoraproject.org/fedora:latest
RUN dnf install -y openldap-clients && dnf clean all
RUN mkdir /the-home
RUN touch /the-home/.ldaprc
LABEL RUN_OPTS "-v ~/.ldaprc:/the-home/.ldaprc"
ENV HOME /the-home
WORKDIR /data
ENTRYPOINT [ "/usr/bin/ldapsearch" ]
