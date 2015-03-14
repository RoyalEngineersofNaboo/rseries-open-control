#details of microSD card usage and animation sequencing

# cfg File #
The cfg file is a simple text file saved to the root of the microSD card. It should be named "cfg" with no file extension. The file should contain two lines of text.

The first line should contain several comma separated numbers indicating...

> 0/1 : 0 for Front, 1 for Rear

> 0-15 : number of 'tween' colors to generate between key colors

> 0-255 : number of milliseconds to pause each Tween color (can be adjusted by the Fade trimmer)

> 0-9999 : maximum number of milliseconds to pause each Key color (can be adjusted by the Delay trimmer)

> 0/1 : 0 for preset speeds, 1 to enable the Delay and Fade trimmers.

> 0-255 : maximum brightness allowed (using a value of 128 or lower is recommended)

The second line should be a comma separated list of numbers signifying the default colors to be used.

If you're using prototype FLD boards with only 40 LEDs, a third line should be added with a "1".

# Animation Files #
Animations are stored as simple files. The first line will contain a single number, defining which Animation Type (see list below) we're dealing with. The remaining lines will be formatted differently depending on the Animation Type.

## Animation Types ##

0 : Frame by frame animation

1 : Modifier (temporarily overrides the standard colors & speeds)

2 : Text/character scroll

3 : Sequence of several other animations