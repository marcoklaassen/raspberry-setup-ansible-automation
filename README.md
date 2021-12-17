# Setup Automation of Raspberry Pi with Ansible

## Prepare base image 

* Prepare SD Card & Write Image as described here: https://www.raspberrypi.com/documentation/computers/getting-started.html#using-raspberry-pi-imager
* Copy `ssh` & `wpa_supplicant.conf` from `boot` directory to sdcard as described here
    * configure network: https://www.raspberrypi.com/documentation/computers/configuration.html#configuring-networking
    * configure remote access: https://www.raspberrypi.com/documentation/computers/remote-access.html#ssh


## Basic Setup

run `ansible-playbook rpi-setup.yml -i hosts` in the `automation` folder to setup the pi user and ssh configuration

## Install Home Assistant 

run `ansible-playbook home-assistent-setup.yml -i hosts` in the `automation` folder to install and start Home Assistant Core directly to your Raspberry pi (https://www.home-assistant.io/installation/raspberrypi#install-home-assistant-core)