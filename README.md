# Raspberrypi initialisation script
RPi basic initialisation and configuration script. Use [raspi-config](https://github.com/RPi-Distro/raspi-config) in non-interactive mode with commands found in [here](https://github.com/raspberrypi/rc_gui/blob/master/src/rc_gui.c).
The main idea is to automatize : hostname change, new user creation with password change and pi profile copy (groups, home folder), ssh update (change port and restrict connection from newly created user).

## Uses
* `bash script1` will ask you inline and when needed the differents stuff (hostname...)
* `bash script1 -H hostname -u username -p 1234` will handle everything except password change for newly created user. This is the way used by [my configuration script](https://github.com/devgiants/raspberry-configuration).
 
## Following closely :
* [wiringPi for PHP](https://github.com/WiringPi/WiringPi-PHP) library installation (include [wiringPi](https://github.com/WiringPi/WiringPi) as git submodule
* Custom "module" (in generic sense) to handle GPIOs interrupts like described by Drogon [here](https://www.raspberrypi.org/forums/viewtopic.php?f=44&t=9207#p146408)
* Software packages : mDNS, Apache, PHP, MySQL...
* SILEX Boilerplate
* ...
