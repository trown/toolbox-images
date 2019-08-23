FROM registry.fedoraproject.org/f30/fedora-toolbox:30

RUN dnf -y copr enable skidnik/termite
RUN dnf -y install termite fish vim bind-utils jq make

RUN rpm --import https://packages.microsoft.com/keys/microsoft.asc
COPY code.repo /etc/yum.repos.d/code.repo
RUN dnf -y install code libX11-xcb
