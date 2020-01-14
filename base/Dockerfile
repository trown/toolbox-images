FROM registry.fedoraproject.org/f31/fedora-toolbox:31

RUN dnf -y copr enable alwaysrookie/alacritty
RUN dnf -y install alacritty fish vim bind-utils jq make openssl-devel protobuf-devel

RUN rpm --import https://packages.microsoft.com/keys/microsoft.asc
COPY code.repo /etc/yum.repos.d/code.repo
RUN dnf -y install code libX11-xcb

RUN rm -f /etc/yum.repos.d/code.repo
RUN dnf -y copr disable alwaysrookie/alacritty
