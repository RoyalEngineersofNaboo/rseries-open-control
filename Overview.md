# Introduction #
This project's goal is to develop a simply-executed and feature-rich method of controlling R-Series droids while keeping components modular, affordable and future-proof.

The principal design revolves around readily available Arduino microcontrollers.  XBee wireless modules are used used by a touchscreen controller to communicate back and forth with a receiver inside the droid. The receiver can then relay commands to the droid's motor drivers as well as optional AudioFX modules (also Arduino based), servo controllers or dome-lighting controllers.

# Controller #
The controller consists of an Arduino Mega 2560 with a custom shield. It includes headers for attaching a touchscreen, Wii nunchuk controller, SD card and an XBee wireless module. The Arduino is configured with a sketch to create a touchscreen GUI, read inputs from the touchscreen, nunchuk and any pushbuttons and then relay information to the droid's receiver using the XBee modules.

In turn, the receiver also receives telemetry data from the droid's receiver which can then be displayed on the touchscreen.

![https://rseries-open-control.googlecode.com/svn/images/controller-v4.png](https://rseries-open-control.googlecode.com/svn/images/controller-v4.png)

# Receiver #
![https://rseries-open-control.googlecode.com/svn/images/receiver-v3.png](https://rseries-open-control.googlecode.com/svn/images/receiver-v3.png)

# FX Modules #
FX Modules share the same PCB design.

![https://rseries-open-control.googlecode.com/svn/images/i2c-fx-v1.png](https://rseries-open-control.googlecode.com/svn/images/i2c-fx-v1.png)
## AudioFX ##
## ServoFX ##
## LogicFX ##

# Slip-Ring Interface #
![https://rseries-open-control.googlecode.com/svn/images/slipring-v3.png](https://rseries-open-control.googlecode.com/svn/images/slipring-v3.png)