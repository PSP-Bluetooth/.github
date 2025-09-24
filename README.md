# PSP Bluetooth

PSP Bluetooth is a project to bring Bluetooth controllers to 2000 and 3000 model PSP's.

It is broken down into multiple components.

## PSP Bluetooth Dongle
[Here](https://github.com/ste2425/PSP-Bluetooth-Dongle)

This is the firmware that runs on an ESP32 microcontroller. Its job is to be the bridge betwen the controllers and the PSP. The PSP communicates with it via custom homebrew over a serial port exposed in the AV connector.

## PSP Bluetooth Av Connector
[Here](https://github.com/ste2425/PSP-Bluetooth-AVConnector)

This is the hardware needed for the Dongle firmware to run on. It's intended as a library providing the a connector to plug into the PSPs AV port as well as a footprint to use an original AV connector socket from the PSP's motherboard.
It is intended that others build their own PCB's using the components from this library. However there are two sample projects you can use, a simple connector breakout and a development board which includes the required logic level converter.

## PSP Bluetooth Tech Demo
[Here](https://github.com/ste2425/PSP-Bluetooth-TechDemo)

This ia a PSP homebrew app to act as a tech demo demonstrating what can be done with bluetooth controllers.

## PSP Bluetooth plugin - Coming soon
This will be a plugin that can be run by CFW to patch controller data into the PSP to allow a single Bluetooth controller to be used accross all PSP games as well as the XMB.
