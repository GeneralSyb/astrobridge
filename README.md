# Work In Progress, may not work and instructions may be incorrect
# AstroBridge
Basically just a barebones Raspberry Pi OS with INDI and the INDI webmanager install. Can be used as a network bridge that allows you to run heavy loads on a computer or laptop, with the raspberry pi only acting as a bridge between your equipment and the network. Should work on the Raspberry Pi 3B and newer.

## Setup
Use the Raspberry Pi imager to write the img file to an SD card (minimum 16gb), add a [wpa_supplicant.conf](https://www.raspberrypi-spy.co.uk/2017/04/manually-setting-up-pi-wifi-using-wpa_supplicant-conf/ "wpa_supplicant.conf") file, put the SD card into the pi and power on the Pi. Find the IP of the Pi through the device list of your router or use an app like PingTools. Enter the IP address of the Pi in the Ekos equipment profile.

## Building from scratch
INDI was installed according to this tutorial: https://astroisk.nl/raspberry-pi-5-indi/
It is meant for the Pi 5, but it works for the Pi 4 as well. Pi 3 doesn't seem to work as it seems to hang at some point, but the image should still work on the Pi 3.

The INDI web manager was installed according to the instructions on the github page: https://github.com/knro/indiwebmanager
The manager itself was installed with `sudo pip install indiweb`, but to get it to run in the background the repo was cloned and the file needed for the daemon was used.

### SSH Access
Default login is `pi` with password `raspberry`
