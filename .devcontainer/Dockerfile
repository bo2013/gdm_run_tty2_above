FROM archlinux:base-devel

RUN pacman -Syu --noconfirm && \
    pacman -S --needed --noconfirm sudo git && \
    pacman -Scc --noconfirm

RUN useradd -m -s /bin/bash builder && \
    echo "builder ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers && \
    visudo -c