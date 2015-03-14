An Arduino based controller, transmitter and receiver system for Astromech R-Series droids.

Requirements:
Arduino IDE 1.0 is required.
Digi XBee Series 2 operating API 2 mode, Pro series is optional & encouraged. Series 1 & 2.5 or clones are not supported, however may work with code changes.


Arduino Mega 2560 or better are needed for the Controller and Receiver due to variable memory requirement.


The design is a very modular, RF controller & receiver with optional additional modules. The RSeries receiver can operate as a centralized or distributed depending on your requirements.

The RSeries Controller & Receiver are shields that fit Arduino Mega 2560 [R1](https://code.google.com/p/rseries-open-control/source/detail?r=1) to [R3](https://code.google.com/p/rseries-open-control/source/detail?r=3), while the I2C FX Module is a Arduino Uno shield for [R1](https://code.google.com/p/rseries-open-control/source/detail?r=1) to [R3](https://code.google.com/p/rseries-open-control/source/detail?r=3) as well.

The SlipRing Interface, is a stand alone upto 24 Wire SlipRing interface at 2amps to pass signals, (Servo, Audio, I2C & Power) between the Dome & Body of the astromech via the slip ring via DB-25 connectors.

Some may just wish to use Controller/Receiver combination to trigger "Events" or actions in their astromech, and not actually control their droid motive systems.

It is possible to control other RC receivers, i.e. Spektrum & Hitech Aurora, with this effort, however that is currently outside of the scope of this project.

Digi XBee Series 2 are required to be running in API 2 mode.

PCB CAM/Gerber Files are also available for Download for submission to PCB fab houses, and we highly recommend pcb.laen.org.

PCBs are available directly at http://store.oshpark.com/collections/droid-parts

Build time ranges from 3hrs to 6hrs with all modules.

## Forks! ##
Some talented builders have reworked the RSeries code, made it their own and graciously shared their hard work with the community.

  * Micke's TUSCEN project can be found [here](http://astromech.net/forums/showthread.php?t=13496).
  * Skwerl's fork is detailed [here](http://astromech.net/forums/showthread.php?t=16108) and the code can be found [here](https://github.com/Skwerl/rseries).