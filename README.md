# PHD2-2.6.11dev6


安装OPENPHD2的依赖库
-
    sudo apt-get install build-essential git cmake pkg-config libwxgtk3.0-gtk3-dev \
       wx-common wx3.0-i18n libindi-dev libnova-dev gettext zlib1g-dev libx11-dev \
       libcurl4-gnutls-dev

编译过程：
-
进到QUARCS_phd2工程目录下打开终端

    mkdir BUILD
    cd BUILD
    cmake .. 
    make -j4
    sudo make install
