# esp8266-scratchpad
Random notes and information about esp8266 devices

# Unbricking/Flashing using a USB TTL cable
* Jumper GND to D3 (GPIO0)
* Attach USB TTL cable
  * Red to +5v
  * Black to GND
  * White to TX
  * Green to RX
* Press the reset button
* Load the sketch from Arduino

It may be necessary to use esptool.py to erase the flash:
```esptool.py --port /dev/cu.usbserial erase_flash```
