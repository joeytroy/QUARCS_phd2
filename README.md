# QUARCS_PHD2

<img align="left" src="https://www.raspberrypi.com/app/uploads/2020/06/raspberrry_pi_logo.png" width="48">

These instructions are written for **Ubuntu 24.04.1 LTS Server (64-bit) ARM** for **Raspberry Pi Models** Please make sure you have already installed the **QUARCS_QT-SeverProgram** or your install will not work correctly.

---

## 1. Install QUARCS_PHD2 2.6.11dev6
**Install QUARCS_PHD2 Prerequisites**
Run the following command to install prerequisites for QUARCS_PHD2:

    sudo apt-get install libwxgtk3.2-dev wx-common wx3.2-i18n libeigen3-dev libgtest-dev packaging-dev libopenmpi-dev -y

**Install QUARCS_PHD2**  
To install the QUARCS_PHD2:

    cd ~
    export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH
    git clone --branch RPi4_5 https://github.com/joeytroy/QUARCS_phd2.git
    cd QUARCS_phd2/phd2
    mkdir BUILD
    cd BUILD
    cmake .. 
    make -j$(nproc) 
    sudo make install

**Verification**  
To confirm QUARCS_PHD2 and QUARCS_QT-SeverProgram installation is working run the folloiwng command:

	cd ~
    client

You should see the client kick off and connect to PHD2 and open PHD2 through SSH. To close the service run the following keyboard commands **"ctrl+z"**

<img src="https://joeytroy.com/wp-content/uploads/2025/01/qhyclient_phd2.jpg" width="800">

This completes the installation of the **QUARCS_PHD2**. To proceed further, you will need to install **QUARCS_stellarium-web-engine**.

---

## Need Assistance?
If you need assistance, join the **[QUARCS Discord Discussion Group](https://discord.gg/uHTPfJ5uuV)** for support and discussions.     
