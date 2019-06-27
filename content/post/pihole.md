---
title: "Pihole"
date: 2019-06-26T22:55:28-05:00
---

![Mad As Hell](/images/MadAsHell.jpeg)

I can't take it anymore.  I just can't take it.  The unending slew of ads are taking their toll.  Wasting of bandwidth and certainly frustrating when they cause the @#$& content to not render correctly.  Tonight's project is building and using a Pi-Hole for my network.

1. Get [Raspbian](https://www.raspberrypi.org/downloads/raspbian/)  (There a couple of OS's that would work but I'm going for simple.)  
1. Get [Etcher](https://www.balena.io/etcher/)  (Again, you can use a couple of different tools to flash a microSD card.)  
1. Enable SSH by mounting the flashed card and touch a ssh file.  
    ```
    touch /mnt/chad/boot/ssh
    ```  
1. Setup access to your WiFi  
    ```
    vi /mnt/chad/boot/wpa_supplicant.conf
    ```
    Edit the contents as needed.  
    ```
    country=US
    ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
    update_config=1
    
    network={
        ssid="NETWORK-NAME"
        psk="NETWORK-PASSWORD"
    }
    ```
1. Boot the device and then ssh into it.  (default password is raspberry)
    ```
    ssh pi@raspberry.local
    ```
1. Change the default password and I guess if you want to change the hostname.
    ```
    sudo raspi-config
    ```
1. Update and upgrade
    ```
    sudo apt-get update -y
    sudo apt-get upgrade -y
    ```
1. Instal Pi-Hole software.
    ```
    cd /tmp
    wget -O basic-install.sh https://install.pi-hole.net
    sudo bash basic-install.sh
    ```
1. Setup your Google WiFi to make the current IP address for your Pi-Hole to be static and make that your DNS.

...
TODO
Aaaannnnnddddd I'm too tired to finish documenting at this time.  