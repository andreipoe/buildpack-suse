FROM registry.suse.com/suse/sle15:15.7
LABEL maintainer "Andrei Poenaru <docker@simd.stream>"

RUN zypper install -y \
    autoconf \
    automake \
    awk \
    bzip2 \
    libbz2-devel \
    cmake \
    curl \
    dirmngr \
    gcc \
    gcc-c++ \
    git \
    glib2-devel \
    gzip \
    kernel-devel \
    libcurl-devel \
    libevent-devel \
    libffi-devel \
    libjpeg8-devel \
    libopenssl-devel \
    libxml2-devel \
    libxslt-devel \
    make \
    ncurses-devel \
    openssl \
    postgresql-devel \
    procps \
    readline-devel \
    sqlite3-devel \
    tar \
    wget \
    which \
    xz \
    zlib-devel \
    && zypper clean --all

# byacc is not available in the SLES 15.7 repo
RUN wget https://download.opensuse.org/repositories/devel:/tools:/compiler/15.6/x86_64/byacc-20260126-lp156.70.1.x86_64.rpm && \
    rpm -i byacc-20260126-lp156.70.1.x86_64.rpm && \
    rm -f byacc-20260126-lp156.70.1.x86_64.rpm
