# Reverse Engieniered EASYHOME Funktsteckdosen 433MHr 

This project allows you to control with your home IOT integration a radio controled power sockets EASYHOME Funktsteckdosen.
It has been reverse ingeniered to find the rc-switch protocols used for each button.

In may case thi software suports the EASYHOME funktsteckdosen 433mhr wireless sockets, with esphome to connect with my homeassistant. A DHT detector has also been added into the code thus is not necesary.

# Hardware needed:

Esp32 or similar with 433MHr radio emmisor connected, a repceptor is also convenient for debugging porpouses.

# Install:

clone repository

change ssid and the password of the wifi in the file:

livingroom.yaml 

Open the terminal and go to the path of the repository:

> cd /REPO_PATH 

Connect the ESP32 to your computer using a wired connection (updates can be done using OTA) and execute:

> sudo docker run --rm -v "${PWD}":/config --device=/dev/ttyUSB0 -it esphome/esphome livingroom.yaml run

For OTA (Over The Air update):

> sudo docker run --rm -v "${PWD}":/config -it esphome/esphome livingroom.yaml run


# Documentation:

Documentation useful for the reverse ingeniering proccess, rc-switch and the radio protocol in general:

https://github.com/sui77/rc-switch/issues/135
https://github.com/sui77/rc-switch/wiki/Add_New_Remote_Part_1
https://github.com/sui77/rc-switch/issues/103
https://esphome.io/components/remote_transmitter.html#remote-transmitter-rc-switch-protocol
https://esphome.io/components/remote_transmitter.html#remote-setting-up-rf
https://esphome.io/components/remote_transmitter.html
https://test.sui.li/oszi/

Esphome documentation:

https://esphome.io
