# Initial Setup

## You Will Need

* Raspberry Pi (assuming v3)
* Micro SD card (with adapter if you need one)
* HDMI monitor plus cable (a TV will do)
* USB keyboard

Note that the monitor and keyboard are only needed temporarily.

## Get Raspbian on the SD card

https://www.raspberrypi.org/documentation/installation/installing-images/mac.md

## Plug Stuff In

Plug in the monitor, keyboard and SD card. Finally, the power.

## Log in and connect to Wi-Fi

https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md

Remember that you can add multiple network blocks, so that if you're planning on using
your Pi in another location it'll already know the Wi-Fi credentials.

## Connect via SSH

On another machine on the network, do `ssh pi@raspberrypi.local`. You should be able to log in (default password is `raspberry`).

## Initial Set Up Completed!

You can now shut the Pi down and remove the monitor and keyboard, as you can now just use SSH to control it.
