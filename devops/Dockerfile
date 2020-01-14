FROM quay.io/alwaystherookie/toolbox-images:base

RUN dnf -y install pass kubernetes-client python2 postgresql python3-yaml python3-pytest bat asciinema

RUN dnf -y copr enable vbatts/bazel
RUN dnf -y install bazel
RUN dnf -y copr disable vbatts/bazel
