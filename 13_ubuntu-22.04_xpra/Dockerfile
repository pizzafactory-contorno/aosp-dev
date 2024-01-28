FROM docker.io/pizzafactory0contorno/piatto-quadrato:ubuntu-22.04_xpra@sha256:9ba0fbce537463848ae52834b1747889ae9893588f057ab8c8f040e798e80835


USER root
RUN apt-get update \
 && DEBIAN_FRONTEND=noninteractive apt-get install -y \
      git-core gnupg flex bison build-essential zip curl zlib1g-dev libc6-dev-i386 libncurses5 \
      x11proto-core-dev libx11-dev lib32z1-dev libgl1-mesa-dev libxml2-utils xsltproc unzip fontconfig \
      repo openssh-client \
      meson dosfstools mtools e2fsprogs \
      fdisk kpartx \
      pkg-config python3-mako python3-jinja2 python3-ply python3-yaml \
 && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y \
 && apt-get clean && rm -rf /var/lib/apt/lists/*
USER user
