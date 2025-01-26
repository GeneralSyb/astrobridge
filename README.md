# Work In Progress, may not work and instructions may be incorrect
# AstroBridge
Basically just a barebones Raspberry Pi OS with INDI and the INDI webmanager installed. Can be used as a network bridge that allows you to run heavy loads on a computer or laptop, with the raspberry pi only acting as a bridge between your equipment and the network.

## Setup


## Building from scratch
INDI was installed according to this tutorial: https://astroisk.nl/raspberry-pi-5-indi/
It is meant for the Pi 5, but it works for the Pi 4 as well. Pi 3 doesn't seem to work as it seems to hang at some point, but the image should still work on the Pi 3.

The INDI web manager was installed according to the instructions on the github page: https://github.com/knro/indiwebmanager
The manager itself was installed with sudo pip install indiweb, but to get it to run in the background the repo was cloned and the file needed for the daemon was used.
