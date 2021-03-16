# esphome

Suport for EASYHOME funktsteckdosen 433mhr, (wireless sockets) with esphome to connect with homeassistant.
DHT detector also in the code

# install

clone repository

open livingroom.yaml 
change ssid and the password of the wifi

open terminal and write:

cd /REPO_PATH 

if using cable (first time always like this):
sudo docker run --rm -v "${PWD}":/config --device=/dev/ttyUSB0 -it esphome/esphome livingroom.yaml run

OTA:
sudo docker run --rm -v "${PWD}":/config -it esphome/esphome livingroom.yaml run


# Documentation

esphome:

https://esphome.io

rc-switch and the radio protocol in general:

https://github.com/sui77/rc-switch/issues/135
https://github.com/sui77/rc-switch/wiki/Add_New_Remote_Part_1
https://github.com/sui77/rc-switch/issues/103
https://esphome.io/components/remote_transmitter.html#remote-transmitter-rc-switch-protocol
https://esphome.io/components/remote_transmitter.html#remote-setting-up-rf
https://esphome.io/components/remote_transmitter.html
https://test.sui.li/oszi/

