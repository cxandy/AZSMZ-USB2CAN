# AZSMZ-USB2CAN

## Where to get:
## http://bancuit.aliexpress.com

## Flashing new firmware
  [Flow me](/Firmware)
  
## 1.slcan firmware

CANables ship with slcan firmware. This firmware enumerates as a standard serial device on Linux, Mac, and Windows for easy interfacing. The CANable can be easily re-flashed with the candlelight firmware which enumerates as a native CAN device in Linux and a generic USB device in Windows.

On Linux the CANable works natively with slcand, so you can use all of the standard can-utils command-line utilities and even Wireshark to interact with the bus.

On Windows and Mac, the CANable works with [cantact-app](https://github.com/linklayer/cantact-app/releases/tag/v0.3.0-alpha). This is a simple Java application that shows CAN traffic in real-time and allows you to transmit messages on the bus.



## 2.candlelight Firmware

If you update to the candlelight firmware, the CANable shows up as a native CAN device with socketcan--no slcandrequired! Performance is higher than the serial-line firmware as slcand is bypassed entirely. With Linux and socketcan you can use all of the standard can-utils command-line utilities and even Wireshark to interact with the bus.

With candlelight on Windows and Linux you can use [cangaroo](http://canable.io/utilities/cangaroo-win32-%20b4a9d6d.zip) to interact with a CAN bus, no drivers required. Cangaroo provides time and aggregate trace capability, as well as raw and repeated raw TX. Beta DBC file parsing is implemented, and is currently under development.
