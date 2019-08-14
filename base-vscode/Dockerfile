FROM quay.io/alwaystherookie/toolbox-images:base

RUN rpm --import https://packages.microsoft.com/keys/microsoft.asc
COPY code.repo /etc/yum.repos.d/code.repo
RUN dnf -y install code libX11-xcb
