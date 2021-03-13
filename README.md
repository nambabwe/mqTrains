# mqTrains
Model railroad electronics using MQTT

www.mqTrains.com

Upload with:

Linux, Pi, MacOS:
sudo apt-get install python python-pip
sudo pip install esptool

esptool.py --chip esp8266 --port /dev/ttyUSB0 --baud 460800 --before default_reset --after hard_reset write_flash 0x0 mqTrains_ServoPCA_0.98_1MB.bin 

Windows:
Use nodemcu-flasher (https://github.com/nodemcu/nodemcu-flasher) with Baudreate 230400m Flash size 1MByte, Flash speed 40MHz AND SPI Mode DOUT

