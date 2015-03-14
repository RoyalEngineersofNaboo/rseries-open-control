

# Introduction #
The control system relies on XBee modules to allow our controller to talk to the receiver wirelessly. One module is mounted to the Controller Shield and acts as a 'Coordinator'. Another is mounted to the Receiver Shield and acts as a 'Router' for commands to and from the controller.
# Recommended Parts #
Most XBee parts are available to buy directly from their manufacturer (Digi) or from distributors such as Digi-Key or Newark.

## Controller ##
  * **XBee Module** : XBee-PRO ZB S2B module w/ U.Fl antenna connector
    * Model Number : XBP24BZ7UIT-004
    * Digi-Key : [602-1257-ND](http://search.digikey.com/scripts/DkSearch/dksus.dll?x=22&y=13&lang=en&site=us&KeyWords=XBP24BZ7UIT-004)
    * Digi : http://www.digi.com/products/model?mid=3588
  * **Antenna Cable** : U.Fl female to RPSMA female 4"
    * Part Number : JF1R6-CR3-4I
    * Digi-Key : [JF1R6-CR3-4I](http://parts.digikey.com/1/parts/26446-rf-cable-assy-jf1r6-cr3-4i.html)
    * Digi : http://www.digi.com/products/model?mid=2602
  * **Antenna** : 2.4GHZ Dipole Half-Wave, 2.1 dBi, RPSMA male, articulating
    * Part Number : A24-HASM-450
    * Digi-Key : [A24-HASM-450-ND](http://parts.digikey.com/1/parts/635412-ant-2-4ghz-dipole-half-wave-a24-hasm-450.html)
    * Digi : http://www.digi.com/products/model?mid=2603


## Receiver ##
  * **XBee Module** : XBee-PRO ZB S2B module with RPSMA connector
    * Model Number : XBP24BZ7SIT-004
    * Digi-Key : [602-1103-ND](http://parts.digikey.com/1/parts/1586162-module-zigbee-pro-w-rpsma-ant-xbp24-z7sit-004.html)
    * Digi : http://www.digi.com/products/model?mid=3587
  * **Antenna** : 2.4GHZ Dipole Half-Wave, 2.1 dBi, RPSMA male, articulating
    * Part Number : A24-HASM-450
    * Digi-Key : [A24-HASM-450-ND](http://parts.digikey.com/1/parts/635412-ant-2-4ghz-dipole-half-wave-a24-hasm-450.html)
    * Digi : http://www.digi.com/products/model?mid=2603

# Configuration #
Before our XBee modules can talk to each other, they need to be configured. This is done by connecting them to a PC and using some software to read and write their settings. To connect the XBee you'll need either an XBee USB Adapter (from [Adafruit](https://www.adafruit.com/products/247) or [Sparkfun](http://www.sparkfun.com/products/8687)) that the XBee connects directly to, or you can use an FTDI/USB adapter (from [Adafruit](https://www.adafruit.com/products/284) or [Sparkfun](http://www.sparkfun.com/products/9716)) to connect via the controller or receiver shields. The shields have a built-in XBee adapter based on an [Adafruit design](http://www.ladyada.net/make/xbee/).

The X-CTU application is downloadable from [Digi's website](http://www.digi.com/support/productdetail?pid=3352&osvid=0&type=utilities) (currently version 5.2.7.5, Windows only). Once X-CTU is installed and your XBee is connected to your PC, open Device Manager and note which COM port it is using (this is probably the last COM# listed under Ports). To verify that X-CTU can talk to the XBee, start the application, select the correct COM port on the left and then click the Test/Query button. If everything went well it should respond with something like this (if not see XbeeTroubleshooting)...
  * Communication with modem... OK
  * Modem type = XBP24BZ7
  * Modem firmware version = 21A0
  * Serial Number = 13A200 **40XXXXXX**

## Serial Numbers ##
Write down the last 8 digits of the serial number (probably starting with 40) and note where you will be using this XBee (is it going in the controller or the receiver?). In order to communicate with each other, the receiver Arduino will need to know the serial number of the controller's XBee and vice versa. Later we will edit our Arduino sketches with these serial numbers. These numbers can also be found printed on the belly of the XBees themselves as shown below.

![![](https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/XBee_Address_ID_sm.jpg)](https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/XBee_Address_ID.jpg)

## More Information ##
More Information about configuration of the XBEE radios for windows can be found in this PDF:

http://astromech.net/gallery2/main.php?g2_view=core.DownloadItem&g2_itemId=62276&g2_GALLERYSID=6f2bc30f5e8e668c90a2ffd58fb96b76

And for Mac, in these two forum posts:

http://astromech.net/forums/showpost.php?p=150410&postcount=327

http://astromech.net/forums/showpost.php?p=150413&postcount=328