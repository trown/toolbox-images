FROM registry.fedoraproject.org/f33/fedora-toolbox:33

RUN dnf -y install alacritty fish vim bind-utils jq make openssl-devel protobuf-devel tmate

RUN rpm --import https://packages.microsoft.com/keys/microsoft.asc
COPY code.repo /etc/yum.repos.d/code.repo
RUN dnf -y install code libX11-xcb

RUN rm -f /etc/yum.repos.d/code.repo
