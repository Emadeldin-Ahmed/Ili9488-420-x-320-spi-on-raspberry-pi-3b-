# Ili9488-420-x-320-spi-on-raspberry-pi-3b-
how to use an ili9488 display on a Raspberry Pi 3B+ using fbcp-ili9341

check the

After making the hardware connections and the first boot, I did this.

Edit the file /boot/config.txt
sudo nano /boot/config.txt

And if you find the following line:
dtparam=spi=on

Put a # in front of that line so that the line looks like this:
#dtparam=spi=on

Next is the installation of the FBCP driver and its configuration for the ILI9488 display.
cd ~

sudo apt update

sudo apt install libraspberrypi-dev
