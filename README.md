# PHD2-2.6.11dev6


Install the dependency library for OPENPHD2
-
    sudo apt-get install build-essential git cmake pkg-config libwxgtk3.0-gtk3-dev \
       wx-common wx3.0-i18n libindi-dev libnova-dev gettext zlib1g-dev libx11-dev \
       libcurl4-gnutls-dev

Compilation and installation:
-
Enter the QUARCS_phd2 project directory and open the terminal

    mkdir BUILD
    cd BUILD
    cmake .. 
    make -j4
    sudo make install
