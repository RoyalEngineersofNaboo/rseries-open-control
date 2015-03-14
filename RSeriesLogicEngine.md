


# Introduction #
The RSeries Logic Engine combines Arduino, RGB LEDs and fiber-optics to accurately emulate the color-wheel logic patterns seen in the original Star Wars trilogy.

At it's heart is an AVR Board (with Arduino Uno bootloader) which runs a series of WS2812B LEDs. These RGB LEDs cross-fade between set colors. For example the Front logic LEDs fade from black to blue to white and back again. As it arrives at each "key" color, that LED is paused for a random length of time - this creates constantly evolving color patterns that appear almost random at first glance.

Fiber-optic cable is used to route the light from each LED to specific 'pixels' on the logic bezel, which is what is finally seen on your droid.

# Assembly #
<table border='2'><tr><td>
<h1>September 2014 Kits</h1>
The plastics and hardware of the newer kits have changed slightly to simplify assembly. Because of this the assembly instructions below might not make complete sense for newer kits. I'm working on putting together assembly videos for the newer kits, but in the meantime you can see a rough video of the procedure here...<br>
<br>
<a href='http://www.youtube.com/watch?feature=player_embedded&v=1wT1KpOCRac' target='_blank'><img src='http://img.youtube.com/vi/1wT1KpOCRac/0.jpg' width='425' height=344 /></a><br>
</td></tr></table>
## Overview ##
The circuit boards come fully assembled, but you'll need to spend a little time putting them together with the fiber optics before they're ready to be installed in your dome. Assembly is simple, but can take a little time so set an evening aside to get everything together. The general procedure is...

  1. Inner screen, inner bezel and outer bezel are attached to the LED boards using screws and spacers.
  1. Fiber-optic cable is threaded through the outer bezel and into the inner bezel so it points directly at an LED.
  1. Once positioned the fiber-optic cable is trimmed to size at the outer bezel. A sharp wire-cutter should be used here to trim the end of the fiber flush with the bezel.
  1. With all fiber-optics placed the AVR board is mounted to the back of the LED board and we're done!

### `*` <font color='red'>Important Assembly Notes</font> `*` ###
<font color='red'>

<b>!</b> Never connect or disconnect LED boards from the AVR boards while powered; doing so can kill LEDs!<br>
<br>
<b>!</b> The plastic bezels are laser-cut and holes have a slight taper. This results in the openings of the "fiber holes" being slightly larger in diameter on one side. When assembling the bezels & screens these larger openings should face outward to make inserting the fiber-optic cable simpler. Bezels are <i>NOT symmetric</i>, so double check that you have them oriented the correct way up and correct way out.<br>
<br>
<b>!</b> The screws used to space the outer bezel away from the inner bezel should not protrude beyond the outer bezel. If you find that the end of your screws do poke out beyond the plastic of the outer bezel, dis-assemble and add some washers to increase spacing before you start placing any fiber-optics. If left protruding these screws can clash with the mounting hardware of the rear logic surround in the dome and cause you headaches down the line.<br>
<br>
<b>!</b> Mounting the AVR board to the back of an LED board can create a short if not done carefully. To be safe, trim down the back of the soldered Teeces pins so they're almost flush with the PCB surface, then cover them with a small piece of electrical tape. You may want to do the same with the OUT pins of the LED boards as an extra precaution.<br>
</font>

## Front Master ##
This is the upper front logic and connects directly to the AVR Board. The LED board has two sets of 3 pins; one set labeled **IN** and another labeled **OUT**. It is intended to mount the AVR Board directly to the back of the LED board, however during assembly it is safer so connect the AVR board to the LED board using one of the 3-wire cables.

**Hardware Required:**
  * (2) 35mm M3 screws
  * (2) 3/4" spacers
  * (2) 1/8" spacers
  * (X) washers
  * (2) M3 threaded brass inserts

To help diffuse the LED colors, lightly sand both sides of the inner-screen (the thin piece without fiber-optic holes) before assembly. 300-500 grit sandpaper should do the trick. Wipe all dust away afterwards.

Line up all the plastic parts with the LED PCB (the one with two sets of pins) to ensure they're all the correct way up.

<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/front_bez_orientation1.jpg' height='150'> <img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/front_bez_orientation2.jpg' height='150'>

Determine which side of the outer bezel will face out; we'll call this the front surface. Remove any paper liner from the front surface. Flip the bezel around so the back surface is facing up, then place the two brass inserts into their holes. Push them into place with some light force - a pliers may be used to squeeze them into place.<br>
<b>Note:</b> some builders have found that the holes for the brass inserts can be a hair bigger than they should be, causing the brass insert to pull out too easily. To help prevent this you may want to put a drop of superglue on the knurls of the brass insert.<br>
<br>
<img src='https://lh3.googleusercontent.com/-lSwxLmfYTJs/Ust0pwu70ZI/AAAAAAABxVE/lgt9h2CPcmM/w240/IMAG1748.jpg' />

Put plastic washers on both 35mm screws and position the screws through the PCB, inner screen and inner bezel. Then stack two washers, one 1/8" spacer and one 3/4" spacer onto each screw. Ensuring that you have the outer bezel positioned the correct way up, drive the two screws into the bezels brass inserts. Once secured, ensure that the screws don't protrude beyond the front surface of the bezel - if they do unscrew them and add a washer or two to the spacers.<br>Note: Optionally, to keep the assembly as compact as possible it is possible to use only the 3/4" spacer between the bezels though this makes positioning fibers a little trickier.<br>
<br>
<img src='https://lh4.googleusercontent.com/-Z_ehUj8IfkQ/Us6R84SdHJI/AAAAAAABxeY/7La_YN8uUYc/w240/IMAG1799.jpg' />

<h3>Fiber-Optic Placement</h3>

Take the bundle of fiber-optic cable and cut a tiny amount from the end to create a nice flat end with all fibers visible. A razor blade or sharp wire cutter can be used for this.<br>
<br>
<img src='https://lh4.googleusercontent.com/-RDuUFvauTmg/Ust0p-yiRvI/AAAAAAABxV8/TRxXGX0yKFI/w240/IMAG1773.jpg' />

Starting from the middle row, thread the end of the fiber-optic cable through a hole in the front surface of the outer bezel. A small needle-nose pliers or strong tweezers can be used to pull the cable through inside and position it into the corresponding hole of the inner bezel. Ensure that the cable is seated fully into the inner bezel.<br>
<br>
<img src='https://lh5.googleusercontent.com/-0gcoMXwQhKA/Ust0p_rlzRI/AAAAAAABxVE/3qp-HiTYi78/w240/IMAG1775.jpg' />
<img src='https://lh4.googleusercontent.com/-w62-2OKtRu8/Ust0p46Y0SI/AAAAAAABxVE/MKU5CbP7U-Y/w240/IMAG1776.jpg' />
<img src='https://lh6.googleusercontent.com/-wY8NQ3916oM/Ust0p7WAuGI/AAAAAAABxVE/wv7yBIuIXVg/w240/IMAG1777.jpg' />

Use a sharp flush-cutter to trim the fiber-optic cable bundle as close to the outer bezel as possible. After trimming the end of the remaining cable may appear "pinched" from the cutter so it may be necessary to trim a tiny portion of cable again (using a razor or sharp wire cutter).<br>
<br>
Continue this procedure until fiber-optic cable has been placed in all holes of the bezel.<br>
<br>
<h2>Front Slave</h2>
This is the lower front logic display. Assembly procedure is identical to the upper front logic. Once assembled, the Front Slave is connected to the Front Master using the short 3-wire jumper cable as shown here (click for larger image)...<br>
<a href='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/fld-connections.png'><img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/fld-connections_th.png' /></a>

<h2>Rear</h2>
Again, while assembling the rear logic it is safer to leave the AVR board detached from the LED boards. The AVR board can be connected to the LED board during assembly using a 3-pin cable. Once the fiber-optics are in place the AVR board can be mounted to the back of the LED boards if you so wish.<br>
<br>
Just like the fronts, make sure you get the inner screen, inner bezel and outer bezel the right way up and out. The bottom edge of these parts have little half-circle keys on them to help figure it out. If you do get them upside-down it won't cause problems like the fronts, so don't worry too much about it...<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rear_bez_orientation1.jpg' height='180'>

The plastics for the rear are assembled similarly to the fronts. You'll notice that the center of the rear 'inner bezel' has a hexagonal cutout; this is for placing a hex nut. Use the 16mm screw (with a plastic washer) to secure the center mounting hole of the LED board to the hex nut.<br>
<br>
Before you start placing the fiber-optics, there's an issue to be aware of. The middle of the RLD can be forced to bow out by the fiber-optics and this might not be noticeable until you're done.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rld_bowed.jpg' height='180'>

To minimize this bowing we want to pull the middle of the bezel in slightly during assembly. One way to achieve this is to put screws through the bezel's center mounting holes and secure them using some nuts and washers. With the screws in place, loop a cable-tie around the screws and over the back of the assembly. Tighten the cable-tie until the middle of the bezel is pulled in very slightly. This should prevent the middle of the bezel to spring out during assembly.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rld-tied1.jpg' height='240'> <img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rld-tied2.jpg' height='240'>

The fiber optic cables on the rear should be placed in a specific way to ensure that everyone has their logics mapped identically. To make this simpler I have built in a 'Testpattern Mode' into the code. On the Rear AVR board, remove the S3 jumper (if it exists) and turn the DELAY trimmer completely counter-clockwise. Restart and you should see a color pattern like this for a few minutes (you may need to reset the AVR board occasionally to get back to this pattern during assembly)...<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rld_pattern.png' />

Now, starting from the center and working outwards, fibers should be routed through the outer bezel and into the inner bezel so the color pattern on the outer bezel ends up looking like this...<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rld_patternbez.png' />

The outer-most fibers shown in blue and pink will be the trickiest to position, so take extra care (and time) with those. Again, a small needle-nose pliers or strong tweezers can come in very useful when positioning the fibers.<br>
<br>
<a href='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/rld-pattern-numbered.png'>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/RLD-Pattern-Numbered_th.png' /></a>

If after assembly you find that the middle of the RLD is bowed out, don't panic! Loosen the two spacer screws a few turns and the bowing should subside slightly. When mounting the assembly to your logic surrounds the bowing should disappear.<br>
<br>
<h2>Piggybacking the AVR Board</h2>
To keep things compact you might want to mount the AVR board to the back of the LED board instead of having it connected by the 3-wire cable. To do this you'll need to replace the spacer screws with something a little longer. On the Front Master you'll replace the 35mm screws with 40mm screws. On the Rear you'll replace the 35mm screw beside the IN pins with a 40mm one.<br>
<br>
To ensure that the fiber-optics don't come out of place during this procedure, wrap some masking tape tightly around the assembly <b>BEFORE YOU REMOVE ANY SCREWS</b>. With the screws removed, attach the AVR board. The LED board's 3 pins should fit securely through the back of the AVR board and into its wacky socket. Screw in the 40mm screw next to the 3 pins first, putting the spacers back in place as you do so. For the opposite screw you will want to use one of the 1/8" spacers or some washers between the AVR and LED board to keep the boards roughly parallel. Additional washers may be needed to ensure the screw doesn't. Now remove the masking tape and you're good to go!<br>
<br>
<h2>Mounting To Logic Surrounds</h2>

<font color='red'><b>WARNING!</b> Several builders have encountered problems when mounting the Rear Logic assembly to its surround. While tightening the assembly to the surround the threaded insert has loosened and slipped out; in some cases losing all the precious fiber-optics! Take care when tightening the nuts; turn them slowly and watch the threaded insert at all times. A drop of glue around the insert may help. This problem is more common where the rear bezel has bowed during assembly and does not affect the front assembly.</font>

<b>Hardware Required:</b>
<ul><li>(14) M3 set screws (12mm or 16mm long)<br>
</li><li>(14) M3 hex nuts</li></ul>

Screw the set screws into the mounting holes of the logic surrounds (4 for each front logic, 6 for the rear logic). Tighten using a 1.5mm hex key. If the set screws appear a little loose in the surround you may want to use a drop of threadlocker fluid.<br>
<br>
Place the clear screen over the set screws, then position the logic engine assembly in place. The set screws will go through the outer bezel, leaving enough thread to be secured with the hex nuts. The hex nuts can prove to be very tricky to place and tighten - it may help to find someone with small fingers and bribe them into helping. Another trick is to hook the nut onto the end of your 1.5mm hex key, then place the key onto the set screw; this prevents the nut from falling while you position and tighten it.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/Logic_Engine_Parts.png' />
<hr />
<h1>Powering</h1>
The AVR board features an efficient regulator module that is capable of supplying plenty of current (up to 2.25A) to the AVR and LED boards. It can take an input voltage between +6V and +17V, so you can safely connect power from a 12V battery.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/avr_powering.png' />

<h1>Standard Settings</h1>

The AVR board can be set to produce standard <a href='https://code.google.com/p/rseries-open-control/source/detail?r=2'>R2</a>-D2 logic colors and speeds for both the Front (FLD) and Rear (RLD) Logic Displays.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/avr_mode.png' />

By default the AVR board will output FLD colors (black, blues, whites) & speeds. Placing a jumper/shunt on the <b>S4</b> pin switches it to RLD mode (slower black, greens, yellows, reds).<br>
<br>
<h1>Custom Settings</h1>
The <b>BRIGHT</b> and <b>COLOR</b> trimpots on the AVR board are used to adjust global brightness and hue values of all LEDs.<br>
<br>
Using a small screwdriver to turn the <b>BRIGHT</b> trimpot completely counter-clockwise sets the LEDs to their darkest levels (ie black). Turning the <b>BRIGHT</b> trimpot slowly clockwise will increase brightness until the maximum brightness is achieved. This maximum brightness value is set to 50% of the LED's possible brightness. This limit is in place to keep current consumption and heat generation down, and also to prevent anyone from being blinded (they're insanely bright at 100%!!). A custom settings file on the microSD card can be used to bypass this safety feature and get 100% brightness - this not recommended for long periods of time so do so at your own risk.<br>
<br>
Similarly turning the <b>COLOR</b> trimpot completely counter-clockwise sets the color palette to their default hues (FLD will be black/blue/white, RLD will be black/green/yellow/red). Slowly turning the <b>COLOR</b> trimpot clockwise will shift the hues of all colors through the full color spectrum, finally arriving at the same default hues again when turned completely clockwise.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/avr_speed.png' />

Additionally, if different speeds are desired a jumper can be placed on the <b>S3</b> pin to enable the <b>DELAY</b> and <b>FADE</b> trimpots. Delay controls how long each key color is paused for. Fade controls how long each "tween" color is paused for - this adjusts how long each key color takes to cross-fade into the next color. When turned completely counter-clockwise the LEDs will behave fastest, turning clockwise slows the LEDs.<br>
<br>
Additional custom settings (such as specific color palettes) may be set by editing the settings.txt file on the microSD card. The microSD card is optional and not needed for basic functionality.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/avr_microsd.png' />

<h1>Connecting a PSI</h1>
The AVR board is also programmed to run a Teeces v3.2 PSI if you have one. To get your PSI running, just connect it using a 5-pin jumper cable like this...<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/avr_to_teeces_psi.png' />

<h1>Reprogramming</h1>
For basic functionality, the AVR board should never need to be reprogrammed. If, however, a future update should be released or you just like to play with the code, the AVR board can be reprogrammed using the Arduino IDE and an FTDI adapter. In the Arduino IDE software you should select 'Arduino UNO' from the Tools->Board menu.<br>
<br>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/avr_ftdi.png' />

The basic Arduino sketches are available on the repository <a href='https://code.google.com/p/rseries-open-control/source/browse/trunk#trunk%2FSoftware%2FLogicEngine'>here</a>.<br>
<br>
<h1>Development Notes</h1>
This system is basically an Arduino running a bunch of WS2812B LEDs. WS2812B's require only one data wire from a microcontroller to run dozens (maybe hundreds) of the RGB LEDs. We use functions from the <a href='https://code.google.com/p/fastspi'>FastSPI_LED2 Library</a> to control all the LEDs, assigning them HSV (Hue Saturation Value) color values and address each LED in the order it is wired.<br>
<br>
In order to pack all the LEDs to closely on the PCBs, they have been wired in a serpentine configuration. Each LED board has 48 LEDs. For the Front Logic two boards are connected via a 3-pin jumper cable and the top row of LEDs is unused on each logic. For the Rear Logic two boards are soldered together side-by-side and all 96 LEDs are used. These odd configurations are simplified in the software by mapping the physical LED numbers to typical matrix numbering.<br>
<br>
<a href='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/Logic-Engine-LED-board-front.png'>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/Logic-Engine-LED-board-front.png' width='210'>
<a href='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/Logic-Engine-LED-board-rear.png'>
<img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/Logic-Engine-LED-board-rear.png' width='400'>

<h1>Where'd this come from?</h1>
These logics are the result of a couple of years of tinkering and development. The Teeces logics are great, but the PWM fading seen in JEDI logics was always a much sought after feature. I worked with John (Teeces) for some time to come up with a method of making fadeable logics. We discovered that it may be possible via software PWM, but would require whole new logic boards. I then discovered that by using bi-color LEDs we could have LEDs fade between colors, much like the original trilogy logics - however, the LEDs couldn't be placed close enough to each other so fiber optic cable was required to get correct spacing. Then I discovered Rainbowduino's and built <a href='https://www.youtube.com/watch?v=Z9KnvJx7TDs'>those RGB logics seen at DroidCon2</a>. There, Michael Erwin and Brett Bourbin convinced me to rework the design from scratch to better suit our needs - in doing so the RSeries Logic Engine was born.