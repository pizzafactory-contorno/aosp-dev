FROM docker.io/pizzafactory0contorno/piatto-quadrato:ubuntu-22.04_broadway@sha256:7dc4576b68a16ca7c1e7d1639ab686f3606c1a7c878663509ffda9bc098f3574


USER root
RUN apt-get update \
 && DEBIAN_FRONTEND=noninteractive apt-get install -y \
      git-core gnupg flex bison build-essential zip curl zlib1g-dev libc6-dev-i386 libncurses5 \
      x11proto-core-dev libx11-dev lib32z1-dev libgl1-mesa-dev libxml2-utils xsltproc unzip fontconfig \
      repo openssh-client \
      meson dosfstools mtools e2fsprogs \
      fdisk kpartx \
      pkg-config python3-mako python3-jinja2 python3-ply python3-yaml \
      psmisc \
 && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y \
 && apt-get clean && rm -rf /var/lib/apt/lists/*
USER user
